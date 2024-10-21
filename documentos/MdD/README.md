# 📊 Modelo de Dominio

En esta sección se describen en detalle los tres diagramas principales que componen el modelo de dominio del proyecto: el diagrama de clases, el diagrama de objetos y el diagrama de estados. Para cada diagrama, se muestra una tabla con la representación en formato SVG y un enlace al código fuente en formato `.puml`.

---

## 1. Diagrama de Clases

El diagrama de clases describe la estructura del sistema en términos de entidades principales (como `Profesor`, `Asignatura`, `Titulacion`, etc.) y las relaciones entre ellas. Este diagrama proporciona una visión general de cómo se conectan las diferentes clases en el dominio de la gestión de datos académicos de UNEATLANTICO.

| Diagrama | Código Fuente |
|----------|---------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaClases.svg) | [Ver código](/modelosUML/diagramaClases.puml) |

### Descripción:

...

---

## 2. Diagrama de Objetos

El diagrama de objetos representa instancias específicas de las clases descritas anteriormente, mostrando un escenario concreto del sistema en acción. Este diagrama visualiza cómo los objetos (instancias de las clases) interactúan en un contexto particular, basado en la gestión de asignaturas, profesores y memorias académicas.

| Diagrama | Código Fuente |
|----------|---------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaObjetos.svg) | [Ver código](/modelosUML/diagramaObjetos.puml) |

### Descripción:

...

---

## 3. Diagrama de Estados

El diagrama de estados detalla los diferentes estados por los que pasan las entidades clave del sistema, en este caso `Asignatura` y `Profesor`, a lo largo de su ciclo de vida. Esto es fundamental para gestionar el flujo de trabajo, desde la creación de una asignatura hasta la generación de la memoria académica.

| Diagrama | Código Fuente |
|----------|---------------|
| ![Diagrama de Estados](/images/modelosUML/MdD/diagramaEstados.svg) | [Ver código](/modelosUML/diagramaEstados.puml) |

### Descripción:

...