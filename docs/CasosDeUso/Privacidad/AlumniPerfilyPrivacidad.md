@startuml

title Plataforma Alumni - Perfil y privacidad

left to right direction

skinparam shadowing false
skinparam packageStyle rectangle
skinparam actorStyle awesome

actor Alumni

rectangle "Gestión del perfil y privacidad" {

    usecase "Crear perfil profesional" as CU01
    usecase "Consultar perfil profesional" as CU02
    usecase "Editar perfil profesional" as CU03
    usecase "Incorporar currículum" as CU04
    usecase "Actualizar currículum" as CU05
    usecase "Configurar privacidad" as CU06
    usecase "Gestionar autorizaciones de datos" as CU07

}

Alumni -- CU01
Alumni -- CU02
Alumni -- CU03
Alumni -- CU04
Alumni -- CU05
Alumni -- CU06
Alumni -- CU07

@enduml