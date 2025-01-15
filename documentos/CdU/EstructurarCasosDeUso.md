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

---

### Relación `<<include>>`

| Caso de Uso Principal                 | Caso de Uso Incluido              | Explicación                                                                            |
|---------------------------------------|-----------------------------------|----------------------------------------------------------------------------------------|
| **Emitir Informe del Profesorado**    | Obtener Indicadores               | Los indicadores se obtienen antes de emitir el informe.                                |
| **Obtener Indicadores**               | Consultar Asignación por Profesor | Los indicadores dependen de la asignación por profesor.                                |
| **Asignar Valores en Memoria**        | Validar Memoria y Titulación      | Es necesario validar la memoria y titulación antes de asignar valores.                 |
| **Validar Memoria y Titulación**      | Consultar Claustro Docente        | Se revisa la memoria y titulación con la consulta al claustro docente.                 |
| **Revisar Carga Docente**             | Consultar Claustro Docente        | La revisión de la carga docente depende de la consulta al claustro docente.            |
| **Validar Datos del Profesorado**     | Consultar Claustro Docente        | Se consulta el claustro para validar los datos del profesorado.                        |
| **Modificar Datos del Profesorado**   | Validar Datos del Profesorado     | Modificar los datos requiere la validación previa de los mismos.                       |
| **Validar Datos del Profesorado**     | Introducir Datos Académicos       | La validación de datos del profesorado requiere introducir datos académicos del mismo. |

---

### Relación `<<extend>>`

| Caso de Uso Principal              | Caso de Uso Extendido        | Explicación                                                                  |
|------------------------------------|------------------------------|------------------------------------------------------------------------------|
| **Asignar Información a SIIU/DGU** | Validar Memoria y Titulación | La asignación de información se extiende si es necesario validar la memoria. |