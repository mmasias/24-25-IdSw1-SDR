# 📝 Priorizar Casos de Uso

| [⬅️ Encontrar Actores y Casos de Uso](ActoresCasosDeUso.md) | [Detallar Casos de Uso ➡️](DetallarCasosDeUso.md) |
|:--|--:|

## 🎯 **Objetivo**

El objetivo de este paso es **priorizar las funcionalidades** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.PCdU.md#c%C3%B3mo) de la asignatura.
El orden ha sido establecido por el cliente según la importancia y necesidad de cada caso de uso. La priorización del desarrollo se ha realizado en base a la [gestión integral del ciclo de vida del producto](/documentos/glosario.md#gestión-integral-del-ciclo-de-vida-del-producto).

---

## 📋 **Casos de Uso y Priorización**


| **#** | **Caso de Uso**                                                                                             | **Prioridad** |  
|-------|-------------------------------------------------------------------------------------------------------------|---------------|  
| 1 | **Introducir** datos de contrato, horas, temporalidad y categoría profesional                                   |    🔴 Alta    |
| 2 | **Asignar** carga docente de asignaturas a profesores                                                           |    🔴 Alta    |
| 3 | **Revisar** listado de profesores cuya carga docente no se ajusta al contrato                                   |    🔴 Alta    |
| 4 | **Validar** los valores de titulación vs. compromisos de memoria                                                |    🔴 Alta    |
| 5 | **Emitir** informe del profesorado por titulación y global                                                      |    🔴 Alta    |
| 6 | **Consultar** asignaciones docentes (por titulación, curso y semestre)                                          |    🟠 Media   |
| 7 | **Asignar** valores consignados en memoria por titulación                                                       |    🟠 Media   |
| 8 | **Obtener** indicadores para Sistema de Gestión                                                                 |    🟠 Media   |
| 9 | **Validar** datos introducidos por el profesorado y modificarlos                                                |    🟠 Media   |
| 10 | **Introducir** datos de experiencia docente, profesional, investigadora, etc.                                  |    🟢 Baja    |
| 11 | **Revisar** cumplimiento de valores consignados en la memoria por titulación                                   |    🟢 Baja    |
| 12 | **Asignar** valor de información a SIIU y DGU del PDI                                                          |    🟢 Baja    |
| 13 | **Consultar** valores asignados de contrato y otros datos personales                                           |    🟢 Baja    |
| 14 | **Consultar** claustro docente (listado PDI asociado a una titulación), anual en la titulación, por semestre.. |    🟢 Baja    |
| 15 | **Consultar** asignación docente por profesor (créditos y asignaturas)                                         |    🟢 Baja    |

### 🪧 Descripción de la Priorización

#### 🔴 **Alta prioridad**
- Los casos de uso asignados como alta prioridad (1-5) son fundamentales para garantizar el funcionamiento esencial del sistema. Incluyen funciones críticas como la gestión de contratos, la asignación de cargas docentes, la revisión de inconsistencias y la emisión de informes, que son esenciales para la operatividad y supervisión del sistema.

#### 🟡 **Media prioridad**
- Los casos en esta categoría (6-9) se centran en tareas relevantes pero no imprescindibles para el funcionamiento inicial del sistema. Incluyen consultas, obtención de indicadores y validación de datos, que tienen un impacto directo en la calidad y eficiencia del sistema, pero cuya ausencia no detendría su operatividad básica.

#### 🟢 Baja prioridad
- Los casos de uso asignados como baja prioridad (10-15) están más relacionados con tareas complementarias o específicas, como consultas adicionales, introducción de datos personales y asignación de valores externos. Son funcionalidades que agregan valor al sistema, pero no son críticas para su funcionamiento inicial o para cumplir con las necesidades más urgentes.