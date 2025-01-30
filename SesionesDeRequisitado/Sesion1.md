<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Priorización_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Priorizacion.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |

</div>


# Sesión de requisitado #1
Fecha: 16 de octubre, 2024

# Información General
**Cliente**: Parte del departamento de calidad. Jorge Crespo Alvarez.

**Proyecto**: Automatización de la actualización del contenido de las guías docentes.

**Problema principal**: Parte del contenido de las guías docentes debe actualizarse anualmente, y en el caso de asignaturas impartidas en varias titulaciones, el contenido puede variar, lo que hace ineficiente el uso del copiar y pegar, ya que son demasiadas guias docentes y el proceso manual se torna engorroso. 

## Proceso Actual
- Las guías docentes son creadas usando una plantilla en Word que contiene campos que deben rellenarse para cada asignatura.
- Este proceso es repetitivo, manual y propenso a errores. Por ejemplo, al inicio de cada semestre, deben gestionarse las guías para todas las asignaturas de todas las titulaciones.
- Esto implica gestionar alrededor de 900 guias docentes al año, sin contar los másteres.

## Problemas Identificados
- **Contenido Estático y no estático**: Algunos contenidos no cambian y otros se deben actualizar manualmente cada año.

- **Multiplicidad de Titulaciones**: Asignaturas impartidas en varias titulaciones requieren guías docentes distintas, ya que el contenido/objetivos/competencias,etc varían.

- **Errores y Compatibilidad**: El proceso actual utiliza Google Drive para almacenar guías en formato Word, lo que genera problemas de compatibilidad y errores al abrir los archivos en Google Docs. 

## Necesidades del Cliente

**Automatización**: Desean una aplicación que automatice el proceso de actualización de las guías, minimizando la intervención manual.

**Roles y Permisos**: Es importante tener un sistema de usuarios con roles claramente definidos y permisos de edición limitados a ciertos campos.

- **Profesor**: Puede editar campos específicos como el nombre del profesor, su email, el contenido de la asignatura, las actividades de evaluación y bibliografía.

- **Director de Grado**: Aprueba o rechaza las propuestas de guías enviadas por los profesores.

- **Técnico de Calidad**: Tiene permisos para editar toda la guía, incluso los campos estáticos, ya que gestionan cambios a nivel de titulación.

- **Dirección de Calidad**: Supervisa el trabajo del técnico y audita el trabajo del director de grado y los profesores.

**Flexibilidad**: La aplicación debe ser flexible, permitiendo que una persona tenga varios roles, como un profesor que también sea director de grado.

**Control de Asignación**: Debe haber un control en la asignación de roles y privilegios, de manera que una misma persona no pueda aprobar su propio trabajo.

**Trazabilidad**: Se necesita un sistema que permita rastrear todo el proceso de creación, edición y aprobación de las guías.

## Funcionalidades Deseadas

**Automatización de Guías**: Que el sistema genere las guías docentes en formato PDF y las suba automáticamente al panel de la universidad.

**Edición Controlada**: Los campos estáticos no deben poder editarse por los docentes, solamente por los del departamento de calidad (Tecnico y direccion) pero los campos específicos deben ser editables por los profesores.

**Roles**: Control de permisos según el rol (profesor, director de grado, técnico de calidad, dirección de calidad).

**Trazabilidad**: Registro de cada acción realizada por los usuarios para cumplir con auditorías futuras.

**API de Verificación**: Uso de un sistema de IA para verificar que los cambios realizados por los profesores cumplan con la memoria verificada. 
    - Proceso de memoria: La memoria es un contrato que se audita cada 6 años, asegurando que los contenidos y metodologías estén alineados con las exigencias de la agencia universitaria.



## Requisitos No Funcionales

**Interfaz de Usuario**: Debe ser simple, con pocos clicks, e incluir el estado de las guías (pendiente, enviado, aprobado)

**Alto Rendimiento**: La aplicación debe ser rápida, incluso durante los periodos de alta demanda, como al inicio del semestre.

**Auditoría**: La aplicación debe ser auditable, permitiendo a la dirección de calidad generar informes sobre el estado de las guías.

## Definicion especificade Roles

1. Profesor:
- Permisos de edición: Solo puede modificar: 
    - Nombre del profesor y su email.
    - Contenidos de la asignatura, siempre en concordancia con los descriptores de contenido establecidos en la memoria verificada. No puede modificar los descriptores.
    - Metodologias docentes y actividades formativas
    - Tipos y porcentajes de las actividades de evaluación, que deben alinearse con la memoria verificada. Si los porcentajes no cumplen, no puede hacer cambios hasta que estos se ajusten.
    - Bibliografía y recursos de referencia generales.

- IA para validación: Una inteligencia artificial, conectada mediante API revisará si los contenidos propuestos y los porcentajes de evaluación se ajustan a la memoria verificada. La IA puede emitir un preaprobado, pero la revisión final es realizada por el director de grado.


2. Director de Grado (Académico):

- Responsabilidad: Es el supervisor del profesor y revisa las propuestas de guías docentes que este envía.
- Notificaciones: Recibe una notificación cuando un profesor envía su propuesta de guía docente. Puede aprobar o rechazar las modificaciones.
- Opciones de decisión:
    - Botones de "notificar aceptación" y "notificar solicitud de modificacion", con un cuadro de texto para dar retroalimentación en caso de que sea necesaria una modificacion. El rechazo(solicitud de modificacion) se hace por módulos individuales, lo que permite un control más preciso sobre el contenido.
- Trazabilidad: Cada cambio debe ser registrado, incluyendo cuándo el profesor envía la propuesta, cuándo el director la acepta o rechaza, y cuándo se genera el PDF final para su subida.
- Generación de PDF y repositorio: Una vez aceptada la guía completa, se genera automáticamente un PDF que se almacena en un repositorio. Es posible realizar una subida masiva de PDFs (batch upload).
- Publicación: Es responsable de que las guías estén publicadas a tiempo, lo que es crucial para auditorías y acreditaciones.

3. Técnico de Calidad:

- Permisos completos: Puede editar toda la guía docente, incluido el contenido estático que el profesor no tiene acceso a modificar. Esto es importante ya que el técnico puede hacer cambios a nivel de titulación.
- Rol inicial: El técnico de calidad es el primero en intervenir, asegurándose de que cualquier modificación al contenido estático esté finalizada antes de que el profesor o el director de grado trabajen en la guía.
- Revisión y corrección: Revisa, ajusta o rechaza cambios, y reenvía las propuestas para su revisión posterior.

4. Dirección de Calidad:

- Supervisión: Es el encargado de auditar el trabajo de todos los demás roles. Realiza auditorías aleatorias en las asignaturas para verificar que todo esté en conformidad.
- API de ordenación académica: Tiene acceso a una API que sincroniza con la base de datos de ordenación académica, obteniendo un listado actualizado de asignaciones de profesores por asignatura, esto ultimo no requiere ser un usuario más dentro de la aplicación, ya que esta información se extrae automáticamente para validar que las asignaciones son correctas (profesor - asignatura).

## Casos Especiales

**Asignaturas Multititulación**: Debe ser posible importar contenido de una plantilla preexistente para aquellas asignaturas que se imparten en varias titulaciones.

**Bajas de Profesores**: Si un profesor es dado de baja, no debe aparecer en la maqueta para el nuevo profesor a la hora de editar la maqueta. 

**Conservación de Versiones Anteriores**: El sistema debe ser capaz de mantener versiones anteriores de las guías en PDF para futuras 
referencias.
