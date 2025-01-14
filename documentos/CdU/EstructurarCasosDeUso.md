# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|

## 🎯 **Objetivo**

El objetivo de este paso es **estructurar el modelo de los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/eCdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

## Modelo de Clases y Relaciones

![Clases y Relaciones](/images/modelosUML/CdU/EstructurarCasosDeUso/ClasesRelaciones.svg)

## Casos de Uso sin Estructurar

![Casos de Uso](/images/modelosUML/CdU/EstructurarCasosDeUso/CdU.svg)

## Casos de Uso por Actor

| Profesor | Recursos Humanos | Ordenación | Técnico de calidad |
|----------|------------------|------------|--------------------|
| ![Diagrama Profesor](/images/modelosUML/CdU/EstructurarCasosDeUso/profesor.svg) | ![Diagrama Recursos Humanos](/images/modelosUML/CdU/EstructurarCasosDeUso/RRHH.svg) | ![Diagrama Ordenacion](/images/modelosUML/CdU/EstructurarCasosDeUso/Ordenacion.svg) | ![Diagrama Tecnico de Calidad](/images/modelosUML/CdU/EstructurarCasosDeUso/TecnicoCalidad.svg) |

## Añadir `Include` y `Extend`

|Include|Extend
|-|-
|Representan funcionalidad obligatoria y común|Representan comportamiento opcional o alternativo
|Reducen la duplicación de especificaciones|Permiten la extensibilidad del sistema

---

![](/images/modelosUML/CdU/EstructurarCasosDeUso/Sistema.svg)

| **Actor**             | **Caso de Uso**                   | **Incluye**                       | **Extiende**                 | **Motivo**                                                                                     |
|-----------------------|-----------------------------------|-----------------------------------|------------------------------|------------------------------------------------------------------------------------------------|
| **RRHH**              | Validar Datos del Profesorado     | Consultar Claustro Docente        |                              | Para validar los datos de un profesor, es obligatorio consultar su información en el claustro. |
|                       | Modificar Datos del Profesorado   | Validar Datos del Profesorado     |                              | Antes de modificar datos, es obligatorio validar que los datos actuales sean correctos.        |
| **Ordenación**        | Asignar Carga Docente             | Consultar Claustro Docente        |                              | Para asignar carga docente, es obligatorio consultar los profesores disponibles.               |
| **Técnico de Calidad**| Validar Memoria y Titulación      | Consultar Claustro Docente        |                              | Para validar la memoria, es obligatorio consultar la composición actual del claustro.          |
|                       | Emitir Informe del Profesorado    | Obtener Indicadores               |                              | Para generar el informe, es obligatorio tener los indicadores calculados.                      |
|                       | Obtener Indicadores               | Consultar Asignación Docente      |                              | Para calcular indicadores, es obligatorio consultar los datos de asignación docente.           |
|                       | Asignar Información a SIIU/DGU    |                                   | Validar Memoria y Titulación | Al asignar información, opcionalmente se puede decidir validarla contra la memoria.            |