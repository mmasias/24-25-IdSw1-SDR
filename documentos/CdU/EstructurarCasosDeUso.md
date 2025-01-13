# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|


## 🎯 **Objetivo**

El objetivo de este paso es **estructurar los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/eCdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

---

# 🛠️ **Diagramas de Casos de Uso**

| **Caso de Uso**                                  | **Actores Involucrados**         | **Diagrama**             |
|--------------------------------------------------|-----------------------------------|--------------------------|
| **Modificación de Datos del Profesorado**        | RRHH, Administrador              | ![Diagrama 1](/images/modelosUML/EstructurarCdU/modificarDatos.svg) |
| **Validación de Datos del Profesorado**          | RRHH, Administrador              | ![Diagrama 2](/images/modelosUML/EstructurarCdU/validarDatos.svg) |
| **Validación de Cumplimiento de Memoria**        | Técnico de Calidad, Administrador, Ordenación | ![Diagrama 3](/images/modelosUML/EstructurarCdU/validarCumplimiento.svg) |
| **Consulta del Claustro Docente**                | RRHH, Administrador, Ordenación, Técnico de Calidad | ![Diagrama 4](/images/modelosUML/EstructurarCdU/consultaClaustro.svg) |
| **Consulta de Asignación Docente**               | Profesor, RRHH, Administrador, Ordenación, Técnico de Calidad | ![Diagrama 5](/images/modelosUML/EstructurarCdU/consultarAsignacion.svg) |
| **Datos Personales y Contrato**                  | Profesor                          | ![Diagrama 6](/images/modelosUML/EstructurarCdU/datosPersonales.svg) |
| **Introducción de Datos Laborales**              | RRHH, Administrador              | ![Diagrama 7](/images/modelosUML/EstructurarCdU/introducirDatos.svg) |
| **Introducción de Datos Académicos**             | Profesor                          | ![Diagrama 8](/images/modelosUML/EstructurarCdU/introAcademicos.svg) |
| **Revisión de Cumplimiento de Carga Docente**    | Ordenación, RRHH, Administrador  | ![Diagrama 9](/images/modelosUML/EstructurarCdU/revisionCumplimiento.svg) |
| **Asignación de Carga Docente**                  | Ordenación, Administrador         | ![Diagrama 10](/images/modelosUML/EstructurarCdU/asignarCarga.svg) |
| **Asignación de Valores de Memoria e Información** | Técnico de Calidad, Administrador | ![Diagrama 11](/images/modelosUML/EstructurarCdU/asignarValores.svg) |
