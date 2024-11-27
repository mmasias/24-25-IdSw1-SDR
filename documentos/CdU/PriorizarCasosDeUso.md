# 📝 **Casos de Uso: Priorizar Casos de Uso**

### 🎯 **Objetivo**
El objetivo de este caso de uso es **priorizar las funcionalidades** del sistema de gestión de asignación de carga docente, enfocándose en la validación del contrato de los profesores, la revisión de su carga de trabajo y la asignación final de las tareas.

---

### 👥 **Actores Involucrados**

| **Actor**               | **Descripción**                                                                 |
|-------------------------|---------------------------------------------------------------------------------|
| 👨‍🏫 **Profesor**        | Interactúa con el sistema para recibir su carga de trabajo docente, investigación y gestión. |
| 🏢 **Departamento**      | Gestiona las asignaciones de carga de los profesores y verifica su contrato y competencias. |
| 💻 **Sistema de Planificación** | Sistema que valida y gestiona las asignaciones de carga, asegurando que las cargas sean compatibles con los contratos de los profesores. |
| 📚 **Memoria Académica** | Almacena la información histórica de las asignaciones de carga docente y verifica el cumplimiento de los requisitos. |

---

### 📋 **Casos de Uso y Priorización**

| **#** | **Caso de Uso**                                          | **Descripción**                                                                                              | **Prioridad** |  
|-------|----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|---------------|
| 1     | 📊 **Propuesta de Carga Docente**                        | Proponer la carga que tiene cada profesor con la relación que presenta según sus horas de dedicación.         | 🔴 **Alta**      |
| 2     | 📜 **Verificación de Contrato y Estado de Carga**        | Verificar que el contrato del profesor (Parcial, Completo, Obra) sea compatible con la carga asignada.         | 🔴 **Alta**      |
| 3     | ⚖️ **Revisión del Equilibrio de Carga de Trabajo (EQ TC)** | Asegurarse de que la carga de trabajo del profesor esté equilibrada entre docencia, investigación y gestión.    | 🔴 **Alta**      |
| 4     | 🛠️ **Ajuste de Carga Docente**                           | Generar y ajustar la propuesta inicial de carga docente, asegurando que las proporciones entre docencia, investigación y gestión sean apropiadas. | 🟡 **Media**     |
| 5     | 📑 **Generación de Memoria Académica**                   | Crear y almacenar la memoria académica que refleje las asignaciones de carga y el año académico correspondiente. | 🟡 **Media**     |
| 6     | ✔️ **Asignación Final de Carga Docente**                 | Asignar la carga final al profesor una vez que la verificación del contrato y la revisión de carga han sido completadas exitosamente. | 🔴 **Alta**      |

---

### 🗺️ **Diagrama de Contexto**

A continuación, se muestran los diagramas que ilustran las interacciones entre los actores y los casos de uso priorizados:

| **Diagrama**           | **Código Fuente**                      |
|------------------------|----------------------------------------|
| ![Departamento](/images/modelosUML/CdU/departamento.svg) | [Ver código](/modelosUML/CdU/Departamento.puml) |
| ![Profesor](/images/modelosUML/CdU/profesor.svg)        | [Ver código](/modelosUML/CdU/Profesor.puml) |
| ![Memoria Académica](/images/modelosUML/CdU/memoriaAcademica.svg) | [Ver código](/modelosUML/CdU/MemoriaAcademica.puml) |
| ![Sistemas](/images/modelosUML/CdU/Sistema.svg)         | [Ver código](/modelosUML/CdU/Sistema.puml) |

---

### 🎨 **Resumen Visual**

Este es el resumen visual con los emoticonos integrados para hacerlo más atractivo y facilitar la comprensión de cada etapa del proceso de asignación de carga docente. ¡Espero que te guste este formato más bonito y visual!

