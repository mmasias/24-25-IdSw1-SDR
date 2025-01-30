<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Priorización_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Priorizacion.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |

</div>

</div>

# Sesión de requisitado #2
Fecha: 13 de noviembre, 2024

# Información General
**Cliente**: Parte del departamento de calidad. Jorge Crespo Alvarez.

**Proyecto**: Automatización de la actualización del contenido de las guías docentes.

**Problema principal**: Parte del contenido de las guías docentes debe actualizarse anualmente, y en el caso de asignaturas impartidas en varias titulaciones, el contenido puede variar, lo que hace ineficiente el uso del copiar y pegar, ya que son demasiadas guias docentes y el proceso manual se torna engorroso. 

# Introducción
En la primera parte de la reunión hubó un repaso del modelo del dominio y el problema que se quiere solucionar, un repaso de la primera sesión.

# Aclaración de dudas

### ¿El director de grado tiene la capacidad de editar el mismo contenido que el profesor para agilizar el proceso?

No, ya que, aunque sea el director de grado, esto no implica que sea experto en la materia o asignatura asignada al profesor. Por ello, únicamente el profesor debería tener la capacidad de editar el contenido de la asignatura. Sin embargo, la modificación en el apartado de porcentajes en una guia docente sí podría ser posible como un extra ya que hay ciertas reglas establecidas que se deben cumplir.  Dicho esto, sería como una funcionalidad extra y no para la primera entrega.

### ¿Supervisar sería un estado?
A nivel de caso de uso no debería de ser un estado por lo cual deberíamos de quitarlo de nuestros casos de uso

### ¿El técnico de calidad puede editar la guía docente?
Sí, puede editar la plantilla pero no el contenido.

### Dudas Pendientes
- ¿A partir de donde podemos agregar las compuertas lógicas?


# Avances en el modelo de dominio

Se le mostró al cliente los avances en los cual nos mencionó que hay que generar una plantilla. Una plantilla es el esqueleto donde se meterá el contenido.  Habrá contenido estático que depende del profesor y también existe el contenido dinámico que depende de la titulación.

## Diagrama de Clases y Objetos
- Se aclaró la jerarquía apuntando a la guía como el documento final, el producto final.
- Hay dos guías docentes, la versión digital y versión física por lo cual se tendrá que adaptar el diagrama de clases

## Diagrama de Estados
- Faltan decisiones lógicas en los diagramas de estados pero falta la aclaración de Masias para saber a partir de cuando se puede agregar las compuertas lógicas o si simplemente deberíamos agregar estados como aceptado o rechazado.

## Revisión de Actores y Casos de Uso
- Se aclaró que la parte de supervisar que hace el técnico de calidad no debería de ser un caso de uso
- "Publicar guía docente" debería de ser un caso de uso
- No puedes supervisar algo que estas haciendo tu, lo tiene que supervisar alguien más.  Si el director de grado esta enseñando una materia y debe de crear su guía docente, no puede hacer el proceso de revisión el mismo.
- El tecnico de calidad puede ver el listado de los estados de las guias docentes


# Resumen por partes de la reunión


**Proceso de Revisión y Auditoría**

- Se explica que el objetivo principal es que el contenido de las guías sea revisado por el profesor, no por el director de grado.

- Se menciona la necesidad de un proceso de auditoría doble, con el director de calidad y el director de grado revisando el contenido.

- Se detalla que el director de calidad auditará la plantilla y el contenido dinámico proporcionado por el profesor.

- Se discute la relación entre la guía docente y la plantilla, y cómo ambos elementos interactúan con el director de grado y el director de calidad.

**Plantilla y Contenido Dinámico**
- Se describe la plantilla como una maqueta que contiene contenido estático y dinámico.

- Se menciona que el contenido dinámico depende del profesor, mientras que el contenido estático depende de la titulación.

- Se explica que la responsabilidad de la plantilla es del director de calidad, mientras que el contenido dinámico es responsabilidad del profesor.

- Se discute la importancia de que la plantilla sea coherente y que el contenido dinámico sea revisado por el profesor.

**Flujo de Trabajo y Casos de Uso**
- Se discute el flujo de trabajo y los casos de uso para la gestión de guías docentes.

- Se menciona la necesidad de un diagrama de flujo que muestre el proceso de revisión y aprobación de guías.

- Se sugiere que el director de calidad debe verificar que la plantilla y el contenido dinámico sean correctos.

- Se discute la posibilidad de que el director de grado rechace o acepte la guía, y cómo esto afecta el proceso de publicación.

**Supervisión y Notificaciones**
- Se discute la supervisión de guías docentes y la importancia de notificar al profesor sobre qué parte de la guía debe revisar.

- Se menciona la posibilidad de que el director de calidad envíe notificaciones al profesor sobre qué apartados de la guía deben ser revisados.

- Se sugiere que el director de grado podría revisar la guía y enviar notificaciones al profesor sobre posibles correcciones.

- Se discute la importancia de que el profesor tenga instrucciones claras sobre qué revisar en la guía.


**Publicación y Distribución de Guías**
- Se discuten el proceso de publicación y distribución de guías docentes.

- Se menciona que la guía debe ser revisada y aprobada antes de ser publicada.

- Se sugiere que el director de calidad debe verificar que la guía sea correcta antes de que el director de grado la publique.

- Se discute la importancia de que la guía sea distribuida correctamente a los estudiantes y profesores.
