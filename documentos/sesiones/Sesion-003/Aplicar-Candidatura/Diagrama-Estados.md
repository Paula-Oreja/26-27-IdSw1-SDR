@startuml
title Diagrama de Estados - Ciclo de Vida de una Candidatura
skinparam state {
  BackgroundColor white
  BorderColor black
  ArrowColor black
}

[*] --> Borrador : Alumni inicia postulación

state Borrador {
  [*] --> ValidandoRequisitos
  ValidandoRequisitos --> ListoParaEnviar : CV adjunto y consentimiento aceptado
}

Borrador --> Enviada : confirmarPostulacion()
Borrador --> [*] : cancelarBorrador()

state Enviada : entry / notificarEmpresa()
Enviada --> EnRevision : empresaVisualizaPerfil()
Enviada --> Retirada : alumniCancelaPostulacion()

state EnRevision
EnRevision --> EnEntrevista : preseleccionarCandidato()
EnRevision --> Rechazada : descartarCandidato()
EnRevision --> Retirada : alumniRetiraConsentimiento()

state EnEntrevista
EnEntrevista --> Seleccionada : emitirOfertaFinal()
EnEntrevista --> Rechazada : descartarTrasEntrevista()
EnEntrevista --> Retirada : alumniAbandonaProceso()

state Seleccionada : entry / registrarContratacion()
state Rechazada : entry / notificarDescarte()
state Retirada : entry / revocarAccesoDatosEmpresa()

Seleccionada --> [*]
Rechazada --> [*]
Retirada --> [*]
@enduml
