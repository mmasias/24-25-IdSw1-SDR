# 📝 Encontrar Actores y Casos de Uso

[Priorizar Casos de Uso ➡️](PriorizarCasosDeUso.md) |
|--:|

## 🎯 **Objetivo**

El objetivo de este paso es **encontrar actores y casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.eAyCdU.md#c%C3%B3mo) de la asignatura.

---

## 👥 **Actores**  

| **Actor**           | **Descripción**                                                                                           |
|---------------------|-----------------------------------------------------------------------------------------------------------|
| 👩‍🏫 **Profesores**   | Introducen y consultan información personal, académica, y asignaciones docentes.                          |
| 🏢 **RRHH**          | Gestionan y validan datos de contratos, cargas docentes y categorías profesionales de los profesores.      |
| 📚 **Ordenación**    | Asignan y revisan la carga docente, así como el cumplimiento de valores consignados en las memorias.       |
| 📊 **Técnico Calidad** | Gestionan indicadores, asignan valores a sistemas externos y validan compromisos de memoria por titulación.|
| 🛠️ **Administrador** | Puede asumir las funciones de RRHH, Ordenación y Técnico de Calidad según sea necesario.                   |

---

## 📋 **Casos de Uso y Actores Involucrados**

| Caso de Uso                                                                                                | Profesores | RRHH | Ordenación | Técnico Calidad | Administrador |
|------------------------------------------------------------------------------------------------------------|------------|------|------------|-----------------|---------------|
| Introducir datos de experiencia docente, profesional, investigadora, etc.                                  | ✅         |      |            |                 |               |
| Consultar valores asignados de contrato y otros datos personales                                           | ✅         |      |            |                 |               |
| Consultar asignaciones docentes (por titulación, curso y semestre)                                         | ✅         |      |            |                 |               |
| Validar datos introducidos por el profesorado y modificarlos                                               |            | ✅   |            |                 | ✅            |
| Introducir datos de contrato, horas, temporalidad y categoría profesional                                  |            | ✅   |            |                 | ✅            |
| Revisar listado de profesores cuya carga docente no se ajusta al contrato                                  |            | ✅   | ✅         |                 | ✅            |
| Consultar claustro docente (listado PDI asociado a una titulación), anual en la titulación, por semestre.. |            | ✅   | ✅         | ✅             | ✅            |
| Consultar asignación docente por profesor (créditos y asignaturas)                                         |            | ✅   | ✅         | ✅             | ✅            |
| Asignar carga docente de asignaturas a profesores                                                          |            |      | ✅         |                 | ✅            |
| Revisar cumplimiento de valores consignados en MEMORIA por titulación                                      |            |      | ✅         |                 | ✅            |
| Asignar valores consignados en memoria por titulación                                                      |            |      |            | ✅              | ✅            |
| Asignar valor de información a SIIU y DGU del PDI                                                          |            |      |            | ✅              | ✅            |
| Validar los valores de titulación vs. compromisos de memoria                                               |            |      |            | ✅              | ✅            |
| Obtener indicadores para Sistema de Gestión                                                                |            |      |            | ✅              | ✅            |
| Emitir informe del profesorado por titulación y global                                                     |            |      |            | ✅              | ✅            |

---

| **Modelo**        | **Código**                 |
|--------------------|----------------------------|
| ![Profesor](/images/modelosUML/CdU/Profesor.svg) | [Ver código](/modelosUML/CdU/Profesor.puml) |
| ![Ordenación](/images/modelosUML/CdU/Ordenacion.svg) | [Ver código](/modelosUML/CdU/Ordenacion.puml) |
| ![RRHH](/images/modelosUML/CdU/RRHH.svg)         | [Ver código](/modelosUML/CdU/RRHH.puml) |
| ![Técnico Calidad](/images/modelosUML/CdU/TecnicoCalidad.svg) | [Ver código](/modelosUML/CdU/TecnicoCalidad.puml) |
| ![Administrador](/images/modelosUML/CdU/Admin.svg) | [Ver código](/modelosUML/CdU/Admin.puml) |
