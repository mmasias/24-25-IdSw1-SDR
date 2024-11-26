# Casos de Uso: Priorizar Casos de Uso

### Objetivo

El objetivo de este caso de uso es **priorizar las funcionalidades** del sistema de gestión de asignación de carga docente, enfocándose en la validación del contrato de los profesores, la revisión de su carga de trabajo, y la asignación final de las tareas. 

---

### Actores Involucrados

- **Profesor**: Interactúa con el sistema para recibir su carga de trabajo docente, investigación y gestión.
- **Departamento**: Gestiona las asignaciones de carga de los profesores y verifica su contrato y competencias.
- **Sistema de Planificación**: Sistema que valida y gestiona las asignaciones de carga, asegurando que las cargas sean compatibles con los contratos de los profesores.
- **Memoria Académica**: Almacena la información histórica de las asignaciones de carga docente y verifica el cumplimiento de los requisitos.

---

### Casos de Uso y Priorización

A continuación, se describen los casos de uso priorizados que forman parte del proceso de asignación de carga docente:

#### 1. **Propuesta de Carga Docente** (Alta prioridad)
- **Descripción**: Proponer la carga que tiene cada profesor con la relación que presenta según sus horas de dedicación.
- **Diagrama relacionado**: --
- **Prioridad**: Alta. Este paso es obligatorio para proponer una estimación de la carga que tiene cada docente en relación con su tiempo de dedicación.


#### 2. **Verificación de Contrato y Estado de Carga** (Alta prioridad)
- **Descripción**: Verificar que el contrato del profesor (Parcial, Completo, Obra) sea compatible con la carga asignada.
- **Diagrama relacionado**: Diagrama de Estados (`Verificar Contrato`).
- **Prioridad**: Alta. Este paso es obligatorio para garantizar que la asignación cumpla con los requisitos legales y contractuales.

#### 3. **Revisión del Equilibrio de Carga de Trabajo (EQ TC)** (Alta prioridad)
- **Descripción**: Asegurarse de que la carga de trabajo del profesor esté equilibrada entre docencia, investigación y gestión, y que no exceda los límites establecidos en el contrato.
- **Diagrama relacionado**: Diagrama de Estados (`Revisión EQ TC`).
- **Prioridad**: Alta. Es crucial para evitar sobrecargar a los profesores y asegurar el cumplimiento de las condiciones laborales.

#### 4. **Ajuste de Carga Docente** (Media prioridad)
- **Descripción**: Generar y ajustar la propuesta inicial de carga docente, asegurando que las proporciones entre docencia, investigación y gestión sean apropiadas.
- **Diagrama relacionado**: Diagrama de Estados (`Propuesta Carga` y `Ajuste Carga`).
- **Prioridad**: Media. Aunque importante, este paso es flexible y puede adaptarse dependiendo de las condiciones del contrato y la carga existente.

#### 5. **Generación de Memoria Académica** (Media prioridad)
- **Descripción**: Crear y almacenar la memoria académica que refleje las asignaciones de carga y el año académico correspondiente.
- **Diagrama relacionado**: Diagrama de Objetos (`Memoria Académica`).
- **Prioridad**: Media. No es urgente, pero es necesario para mantener un registro adecuado de las asignaciones.

#### 6. **Asignación Final de Carga Docente** (Alta prioridad)
- **Descripción**: Asignar la carga final al profesor una vez que la verificación del contrato y la revisión de carga han sido completadas exitosamente.
- **Diagrama relacionado**: Diagrama de Estados (`Asignada`).
- **Prioridad**: Alta. Este paso finaliza el proceso de asignación y asegura que todo esté registrado correctamente.

---

### Diagrama de Contexto

Los siguientes diagramas ilustran las interacciones entre los actores y los casos de uso priorizados:

| **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![Departamento](/images/modelosUML/CdU/departamento.svg) | [Ver código](/modelosUML/CdU/Departamento.puml) |

| **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![Profesor](/images/modelosUML/CdU/profesor.svg) | [Ver código](/modelosUML/CdU/Profesor.puml) |

| **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![Memoria Académica](/images/modelosUML/CdU/memoriaAcademica.svg) | [Ver código](/modelosUML/CdU/MemoriaAcademica.puml) |

 **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![Sistemas](/images/modelosUML/CdU/Sistema.svg) | [Ver código](/modelosUML/CdU/Sistema.puml) |


