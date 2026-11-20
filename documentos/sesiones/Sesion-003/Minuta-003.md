# Sesión 003 de Requisitado con el cliente

## 1. Información general de la sesión

1. **Fecha:** 2026-11-18.
2. **Hora de inicio:** 15:15
3. **Equipo:** Paula Oreja, Bamba Niang, Miguel Gómez, Alexis,Mario Osorio, José Melgares y Miguel Rojas.
4. **Cliente:** Jesús Peña.
5. **Modalidad:** Presencial.
6. **Proyecto:** Plataforma Alumni UNEATLANTICO.

### 1.1. Registro de asistencia

A continuación, se recoge la asistencia de los integrantes del equipo a la tercera sesión de requisitado con el cliente.

| Integrante | Asistencia |
|---|:---:|
| Miguel Gómez | Sí |
| Bamba Niang | Sí |
| Alexis | Sí |
| Miguel Rojas | No |
| Mario Osorio | Sí |
| José Melgares | Sí |
| Paula Oreja | Sí |
| **Total** | **6/7 (85,71%)** |

## 2. Objetivo de la sesión

### 2.1. Objetivo general

Presentar al cliente los avances realizados en la definición de la Plataforma Alumni UNEATLANTICO, con el propósito de validar las propuestas elaboradas por el equipo, aclarar los requisitos identificados en sesiones anteriores y recoger nuevas necesidades que permitan continuar con el desarrollo del proyecto.

### 2.2. Objetivos específicos

- Presentar y revisar los diagramas de casos de uso propuestos para los diferentes actores de la plataforma.
- Revisar el modelo del dominio y las relaciones identificadas entre sus principales entidades.
- Aclarar los requisitos relacionados con la gestión del perfil profesional y la privacidad de los datos personales.
- Definir el alcance del módulo social y la participación de la universidad, los Alumni y las empresas.
- Concretar las funcionalidades relacionadas con la publicación de ofertas de empleo y la presentación de candidaturas.
- Identificar los mecanismos de administración y las métricas que resultan de interés para la universidad.

## 3. Desarrollo de la sesión

### 3.1. Presentación de los avances del proyecto

El equipo inició la presentación mostrando los diagramas elaborados a partir de las necesidades identificadas en las reuniones anteriores.

Se presentaron los casos de uso correspondientes a la gestión del perfil y la privacidad, el módulo social y de networking, las funcionalidades del administrador y el módulo laboral.

También se mostró el modelo del dominio, con las principales entidades de la plataforma y las relaciones existentes entre ellas.

El cliente realizó observaciones sobre las funcionalidades propuestas, señalando la necesidad de diferenciar los requisitos solicitados de aquellas funcionalidades adicionales planteadas por el equipo.

### 3.2. Gestión del perfil profesional y protección de datos

Se presentó la propuesta de permitir que los Alumni gestionen su perfil profesional, incorporando información personal, formación, trayectoria laboral, intereses y currículum.

El cliente destacó la importancia de establecer una gestión específica de la privacidad, indicando que no resulta adecuado utilizar una única autorización general para todos los datos y funcionalidades de la plataforma.

Se aclaró que deben diferenciarse los datos necesarios para acceder al servicio de aquellos utilizados para finalidades adicionales.

Asimismo, se señaló que las autorizaciones deben especificar qué datos se utilizan, para qué finalidad, durante cuánto tiempo y bajo qué condiciones se conservan, modifican o eliminan.

El cliente recordó que los Alumni podrían utilizar diferentes servicios de la plataforma, como el módulo social o el laboral, sin estar obligados a participar en todos ellos. Por ello, cada servicio podría requerir condiciones y autorizaciones diferentes.

En relación con el currículum, se planteó que el Alumni pudiera incorporarlo a su perfil para utilizarlo posteriormente al presentar candidaturas. El cliente indicó que debe informarse adecuadamente al usuario cuando sus datos vayan a compartirse con una empresa.

Quedó pendiente concretar el procedimiento de autorización más adecuado para la comunicación de información profesional a las empresas.

### 3.3. Módulo social y networking

Durante la revisión del módulo social, el equipo presentó funcionalidades relacionadas con la búsqueda de otros Alumni, la consulta de perfiles, la participación en comunidades y la organización de eventos.

El cliente aclaró que el objetivo principal de este módulo es favorecer la conexión entre antiguos alumnos y promover actividades vinculadas a la universidad, como encuentros de promociones, conmemoraciones, conferencias y otras iniciativas de carácter social o académico.

Se identificó una diferencia de interpretación respecto a la participación de las empresas. El equipo había contemplado que estas pudieran intervenir directamente en el espacio social y publicar actividades propias.

El cliente explicó que las actividades empresariales deben mantenerse diferenciadas del espacio social de los Alumni, para evitar que las publicaciones comerciales desplacen los contenidos de interés universitario.

Se estableció que las empresas podrán proponer actividades a la universidad, pero no publicarlas directamente en el módulo social. La universidad será responsable de valorar dichas propuestas y decidir si procede su publicación.

También se contempló la posibilidad de que los participantes en un evento puedan consultar quiénes se han inscrito, siempre que los usuarios hayan autorizado la visibilidad de esa información.

### 3.4. Organización y gestión de eventos

El cliente explicó que la gestión de los eventos debe permanecer bajo el control de la universidad.

La creación y publicación de actividades podrá realizarse mediante el administrador o mediante determinados Alumni a quienes la universidad haya concedido responsabilidades específicas.

Estos Alumni autorizados podrán colaborar en la coordinación de actividades, sin que ello implique que cualquier usuario pueda organizar y publicar eventos libremente.

Se mencionaron diferentes tipos de actividades, como encuentros presenciales, reuniones de promociones, conferencias y seminarios en línea.

El cliente también planteó la conveniencia de recoger autorizaciones específicas relacionadas con el uso de imágenes de los asistentes en fotografías y publicaciones de los eventos.

Por tanto, deberá contemplarse la gestión de los permisos correspondientes cuando un Alumni se inscriba en una actividad.

### 3.5. Funcionalidades del administrador

Se revisaron los casos de uso relacionados con la administración de la plataforma.

El equipo presentó funcionalidades como la revisión de ofertas de empleo, la moderación de contenidos, la gestión de eventos y la consulta de métricas.

El cliente señaló que el administrador debe disponer de capacidad para gestionar los perfiles de los Alumni y las empresas, incluyendo las posibles bajas de usuarios.

Asimismo, destacó la necesidad de contemplar la asignación de permisos especiales a determinados Alumni, que podrán asumir funciones de coordinación o moderación dentro del módulo social.

Se reafirmó que la universidad debe mantener el control sobre las actividades y contenidos publicados en sus espacios institucionales.

### 3.6. Métricas e información de la plataforma

Durante la presentación de las funcionalidades del administrador, el equipo propuso consultar métricas relacionadas principalmente con la empleabilidad.

El cliente indicó que la universidad necesita obtener información de todos los módulos de la plataforma, no únicamente de las ofertas de empleo y las contrataciones.

Se mencionaron como ejemplos de información de interés:

- Número de Alumni y empresas registrados.
- Ofertas de empleo publicadas.
- Candidaturas e interacciones entre Alumni y empresas.
- Propuestas de eventos recibidas.
- Participación de los Alumni en las actividades.
- Actividad de las diferentes comunidades y promociones.
- Interacciones generadas dentro de cada módulo.

El cliente destacó que esta información puede resultar útil para conocer el grado de participación de los antiguos alumnos, identificar comunidades activas y valorar futuras iniciativas universitarias.

Por tanto, se deberá contemplar la obtención de métricas relacionadas con cada uno de los servicios de la plataforma.

### 3.7. Módulo laboral y candidaturas

El equipo presentó las funcionalidades relacionadas con la consulta de ofertas de empleo por parte de los Alumni y la publicación de ofertas por parte de las empresas.

También se planteó la posibilidad de que las empresas gestionen las candidaturas recibidas y establezcan contacto con los candidatos.

El cliente volvió a destacar la importancia de la protección de datos en estos procesos, especialmente cuando el Alumni decide compartir su currículum con una empresa.

Se consideró la posibilidad de informar al usuario, en el momento de incorporar o utilizar su currículum, de las condiciones en las que será compartido al presentar una candidatura.

No se concretó definitivamente el procedimiento, por lo que será necesario continuar analizando los permisos y las condiciones de utilización de la información personal.

### 3.8. Comunicación entre Alumni

El equipo consultó al cliente sobre la posibilidad de incorporar mensajes privados entre los Alumni.

El cliente explicó que la finalidad de la plataforma no es convertirse en una red social generalista ni incorporar funcionalidades complejas de mensajería.

Como alternativa, planteó que los usuarios puedan disponer de información de contacto, siempre que autoricen su visualización.

Se mencionó la posibilidad de mostrar determinados datos del perfil, como la titulación, la promoción o la participación en eventos, dependiendo de las preferencias de privacidad del usuario.

También se consideró que los espacios de participación vinculados a comunidades o publicaciones podrían permitir comentarios e interacciones sencillas.

La incorporación de un sistema de mensajería privada no quedó establecida como requisito prioritario.

### 3.9. Revisión del modelo del dominio y presentación al cliente

En la parte final de la reunión se mostró el modelo del dominio elaborado por el equipo.

El cliente observó que la representación presentada resultaba compleja de interpretar debido al elevado número de elementos y relaciones.

Señaló que los diagramas pueden resultar útiles para el trabajo académico y técnico, pero que, cuando se presentan a un cliente, deben facilitar la comprensión de la solución propuesta.

El cliente recomendó priorizar la claridad de las explicaciones y adaptar la presentación a las necesidades de la asignatura.

Asimismo, insistió en la importancia de que los integrantes del equipo compartan y contrasten sus interpretaciones de los requisitos, para evitar desarrollar funcionalidades que no respondan a las necesidades expresadas.

## 4. Conclusiones

La sesión permitió revisar los avances del proyecto y aclarar aspectos relevantes de las funcionalidades propuestas.

Se obtuvieron las siguientes conclusiones:

1. La gestión de la privacidad debe diferenciar los datos necesarios para el funcionamiento de la plataforma de aquellos utilizados para finalidades adicionales, mediante las autorizaciones que correspondan.

2. El módulo social debe centrarse en la comunidad Alumni y las actividades relacionadas con la universidad, manteniéndose diferenciado de los espacios propios de las empresas.

3. La creación y publicación de eventos debe permanecer bajo el control de la universidad, aunque determinados Alumni autorizados puedan colaborar en su gestión.

4. Las empresas podrán proponer actividades, pero su publicación en el espacio social dependerá de la aprobación y gestión de la universidad.

5. Las métricas deben abarcar los diferentes módulos de la plataforma, permitiendo conocer tanto la actividad laboral como la participación social de los Alumni.

6. El módulo laboral deberá contemplar la comunicación de datos personales y currículums a las empresas con las condiciones y autorizaciones correspondientes.

7. La mensajería privada no constituye una funcionalidad prioritaria. Se considera más adecuado estudiar mecanismos sencillos de contacto y participación.

8. El equipo deberá mejorar la claridad de los diagramas y comprobar que las funcionalidades representadas se corresponden con los requisitos expresados por el cliente.

## 5. Próximos pasos

De cara a la siguiente sesión, el equipo se propone:

1. **Actualizar los diagramas de casos de uso**, incorporando las aclaraciones realizadas por el cliente y diferenciando correctamente las funcionalidades de cada actor.

2. **Revisar el modelo del dominio**, teniendo en cuenta las relaciones entre Alumni, empresas, administradores, eventos, perfiles profesionales y autorizaciones de datos.

3. **Profundizar en la gestión de la privacidad**, identificando qué información se utiliza en cada servicio y qué autorizaciones pueden resultar necesarias.

4. **Reorganizar el módulo social**, diferenciando las actividades universitarias de las propuestas empresariales y estableciendo los permisos de creación y publicación de eventos.

5. **Ampliar las funcionalidades del administrador**, contemplando la gestión de perfiles, la asignación de responsabilidades y las métricas de los diferentes módulos.

6. **Revisar el proceso de presentación de candidaturas**, especialmente la utilización del currículum y la autorización para comunicar datos a las empresas.

7. **Simplificar la presentación de los modelos**, con el objetivo de facilitar su comprensión durante las próximas reuniones.

8. **Preparar las cuestiones pendientes de validación**, especialmente las relacionadas con la privacidad, la visibilidad de los perfiles y los mecanismos de contacto entre usuarios.

## 6. Cuestiones pendientes de aclaración

Quedan pendientes de concretar con el cliente los siguientes aspectos:

- Qué datos del perfil Alumni serán obligatorios y cuáles opcionales.
- Qué información del perfil podrá consultar cada tipo de usuario.
- Cómo se gestionarán las autorizaciones específicas de privacidad.
- En qué momento se solicitará autorización para compartir el currículum con las empresas.
- Qué funcionalidades concretas tendrán los Alumni autorizados para coordinar eventos.
- Qué mecanismos de contacto entre Alumni se incorporarán finalmente.
- Qué métricas específicas se considerarán prioritarias para la universidad.
