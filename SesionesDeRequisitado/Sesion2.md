# Sesión de requisitado #2
Fecha: 13 de noviembre, 2024

# Información General
**Cliente**: Parte del departamento de calidad. Jorge Crespo Alvarez.

**Proyecto**: Automatización de la actualización del contenido de las guías docentes.

**Problema principal**: Parte del contenido de las guías docentes debe actualizarse anualmente, y en el caso de asignaturas impartidas en varias titulaciones, el contenido puede variar, lo que hace ineficiente el uso del copiar y pegar, ya que son demasiadas guias docentes y el proceso manual se torna engorroso. 

## Introducción
En la primera parte de la reunión hubó un repaso del modelo del dominio y el problema que se quiere solucionar, un repaso de la primera sesión.

# Aclaración de dudas

### ¿El director de grado tiene la capacidad de editar el mismo contenido que el profesor para agilizar el proceso?

No, ya que, aunque sea el director de grado, esto no implica que sea experto en la materia o asignatura asignada al profesor. Por ello, únicamente el profesor debería tener la capacidad de editar el contenido de la asignatura. Sin embargo, la modificación en el apartado de porcentajes en una guia docente sí podría ser posible como un extra ya que hay ciertas reglas establecidas que se deben cumplir.  Dicho esto, sería como una funcionalidad extra y no para la primera entrega.

### ¿Supervisar sería un estado?
A nivel de caso de uso no debería de ser un estado por lo cual deberíamos de quitarlo de nuestros casos de uso

### ¿El técnico de calidad puede editar la guía docente?
Sí, puede editar la plantilla pero no el contenido.

## Dudas Pendientes
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

