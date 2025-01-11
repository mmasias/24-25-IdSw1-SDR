# 📝 Prototipar Casos de Uso

| [⬅️ Detallar Casos de Uso](DetallarCasosDeUso.md) | [Estructurar el Modelo de Casos de Uso ➡️](EstructurarCasosDeUso.md) |
|:--|--:|

## 🎯 **Objetivo**
El objetivo de este paso es **prototipar los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.ICdU.md) de la asignatura.

---

### Vista General por Actores

Debido a que este proyecto tiene direfentes actores, en primer lugar se mostrara las pantallas de inicio correspondientes a cada actor, lo que reflejará las acciones que puede hacer cada uno de ellos.

| **Actor**                | **Prototipo**                                      |
|--------------------------|----------------------------------------------------|
| Inicio de Sesión         | ![InicioSesion](/images/modelosUML/MockUp/Inicio.png) |
| Admin                    | ![UsuarioAdmin](/images/modelosUML/MockUp/Admin.png)  |
| Recursos Humanos         | ![UsuarioRRHH](/images/modelosUML/MockUp/RRHH.png)    |
| Profesor                 | ![UsuarioProfesor](/images/modelosUML/MockUp/Profesor.png) |
| Técnico de Calidad       | ![UsuarioCalidad](/images/modelosUML/MockUp/Calidad.png)  |
| Ordenación Académica     | ![UsuarioOrdenacion](/images/modelosUML/MockUp/Ordenacion.png) |

---

### Casos de Uso

A continuación se presentan los casos de uso prototipados.

| **#** | **Caso de Uso**                                      | **Prototipo** |  
|-------|------------------------------------------------------|---------------|
| 1 | **Introducir** Datos Laborales (contrato, horas, temporalidad y categoría profesional)             | ![IntroducirDatos](/images/Prototipar/DatosLaborales.png)      |
| 2 | **Asignar** Carga Docente de Asignaturas a Profesores                                              | ![AsignacionAsignaturasProfesor](/images/Prototipar/AsignacióndeCargaDocente.png)      |
| 3 | **Revisar** listado de Profesores cuya Carga Docente no se ajusta al Contrato                      | ![RevisarCargaProfesoresNoAjustada](/images/Prototipar/RevisionCargaDocente.png)      |
| 4 | **Validar** cumplimiento de compromisos de Memoria con los valores de la Titulación                |       |
| 5 | **Emitir** Informe del Profesorado (Global o por Titulación)                                       |   ![Emitir Informe]()    |
| 6 | **Consultar** Asignación Docente (por titulación, curso y semestre)                                |   ![ConsultarAsignacionDocente]()    |
| 7 | **Asignar** valores consignados en Memoria por Titulación                                          |       |
| 8 | **Obtener** Indicadores para Sistema de Gestión                                                    |  ![Obtener indicadores](/)     |
| 9 | **Modificar** los Datos introducidos por el Profesorado                                            |![ModificarDatosProfesorado]()       |
| 10 | **Validar** los Datos introducidos por el Profesorado                                             | ![ValidarDatosProfesorado]()      |
| 11 | **Introducir** Datos Académicos (experiencia docente, profesional, investigadora, sexenios, acreditaciones, movilidad y titulación profesional) |   ![DatosAcademicos](/images/Prototipar/DatosAcademicos.png)     |
| 12 | **Validar** cumplimiento de valores consignados en la Memoria por Titulación                      |        |
| 13 | **Asignar** valor de Información a SIIU y DGU del PDI                                             |        |
| 14 | **Consultar** valores asignados de Contrato y otros Datos Personales                              | ![ConsultarDatosyContrato]()       |
| 15 | **Consultar** Claustro Docente (listado PDI asociado a una titulación)                            |        |
| 16 | **Consultar** Asignación Docente por Profesor (créditos y asignaturas)                            |   ![ConsultaAsignacionDocenteProfesor](/images/Prototipar/ConsultaAsignaciónDocenteProfesor.png)     |
