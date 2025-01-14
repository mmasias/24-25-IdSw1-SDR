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

---

# Beneficios

| Mantenibilidad                                  | Comprensión                                | Escalabilidad                              |
|------------------------------------------------|--------------------------------------------|-------------------------------------------|
| Facilita la modificación de funcionalidades específicas de actores como `Profesor` y `RRHH`. | Organización jerárquica clara en paquetes como "Gestión de Profesores" y "Gestión de Calidad". | Estructura preparada para añadir nuevas funcionalidades, como "Gestión de Indicadores". |
| Permite la evolución independiente de subsistemas como "Gestión de Memorias e Informes". | Separación lógica de funcionalidades en cada paquete. | Patrones claros para la extensión del sistema mediante relaciones `include` y `extend`. |

---

# ¿Cómo sé si...?

| Completitud                                     | Consistencia                              | Viabilidad                                |
|------------------------------------------------|-------------------------------------------|-------------------------------------------|
| Todos los requisitos funcionales están cubiertos, incluyendo la gestión de datos académicos y laborales. | No hay redundancia en la funcionalidad entre actores como `Ordenación` y `Técnico de Calidad`. | La estructura es implementable con casos de uso claros por paquete. |
| Cada caso de uso tiene un propósito claro, como "Consultar Claustro Docente" y "Emitir Informe del Profesorado". | Las dependencias son bidireccionales donde es necesario, como entre "Gestión de Calidad" y "Gestión de Ordenación". | Las interfaces entre paquetes, como "Gestión de Profesores" y "Gestión de Recursos Humanos", son claras. |
| Las relaciones están completamente especificadas con relaciones `include` y `extend`. | Los nombres son consistentes y significativos en todos los diagramas. | Los patrones de comunicación entre subsistemas son eficientes. |

---

# Entregables

1. Diagramas de paquetes de casos de uso.
2. Diagramas de casos de uso por paquete.
3. Especificación de relaciones entre casos de uso.
4. Matriz de trazabilidad de requisitos.

---