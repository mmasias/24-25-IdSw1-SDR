# 📝 Detallar Casos de Uso

---

### 🎯 **Objetivo**
El objetivo es **detallar los actores y casos de uso**

---

### 👥 **Actores Involucrados**  

| **Actor**                          | **Descripción**                                                                                                                                  |  
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|  
| 👨‍🏫 **Profesor**                   | El profesor es quien recibe la carga docente y debe interactuar con el sistema para revisar su carga de trabajo, asegurarse de que está equilibrada y recibir la asignación final de carga.                                                                 |  
| 🏢 **Departamento**                 | El departamento gestiona las cargas docentes y verifica que se cumplan los requisitos de distribución de trabajo entre los profesores. Son responsables de revisar la propuesta de carga y asegurarse de que sea equitativa y cumpla con las normativas internas. |  
| 💻 **Sistema de Planificación**     | El sistema es la plataforma que gestiona la propuesta, verificación y asignación de la carga docente. Es clave para automatizar y facilitar la distribución y la revisión de cargas de trabajo.                                  |  
| 📚 **Memoria Académica**            | La memoria académica es el registro de las asignaciones y actividades académicas de los profesores. Se utiliza para generar informes y realizar seguimientos del trabajo realizado por los docentes.                                          |  

---

### 📋 **Casos de Uso y Priorización**  

| **#** | **Caso de Uso**                                         | **Prioridad** | **Descripción**                                                                                                                                               |  
|-------|---------------------------------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| 1     | 📊 **Propuesta de Carga Docente**                       | 🔴 **Alta**   | El sistema presenta la propuesta de carga docente a los profesores y al departamento para su revisión. Los profesores pueden consultar la carga inicial antes de su asignación final.                        |  
| 2     | 📜 **Verificación de Contrato y Estado de Carga**       | 🔴 **Alta**   | Este proceso permite verificar el contrato del profesor y su estado actual de carga docente, asegurando que no se exceda el número de horas estipulado o se incumplan los acuerdos contractuales.               |  
| 3     | ⚖️ **Revisión del Equilibrio de Carga de Trabajo (EQ TC)** | 🔴 **Alta**   | Los departamentos revisan si la distribución de carga entre los docentes está equilibrada, considerando tanto la cantidad de horas como la intensidad de trabajo. Es crucial para evitar cargas excesivas. |  
| 4     | 🛠️ **Ajuste de Carga Docente**                          | 🟡 **Media**  | Si se detectan desequilibrios o problemas en la distribución de las cargas, el sistema permite ajustar la asignación de horas de los profesores para mantener la equidad.                                         |  
| 5     | 📑 **Generación de Memoria Académica**                  | 🟡 **Media**  | Genera el informe o memoria académica que resume la carga docente final y las actividades realizadas por los profesores. Este documento es utilizado para seguimiento y auditorías.                                 |  
| 6     | ✔️ **Asignación Final de Carga Docente**                | 🔴 **Alta**   | Una vez revisada y ajustada la carga docente, el sistema realiza la asignación final, confirmando la carga que cada profesor debe asumir durante el periodo académico correspondiente.  
