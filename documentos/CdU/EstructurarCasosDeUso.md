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