# 📝 Encontrar Actores y Casos de Uso

[Priorizar Casos de Uso ➡️](PriorizarCasosDeUso.md) |
|--:|

## 🎯 **Objetivo**

El objetivo de este paso es **encontrar actores y casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.eAyCdU.md#c%C3%B3mo) de la asignatura.

## 👥 **Actores**  

![DiagramaDeActores](/images/modelosUML/CdU/Individuales/Actores.svg) 

 
 

## 📋 **Casos de Uso y Actores Involucrados**

| Caso de Uso                                  | Profesores | RRHH | Ordenación | Técnico Calidad | Administrador | Enlaces |
|----------------------------------------------|------------|------|------------|-----------------|---------------|
| **Iniciar Sesión**                           | ✅         | ✅  | ✅         | ✅              | ✅           | [📝](DetallarCasosDeUso.md#inicio-de-sesión)|
| **Introducir** Datos Académicos              | ✅         |      |            |                 |               | 📝|
| **Consultar** Datos Personales               | ✅         |      |            |                 |               | 📝|
| **Consultar** Asignación Docente             | ✅         |      |            |                 |               | 📝|
| **Validar** Datos del Profesorado            |            | ✅   |            |                 | ✅            | 📝|
| **Modificar** Datos del Profesorado          |            | ✅   |            |                 | ✅            | 📝|
| **Introducir** Datos Laborales               |            | ✅   |            |                 | ✅            | 📝|
| **Revisar** Profesores con Carga no ajustada |            | ✅   | ✅         |                 | ✅           | 📝|
| **Consultar** Claustro Docente               |            | ✅   | ✅         | ✅              | ✅           | 📝|
| **Consultar** Asignación por Profesor        |            | ✅   | ✅         | ✅              | ✅           | 📝|
| **Validar** Cumplimiento de Memoria          |            |      | ✅         | ✅              | ✅           | 📝|
| **Asignar** Carga Docente                    |            |      | ✅         |                 | ✅            | 📝|
| **Asignar** Valores en Memoria               |            |      |            | ✅              | ✅            | 📝|
| **Asignar** Información SIIU/DGU             |            |      |            | ✅              | ✅            | 📝|
| **Obtener** Indicadores                      |            |      |            | ✅              | ✅            | 📝|
| **Emitir** Informe                           |            |      |            | ✅              | ✅            | 📝|

## Casos de Uso por Actor

| Profesor | Recursos Humanos | Ordenación | Técnico de calidad |
|----------|------------------|------------|--------------------|
| ![Diagrama Profesor](/images/modelosUML/CdU/EstructurarCasosDeUso/profesor.svg) | ![Diagrama Recursos Humanos](/images/modelosUML/CdU/EstructurarCasosDeUso/RRHH.svg) | ![Diagrama Ordenacion](/images/modelosUML/CdU/EstructurarCasosDeUso/Ordenacion.svg) | ![Diagrama Tecnico de Calidad](/images/modelosUML/CdU/EstructurarCasosDeUso/TecnicoCalidad.svg) |