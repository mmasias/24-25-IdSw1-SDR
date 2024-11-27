# 📝 Encontrar Actores y Casos de Uso

[Priorizar Casos de Uso ➡️](PriorizarCasosDeUso.md) |
|--:|

## 🎯 **Objetivo**

El objetivo de este paso es **encontrar actores y casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.eAyCdU.md#c%C3%B3mo) de la asignatura.

---

## 👥 **Actores**  

| **Actor**                       | **Descripción**                                                                                            |  
|---------------------------------|------------------------------------------------------------------------------------------------------------|  
| 👨‍🏫 **Profesor**                 | Responsable de consultar, ajustar y validar su carga docente en función de las asignaciones del sistema.   |  
| 🏢 **Departamento**             | Supervisa las asignaciones y asegura el cumplimiento de normativas y distribución equitativa de cargas.    |  
| 💻 **Sistema de Planificación** | Gestiona la asignación, validación y automatización de la carga docente y otros procesos académicos clave. |  
| 📚 **Memoria Académica**        | Encargada de almacenar y generar informes basados en los datos históricos y asignaciones docentes.         |  

---

## 📋 **Casos de Uso y Actores Involucrados**

| **Caso de Uso**                                           | **Actor(es)**                                           |
|-----------------------------------------------------------|---------------------------------------------------------|
| 🛠️ **Ajuste de Carga Docente**                            | [👨‍🏫], [💻]                                              |
| 📊 **Propuesta de Carga Docente**                         | [👨‍🏫], [🏢]                                              |
| 📑 **Generación de Memoria Académica**                    | [👨‍🏫], [📚]                                              |
| ⚖️ **Revisión del Equilibrio de Carga de Trabajo (EQ TC)**| [👨‍🏫], [🏢]                                              |
| ✔️ **Asignación Final de Carga Docente**                  | [👨‍🏫], [🏢]                                              |
| 📜 **Verificación de Contrato y Estado de Carga**         | [💻]                                                     |



---

| **Modelo** | **Código** |
|--------------|--------------------|
| ![Modelo](/images/modelosUML/CdU/EncontrarCasos.svg) | [Ver código](/modelosUML/CdU/encontrarCasos.puml) |
