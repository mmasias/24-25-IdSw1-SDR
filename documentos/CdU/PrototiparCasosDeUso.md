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
| 1 | Inicio de sesión en la plataforma                                                                  | ![InicioSesion](/images/Prototipar/InicioSesion.svg) |  
| 2 | **Introducir** Datos Laborales (contrato, horas, temporalidad y categoría profesional)             | ![IntroducirDatos](/images/Prototipar/PrototiparIntroducirDatos.svg)      |
| 3 | **Asignar** Carga Docente de Asignaturas a Profesores                                              | ![AsignacionAsignaturasProfesor](/images/Prototipar/PrototiparAsignacionAsignaturasProfesor.svg)      |
| 4 | **Revisar** listado de Profesores cuya Carga Docente no se ajusta al Contrato                      | ![RevisarCargaProfesoresNoAjustada](/images/Prototipar/PrototiparRevisarProfesoresCargaNoAjustada.svg)      |
| 5 | **Validar** cumplimiento de compromisos de Memoria con los valores de la Titulación                |       |
| 6 | **Emitir** Informe del Profesorado (Global o por Titulación)                                       |   ![Emitir Informe](/images/Prototipar/PrototiparEmitirInformeProfesorado.svg)    |
| 7 | **Consultar** Asignación Docente (por titulación, curso y semestre)                                |   ![ConsultarAsignacionDocente](/images/Prototipar/PrototiparConsultarAsignacionDocente.svg)    |
| 8 | **Asignar** valores consignados en Memoria por Titulación                                          |       |
| 9 | **Obtener** Indicadores para Sistema de Gestión                                                    |  ![Obtener indicadores](/images/Prototipar/PrototiparObtenerIndicadores.svg)     |
| 10 | **Modificar** los Datos introducidos por el Profesorado                                            |![ModificarDatosProfesorado](/images/Prototipar/PrototiparModificarDatosProfesorado.svg)       |
| 11 | **Validar** los Datos introducidos por el Profesorado                                             | ![ValidarDatosProfesorado](/images/Prototipar/PrototiparValidarDatosProfesorado.svg)      |
| 12 | **Introducir** Datos Académicos (experiencia docente, profesional, investigadora, sexenios, acreditaciones, movilidad y titulación profesional) |        |
| 13 | **Validar** cumplimiento de valores consignados en la Memoria por Titulación                      |        |
| 14 | **Asignar** valor de Información a SIIU y DGU del PDI                                             |        |
| 15 | **Consultar** valores asignados de Contrato y otros Datos Personales                              | ![ConsultarDatosyContrato](/images/Prototipar/PrototiparConsultarDatosYContrato.svg)       |
| 16 | **Consultar** Claustro Docente (listado PDI asociado a una titulación)                            |        |
| 17 | **Consultar** Asignación Docente por Profesor (créditos y asignaturas)                            |        |
