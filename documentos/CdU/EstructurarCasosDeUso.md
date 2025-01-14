# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|

## 🎯 **Objetivo**

El objetivo de este paso es **estructurar el modelo de los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/eCdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

## 1️⃣ Primer Paso

![Paso 1](/images/modelosUML/CdU/EstructurarCasosDeUso/Paso1.svg)

## 2️⃣ Segundo Paso

![Paso 2](/images/modelosUML/CdU/EstructurarCasosDeUso/Paso2.svg)

# Decisiones & Criterios por Actor

| Actor                   | Cohesión funcional                          | Minimización de dependencias                     | Reutilización                                      |
|-------------------------|---------------------------------------------|------------------------------------------------|--------------------------------------------------|
| **Profesor**            | Agrupar las acciones relacionadas con la consulta y modificación de asignaciones. | Minimizar la dependencia de otros sistemas académicos. | Usar operaciones comunes como casos de uso `include`. |
| **Recursos Humanos**    | Unificar las operaciones de validación y registro de datos académicos y laborales. | Documentar las dependencias con bases de datos externas. | Extender casos de uso para variaciones de validación. |
| **Ordenación**          | Manejar de forma conjunta la asignación y revisión de carga docente. | Reducir dependencias entre indicadores y métricas. | Reutilizar operaciones comunes como casos de uso `include`. |
| **Técnico de Calidad**  | Agrupar las acciones relacionadas con memoria, informes y validación de calidad. | Evitar duplicidad en cálculos de indicadores y límites. | Separar variaciones en casos de uso `extend`. |



| Profesor                                | Recursos Humanos                                 | Ordenación                               | Técnico de calidad               |
|------------------------------------------|---------------------------------------|----------------------------------------|-----------------------------------------|
| ![Diagrama Profesor](/images/modelosUML/CdU/EstructurarCasosDeUso/profesor.svg) | ![Diagrama Médico](/images/modelosUML/CdU/EstructurarCasosDeUso/RRHH.svg) | ![Diagrama Paciente](/images/modelosUML/CdU/EstructurarCasosDeUso/Ordenacion.svg) | ![Diagrama Administrativo](/images/modelosUML/CdU/EstructurarCasosDeUso/TecnicoCalidad.svg) |

---
# Decisiones sobre `Include` y `Extend`

| Include                                     | Extend                                      |
|---------------------------------------------|--------------------------------------------|
| Representan funcionalidad obligatoria y común en casos de uso como la validación de datos o consulta de indicadores. | Representan comportamiento opcional o alternativo, como extensiones para validar memoria y titulación. |
| Reducen la duplicación de especificaciones mediante operaciones comunes entre actores del sistema académico. | Permiten la extensibilidad del sistema, manejando variaciones como la asignación específica de memoria. |

---

![](/images/modelosUML/CdU/EstructurarCasosDeUso/esquema.svg)
