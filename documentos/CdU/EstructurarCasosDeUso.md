# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|

## 🎯 **Objetivo**

El objetivo de este paso es **estructurar el modelo de los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/eCdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

## Añadir `Include` y `Extend`

|Include|Extend
|-|-
|Representan funcionalidad obligatoria y común|Representan comportamiento opcional o alternativo
|Reducen la duplicación de especificaciones|Permiten la extensibilidad del sistema

---

![](/images/modelosUML/CdU/EstructurarCasosDeUso/Sistema.svg)

---

### Relación `<<include>>`

| Caso de Uso Principal                        | Caso de Uso Incluido            | Explicación                                                                             |
|----------------------------------------------|---------------------------------|-----------------------------------------------------------------------------------------|
| **Emitir Informe del Profesorado**           | Obtener Indicadores             | Los indicadores se obtienen antes de emitir el informe.                                 |
| **Asignar Valores en Memoria**               | Validar Cumplimiento de Memoria | Es necesario validar el cumplimiento de memoria antes de asignar valores.               |
| **Validar Cumplimiento de Memoria**          | Consultar Claustro Docente      | Se revisa la memoria y titulación con la consulta al claustro docente.                  |
| **Revisar Profesores con Carga no Ajustada** | Consultar Claustro Docente      | La revisión de la carga docente no ajustada depende de la consulta al claustro docente. |
| **Asignar Carga Docente**                    | Consultar Claustro Docente      | La asignación de carga docente se realiza tras consultar el claustro docente.           |
| **Modificar Datos del Profesorado**          | Validar Datos del Profesorado   | Modificar los datos requiere la validación previa de los mismos.                        |
| **Validar Datos del Profesorado**            | Introducir Datos Académicos     | La validación de datos del profesorado requiere introducir datos académicos del mismo.  |
| **Validar Datos del Profesorado**            | Consultar Claustro Docente      | Se consulta el claustro para validar los datos del profesorado.                         |

---

### Relación `<<extend>>`

| Caso de Uso Principal              | Caso de Uso Extendido           | Explicación                                                                  |
|------------------------------------|---------------------------------|------------------------------------------------------------------------------|
| **Asignar Información a SIIU/DGU** | Validar Cumplimiento de Memoria | La asignación de información se extiende si es necesario validar la memoria. |