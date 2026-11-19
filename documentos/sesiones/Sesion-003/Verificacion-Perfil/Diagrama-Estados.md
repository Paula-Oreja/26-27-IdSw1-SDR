@startuml perfilProfesionalAlumni

title Plataforma Alumni UNEATLANTICO\nCreacion del Perfil Profesional

top to bottom direction
skinparam linetype polyline
skinparam shadowing false
skinparam nodesep 75
skinparam ranksep 85

state "SIN PERFIL" as SIN_PERFIL
state "PERFIL INCOMPLETO" as INCOMPLETO
state "PERFIL COMPLETO" as COMPLETO
state "PERFIL VERIFICADO" as VERIFICADO

' CREAR PERFIL

state "Crear perfil profesional" as CrearPerfil {

    state "Introducir datos" as Datos
    state "Añadir experiencia" as Experiencia
    state "Incorporar currículum" as Curriculum
    state c1 <<choice>>

    [*] -[#green]-> Datos
    note on link
    <b>Alumni</b> solicita crear perfil
    <b>Sistema</b> presenta formulario
    end note

    Datos -[#green]-> Experiencia
    note on link
    <b>Alumni</b> introduce formación,
    idiomas e intereses
    end note

    Experiencia -[#green]-> Curriculum
    note on link
    <b>Alumni</b> añade experiencia laboral
    end note

    Curriculum -[#green]-> c1
    note on link
    <b>Alumni</b> incorpora currículum
    y solicita guardar
    end note

    c1 -[#green]-> [*] : datos completos
    c1 -[#red]-> Datos : faltan datos
}

[*] -[#green]-> SIN_PERFIL

SIN_PERFIL -[#green]-> CrearPerfil
INCOMPLETO -[#green]-> CrearPerfil : continuar perfil

CrearPerfil -[#green]-> COMPLETO : perfil guardado
CrearPerfil -[#red]-> INCOMPLETO : perfil pendiente

' VERIFICAR PERFIL

state "Verificar perfil" as Verificar {

    state "Revisar información" as Revisar
    state c2 <<choice>>

    [*] -[#green]-> Revisar
    note on link
    <b>Administrador</b> revisa
    los datos del Alumni
    end note

    Revisar -[#green]-> c2

    c2 -[#green]-> [*] : verificado
    c2 -[#red]-> [*] : requiere corrección
}

COMPLETO -[#green]-> Verificar

Verificar -[#green]-> VERIFICADO : datos aceptados
Verificar -[#red]-> INCOMPLETO : corregir datos

VERIFICADO -[#green]-> [*]

@enduml
