# 📝 Estructurar el Modelo de Casos de Uso

| [⬅️ Prototipar Casos de Uso](PrototiparCasosDeUso.md) |
|:--|


## 🎯 **Objetivo**

El objetivo de este paso es **estructurar los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.ICdU.md) de la asignatura para reducir redundancias, identificar funcionalidades compartidas y opcionales, y aplicar las relaciones de inclusión/extensión según las pautas establecidas. 

---

## 🔍 **Identificar descripciones de funcionalidad compartida**

Para reducir la redundancia, debemos identificar acciones o partes de acciones comunes compartidas por varios casos de uso. Esto incluye:

1. **Generalización de Casos de Uso**:
   - Un caso de uso `A` generaliza a un caso de uso `B` cuando una instancia de `A` incluye el comportamiento especificado por `B`.
   - **Ejemplo**: Si varios casos de uso necesitan mostrar un estado común, este comportamiento puede generalizarse en un caso de uso abstracto.

2. **Casos de Uso Concretos y Abstractos**:
   - Los **casos de uso concretos** son iniciados por un actor y describen una secuencia completa de acciones realizadas por el sistema.
   - Los **casos de uso abstractos** no se instancian por sí mismos; existen para ser reutilizados por otros casos de uso.

---

## 🧩 **Identificar descripciones opcionales y adicionales de funcionalidad**

Las relaciones de inclusión y extensión ayudan a manejar la funcionalidad opcional y adicional:

1. **Inclusión**:
   - Proporciona una extensión explícita e incondicional a un caso de uso.
   - Relación entre dos casos de uso donde uno incluye al otro siempre que se ejecuta.

2. **Extensión**:
   - Permite añadir comportamiento adicional sujeto a condiciones específicas.
   - Incluye un punto de extensión en el caso de uso destino donde puede realizarse la extensión.

---

## 👥 **Actores y Casos de Uso Relacionados**

| Caso de Uso                                                                         | Profesores | RRHH | Ordenación | Técnico Calidad | Administrador |
|-------------------------------------------------------------------------------------|------------|------|------------|-----------------|---------------|
| **Iniciar Sesión** en la plataforma                                                 | ✅         | ✅  | ✅         | ✅              | ✅           |
| **Introducir** Datos Académicos                                                     | ✅         |      |            |                 |               |
| **Consultar** valores asignados de Contrato y otros Datos Personales                | ✅         |      |            |                 |               |
| **Consultar** Asignación Docente (por titulación, curso y semestre)                 | ✅         |      |            |                 |               |
| **Validar** los Datos introducidos por el Profesorado                               |            | ✅   |            |                 | ✅            |
| **Modificar** los Datos introducidos por el Profesorado                             |            | ✅   |            |                 | ✅            |
| **Introducir** Datos Laborales                                                      |            | ✅   |            |                 | ✅            |
| **Revisar** listado de Profesores cuya Carga Docente no se ajusta al Contrato       |            | ✅   | ✅         |                 | ✅           |
| **Consultar** Claustro Docente (listado PDI asociado a una titulación)              |            | ✅   | ✅         | ✅              | ✅           |
| **Consultar** Asignación Docente por Profesor (créditos y asignaturas)              |            | ✅   | ✅         | ✅              | ✅           |
| **Validar** cumplimiento de compromisos de Memoria con los valores de la Titulación |            |      | ✅         | ✅              | ✅           |
| **Asignar** Carga Docente de Asignaturas a Profesores                               |            |      | ✅         |                 | ✅            |
| **Asignar** valores consignados en Memoria por Titulación                           |            |      |            | ✅              | ✅            |
| **Asignar** valor de Información a SIIU y DGU del PDI                               |            |      |            | ✅              | ✅            |
| **Obtener** Indicadores para Sistema de Gestión                                     |            |      |            | ✅              | ✅            |
| **Emitir** Informe del Profesorado (Global o por Titulación)                        |            |      |            | ✅              | ✅            |

---

## 🖼️ **Diagramas de Casos de Uso**

### Caso 1: Casos de Uso Básicos
![Casos de Uso Básicos](attachment:image1)

### Caso 2: Casos de Uso con Relaciones de Inclusión/Extensión
![Casos de Uso Avanzados](attachment:image2)

---

## 📌 **Notas Adicionales**

1. Los casos de uso **abstractos** y las relaciones de **inclusión/extensión** mejoran la reusabilidad y claridad del modelo.
2. Es importante identificar los puntos de extensión y las condiciones asociadas.
3. Los diagramas ilustrados deben complementarse con documentación textual detallada.

---

Este contenido ha sido generado para estructurar tus casos de uso siguiendo las mejores prácticas y las pautas teóricas proporcionadas.
