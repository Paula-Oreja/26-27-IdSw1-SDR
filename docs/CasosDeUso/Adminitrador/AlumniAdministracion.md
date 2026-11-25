@startuml

title Plataforma Alumni - Administración

left to right direction

skinparam shadowing false
skinparam packageStyle rectangle
skinparam actorStyle awesome

actor Administrador

rectangle "Administración" {

    usecase "Validar empresa" as CU25
    usecase "Revisar oferta de empleo" as CU26
    usecase "Gestionar perfiles Alumni" as CU27
    usecase "Gestionar perfiles de empresas" as CU28
    usecase "Asignar permisos a Alumni" as CU29
    usecase "Revisar propuesta de evento" as CU30
    usecase "Publicar evento" as CU31
    usecase "Moderar contenidos" as CU32
    usecase "Consultar métricas" as CU33

}

Administrador -- CU25
Administrador -- CU26
Administrador -- CU27
Administrador -- CU28
Administrador -- CU29
Administrador -- CU30
Administrador -- CU31
Administrador -- CU32
Administrador -- CU33

@enduml