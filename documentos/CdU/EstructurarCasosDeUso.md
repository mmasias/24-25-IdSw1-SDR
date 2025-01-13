# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|

## 🎯 **Objetivo**

El objetivo de este paso es **estructurar el modelo de los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/eCdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

## 1️⃣ Primer Paso

![Paso 1](/images/modelosUML/CdU/EstructurarCasosDeUso/Paso1.svg)

## 2️⃣ Segundo Paso

![Paso 2](/images/modelosUML/CdU/EstructurarCasosDeUso/Paso2.svg)

## 🛠️ **Diagramas de Casos de Uso**

| **Caso de Uso**                                  | **Actores Involucrados**         | **Diagrama**             |
|--------------------------------------------------|-----------------------------------|--------------------------|
| **Modificación de Datos del Profesorado**        | RRHH, Administrador              | ![Diagrama 1](/images/modelosUML/CdU/EstructurarCasosDeUso/modificarDatos.svg) |
| **Validación de Datos del Profesorado**          | RRHH, Administrador              | ![Diagrama 2](/images/modelosUML/CdU/EstructurarCasosDeUso/validarDatos.svg) |
| **Validación de Cumplimiento de Memoria**        | Técnico de Calidad, Administrador, Ordenación | ![Diagrama 3](/images/modelosUML/CdU/EstructurarCasosDeUso/validarCumplimiento.svg) |
| **Consulta del Claustro Docente**                | RRHH, Administrador, Ordenación, Técnico de Calidad | ![Diagrama 4](/images/modelosUML/CdU/EstructurarCasosDeUso/consultaClaustro.svg) |
| **Consulta de Asignación Docente**               | Profesor, RRHH, Administrador, Ordenación, Técnico de Calidad | ![Diagrama 5](/images/modelosUML/CdU/EstructurarCasosDeUso/consultarAsignacion.svg) |
| **Datos Personales y Contrato**                  | Profesor                          | ![Diagrama 6](/images/modelosUML/CdU/EstructurarCasosDeUso/datosPersonales.svg) |
| **Introducción de Datos Laborales**              | RRHH, Administrador              | ![Diagrama 7](/images/modelosUML/CdU/EstructurarCasosDeUso/introducirDatos.svg) |
| **Introducción de Datos Académicos**             | Profesor                          | ![Diagrama 8](/images/modelosUML/CdU/EstructurarCasosDeUso/introAcademicos.svg) |
| **Revisión de Cumplimiento de Carga Docente**    | Ordenación, RRHH, Administrador  | ![Diagrama 9](/images/modelosUML/CdU/EstructurarCasosDeUso/revisionCumplimiento.svg) |
| **Asignación de Carga Docente**                  | Ordenación, Administrador         | ![Diagrama 10](/images/modelosUML/CdU/EstructurarCasosDeUso/asignarCarga.svg) |
| **Asignación de Valores de Memoria e Información** | Técnico de Calidad, Administrador | ![Diagrama 11](/images/modelosUML/CdU/EstructurarCasosDeUso/asignarValores.svg) |
