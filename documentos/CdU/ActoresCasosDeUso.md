# 📝 Encontrar Actores y Casos de Uso

[Priorizar Casos de Uso ➡️](PriorizarCasosDeUso.md) |
|--:|

## 🎯 Objetivo

El objetivo de este paso es **encontrar actores y casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.eAyCdU.md#c%C3%B3mo) de la asignatura.

## 👥 **Actores**  

![DiagramaDeActores](/images/modelosUML/CdU/Individuales/Actores.svg) 

## 📋 Casos de Uso y Actores Involucrados

| Caso de Uso                                  | Profesores | RRHH | Ordenación | Técnico Calidad | Administrador | Detalle | Prototipo |
|----------------------------------------------|------------|------|------------|-----------------|---------------|---------|-----------|
| **Iniciar Sesión**                           | ✅         | ✅  | ✅         | ✅              | ✅           | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Conjunto/IniciarSesion.svg) | [Ver](/images/Prototipar/Inicio.png) |
| **Introducir** Datos Académicos              | ✅         |      |            |                 |               | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Profesores/IntroducirDatosAcademicos.svg) | [Ver](/images/Prototipar/DatosAcademicos.png) |
| **Consultar** Datos Personales               | ✅         |      |            |                 |               | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Profesores/ConsultarValores.svg) | [Ver](/images/Prototipar/DatosContratoPersonales.png) |
| **Consultar** Asignación Docente             | ✅         |      |            |                 |               | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Profesores/ConsultarAsignacionFiltros.svg) | [Ver](/images/Prototipar/AsignaciónDocenteTitulacion.png) |
| **Validar** Datos del Profesorado            |            | ✅   |            |                 | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/RRHH/ValidarDatos.svg) | --- |
| **Modificar** Datos del Profesorado          |            | ✅   |            |                 | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/RRHH/ModificarDatos.svg) | [Ver](/images/Prototipar/ModificacionDatosProfesorado.png) |
| **Introducir** Datos Laborales               |            | ✅   |            |                 | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/RRHH/IntroducirDatosLaborales.svg)  | [Ver](/images/Prototipar/DatosLaborales.png) |
| **Revisar** Profesores con Carga no ajustada |            | ✅   | ✅         |                 | ✅           | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Conjunto/RevisarProfesores.svg) | --- |
| **Consultar** Claustro Docente               |            | ✅   | ✅         | ✅              | ✅           | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Conjunto/ConsultarClaustroDocente.svg)  | [Ver](/images/Prototipar/ConsultarClaustroDocente.png) |
| **Consultar** Asignación por Profesor        |            | ✅   | ✅         | ✅              | ✅           | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Conjunto/ConsultarAsignacion.svg) | [Ver](/images/Prototipar/ConsultaAsignaciónDocenteProfesor.png) |
| **Validar** Cumplimiento de Memoria          |            |      | ✅         | ✅              | ✅           | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Conjunto/ValidarMemoria.svg) | --- |
| **Asignar** Carga Docente                    |            |      | ✅         |                 | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/Ordenacion/AsignarCargaDocente.svg)  | [Ver](/images/Prototipar/AsignacióndeCargaDocente.png) |
| **Asignar** Valores en Memoria               |            |      |            | ✅              | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/TecnicoCalidad/AsignarValores.svg) | [Ver](/images/Prototipar/AsignarValores.png) |
| **Asignar** Información SIIU/DGU             |            |      |            | ✅              | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/TecnicoCalidad/AsignarSIIUyDGU.svg) | [Ver](/images/Prototipar/AsignarSIIU.png) |
| **Obtener** Indicadores                      |            |      |            | ✅              | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/TecnicoCalidad/ObtenerIndicadores.svg) | ---    |
| **Emitir** Informe                           |            |      |            | ✅              | ✅            | [Ver](/images/modelosUML/CdU/DetallarCasosDeUso/TecnicoCalidad/EmitirInforme.svg) | [Ver](/images/Prototipar/EmitirInformeProfesorado.png) |


## 🎭 Casos de Uso por Actor

| Profesor | Recursos Humanos | Ordenación | Técnico de calidad |
|----------|------------------|------------|--------------------|
| ![Diagrama Profesor](/images/modelosUML/CdU/PorActor/Profesor.svg) | ![Diagrama Recursos Humanos](/images/modelosUML/CdU/PorActor/RRHH.svg) | ![Diagrama Ordenacion](/images/modelosUML/CdU/PorActor/Ordenacion.svg) | ![Diagrama Tecnico de Calidad](/images/modelosUML/CdU/PorActor/TecnicoCalidad.svg) |

## 🗺️ Diagramas de Contexto

### Profesor

||
|-:|
![](/images/modelosUML/CdU/DiagramaDeContexto/Profesor.svg)

### Recursos Humanos

||
|-:|
![](/images/modelosUML/CdU/DiagramaDeContexto/RRHH.svg)

### Ordenación

||
|-:|
![](/images/modelosUML/CdU/DiagramaDeContexto/Ordenacion.svg)

### Técnico de Calidad

||
|-:|
![](/images/modelosUML/CdU/DiagramaDeContexto/TecnicoCalidad.svg)
