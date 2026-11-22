@startuml cicloOfertaEmpleo

title Plataforma Alumni UNEATLANTICO\nDiagrama de Estados - Oferta de Empleo

top to bottom direction
skinparam linetype polyline
skinparam shadowing false
skinparam nodesep 75
skinparam ranksep 90

state "PROPUESTA" as PROPUESTA
state "PENDIENTE_REVISION" as PENDIENTE
state "PUBLICADA" as PUBLICADA
state "RECHAZADA" as RECHAZADA
state "CERRADA" as CERRADA

[*] -[#green]-> PROPUESTA
note on link
<b>Empresa</b> propone una oferta de empleo
end note

PROPUESTA -[#green]-> PENDIENTE
note on link
<b>Sistema</b> registra la oferta
como pendiente de revisión
end note

state revisionOferta as "revisarOfertaEmpleo()" {

    state " " as ConsultandoOferta
    state " " as DecidiendoRevision
    state c1 <<choice>>

    [*] -[#green]-> ConsultandoOferta
    note on link
    <b>Administrador</b> solicita
    revisar una oferta
    end note

    ConsultandoOferta -[#green]-> DecidiendoRevision
    note on link
    <b>Sistema</b> presenta
    información de la oferta

    <b>Sistema</b> permite solicitar:
    - aprobar
    - rechazar
    end note

    DecidiendoRevision -[#green]-> c1
    note on link
    <b>Administrador</b> comunica
    su decisión
    end note

    c1 -[#green]-> [*]
    note on link
    oferta aprobada
    end note

    c1 -[#red]-> [*]
    note on link
    oferta rechazada
    end note
}

PENDIENTE -[#green]-> revisionOferta
note on link
<b>Administrador</b> solicita
revisar oferta
end note

revisionOferta -[#green]-> PUBLICADA
note on link
oferta aprobada

<b>Sistema</b> presenta
la oferta a los Alumni
end note

revisionOferta -[#red]-> RECHAZADA
note on link
oferta rechazada

<b>Sistema</b> registra
el rechazo
end note

PUBLICADA -[#green]-> CERRADA
note on link
<b>Empresa</b> solicita
cerrar la oferta

<b>Sistema</b> registra
el cierre
end note

RECHAZADA -[#red]-> [*]
CERRADA -[#green]-> [*]

@enduml
