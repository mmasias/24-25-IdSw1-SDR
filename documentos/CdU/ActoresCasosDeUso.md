# 📝 Encontrar Actores y Casos de Uso

[Priorizar Casos de Uso ➡️](PriorizarCasosDeUso.md) |
|--:|

## 🎯 **Objetivo**

El objetivo de este paso es **encontrar actores y casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.eAyCdU.md#c%C3%B3mo) de la asignatura.

---

## 👥 **Actores**  

| **Actor**              | **Descripción**                                                                                                                             |
|------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| 👩‍🏫 **Profesores**      | Introducen y consultan información personal, académica, y asignaciones docentes.                                                            |
| 🏢 **RRHH**            | Gestionan y validan datos de contratos, cargas docentes y categorías profesionales de los profesores.                                       |
| 📚 **Ordenación**      | Asignan y revisan la carga docente, así como el cumplimiento de valores consignados en las memorias.                                        |
| 📊 **Técnico Calidad** | Gestionan indicadores, asignan valores a sistemas externos y validan compromisos de memoria por titulación.                                 | 
| 🛠️ **Administrador**   | Ha de pertenecer al departamento de calidad y debe poder asumir las funciones de RRHH, Ordenación y Técnico de Calidad según sea necesario. |

---

## 📋 **Casos de Uso y Actores Involucrados**

| Caso de Uso                                                                                                                                     | Profesores | RRHH | Ordenación | Técnico Calidad | Administrador |
|-------------------------------------------------------------------------------------------------------------------------------------------------|------------|------|------------|-----------------|---------------|
| **Inicio de sesion en la plataforma** | ✅    |   ✅   |    ✅    |    ✅    |    ✅    |
| **Introducir** Datos Académicos (experiencia docente, profesional, investigadora, sexenios, acreditaciones, movilidad y titulación profesional) | ✅         |      |            |                 |               |
| **Consultar** valores asignados de Contrato y otros Datos Personales                                                                            | ✅         |      |            |                 |               |
| **Consultar** Asignación Docente (por titulación, curso y semestre)                                                                             | ✅         |      |            |                 |               |
| **Validar** los Datos introducidos por el Profesorado                                                                                           |            | ✅   |            |                 | ✅            |
| **Modificar** los Datos introducidos por el Profesorado                                                                                         |            | ✅   |            |                 | ✅            |
| **Introducir** Datos Laborales (contrato, horas, temporalidad y categoría profesional)                                                          |            | ✅   |            |                 | ✅            |
| **Revisar** listado de Profesores cuya Carga Docente no se ajusta al Contrato                                                                   |            | ✅   | ✅         |                 | ✅           |
| **Consultar** Claustro Docente (listado PDI asociado a una titulación)                                                                          |            | ✅   | ✅         | ✅              | ✅           |
| **Consultar** Asignación Docente por Profesor (créditos y asignaturas)                                                                          |            | ✅   | ✅         | ✅              | ✅           |
| **Asignar** Carga Docente de Asignaturas a Profesores                                                                                           |            |      | ✅         |                 | ✅            |
| **Validar** cumplimiento de valores consignados en la Memoria por Titulación                                                                    |            |      | ✅         |                 | ✅            |
| **Asignar** valores consignados en Memoria por Titulación                                                                                       |            |      |            | ✅              | ✅            |
| **Asignar** valor de Información a SIIU y DGU del PDI                                                                                           |            |      |            | ✅              | ✅            |
| **Validar** cumplimiento de compromisos de Memoria con los valores de la Titulación                                                             |            |      |            | ✅              | ✅            |
| **Obtener** Indicadores para Sistema de Gestión                                                                                                 |            |      |            | ✅              | ✅            |
| **Emitir** Informe del Profesorado (Global o por Titulación)                                                                                    |            |      |            | ✅              | ✅            |