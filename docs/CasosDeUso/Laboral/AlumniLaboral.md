@startuml

title Plataforma Alumni - Módulo laboral

left to right direction

skinparam shadowing false
skinparam packageStyle rectangle
skinparam actorStyle awesome

actor Alumni
actor Empresa

rectangle "Módulo laboral" {

    usecase "Consultar ofertas de empleo" as CU16
    usecase "Presentar candidatura" as CU17
    usecase "Consultar candidaturas propias" as CU18

    usecase "Publicar oferta de empleo" as CU19
    usecase "Editar oferta de empleo" as CU20
    usecase "Retirar oferta de empleo" as CU21
    usecase "Consultar candidaturas recibidas" as CU22
    usecase "Gestionar candidaturas" as CU23
    usecase "Contactar con candidato" as CU24

}

Alumni -- CU16
Alumni -- CU17
Alumni -- CU18

Empresa -- CU19
Empresa -- CU20
Empresa -- CU21
Empresa -- CU22
Empresa -- CU23
Empresa -- CU24

@enduml