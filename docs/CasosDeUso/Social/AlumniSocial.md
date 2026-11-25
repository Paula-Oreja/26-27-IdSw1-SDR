@startuml

title Plataforma Alumni - Módulo social

left to right direction

skinparam shadowing false
skinparam packageStyle rectangle
skinparam actorStyle awesome

actor Alumni
actor "Alumni autorizado" as Autorizado
actor Administrador
actor Empresa

Autorizado --|> Alumni

rectangle "Módulo social" {

    usecase "Buscar Alumni" as CU08
    usecase "Consultar perfil de otro Alumni" as CU09
    usecase "Consultar eventos" as CU10
    usecase "Inscribirse en evento" as CU11
    usecase "Cancelar inscripción" as CU12
    usecase "Consultar participantes" as CU13
    usecase "Crear evento" as CU14
    usecase "Proponer evento" as CU15

}

Alumni -- CU08
Alumni -- CU09
Alumni -- CU10
Alumni -- CU11
Alumni -- CU12
Alumni -- CU13

Autorizado -- CU14
Administrador -- CU14

Empresa -- CU15

@enduml