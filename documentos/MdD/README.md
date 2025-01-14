<div align="center">

# 📊 Modelo de Dominio

</div>

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

## 1. Diagrama de Clases

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaDeClases.svg) | [Ver código](/modelosUML/MdD/diagramaDeClases.puml) |

- **Descripción**: 
  - La `Asignación` asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.

  - La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica).

  - La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores utilizando [`Indicadores`](/documentos/glosario.md#-indicador), que extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).

  - [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador).

## 2. Diagrama de Objetos

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaDeObjetos.svg) | [Ver código](/modelosUML/MdD/diagramaDeObjetos.puml) |

- **Descripción**:
  - La `Asignación` (id_asignacion = 1001) asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.

  - La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica), asegurándose de que los valores comprometidos se alcancen.

  - La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores, como la movilidad y los sexenios, utilizando [`Indicadores`](/documentos/glosario.md#-indicador) (como el código "IND001"). Estos indicadores extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).

  - [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) (id_profesor = 001) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador). Además, cumple con las validaciones de movilidad y mantiene destinos de movilidad establecidos.

  - La `Asignatura` (codigo = "INF101", nombre = "Programación I") pertenece a la `Titulación` (nombre = "Grado en Ingeniería Informática") y tiene asignado un porcentaje del 50% de carga académica para el curso "2023/2024".

## 3. Diagramas de Estados

### 3.1 Diagrama de Estado para Gestión de Profesores

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 1](/images/modelosUML/MdD/diagramaDeEstados1.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados1.puml) |

- **Descripción**:
  - Un `Profesor` es seleccionado, verificando su disponibilidad y carga actual. Se procede a asignarle una `Asignatura`, revisando compatibilidad contractual y los grupos disponibles.

  - La asignación genera una `Carga Validada`, donde se comparan las proporciones de trabajo (docencia, investigación, gestión) con los límites del contrato del profesor.  

  - Si la carga asignada resulta incorrecta, se entra al estado de `Ajuste Necesario`, modificando las proporciones para corregir desbalances, antes de regresar a validar la carga. 

  - Finalmente, una vez validada la carga, se verifica el `Cumplimiento Normativo`. Si no cumple, el proceso termina sin asignación; si cumple, se registra la `Asignación Completa`, concluyendo el flujo.

---

### 3.2 Diagrama de Estado para Gestión de Asignaturas

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 2](/images/modelosUML/MdD/diagramaDeEstados2.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados2.puml) |

- **Descripción**:
  - El flujo inicia con la selección de una `Asignatura`, donde se revisan los grupos pendientes y los requisitos necesarios para impartirla. Luego, se asigna un `Profesor`, verificando su disponibilidad, compatibilidad con el contrato y adecuación al EQ TC.  

  - Tras asignar al profesor, se valida la asignatura en el estado de `Asignatura Validada`, comprobando que todos los grupos están cubiertos y los balances de carga son correctos. Si existen desbalances, el sistema entra a `Ajuste Profesor`, donde se reasignan profesores o grupos antes de volver a validar.  

  - Al concluir esta validación, se realiza una `Revisión Legal`. Si cumple con los requisitos normativos, se registra como una `Asignación Completada`. En caso contrario, el flujo finaliza sin asignación válida.

---

### 3.3 Diagrama de Estado para Validación de Indicadores e Informes

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 3](/images/modelosUML/MdD/diagramaDeEstados3.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados3.puml) |

- **Descripción**:
  - El flujo comienza con la `Entradas Preparadas`, verificando las memorias y asignaciones iniciales. Una vez preparados, se validan los datos en `Entradas Validadas` para asegurar su consistencia. Si son correctos, se generan los indicadores necesarios en `Indicadores Generados` para la creación del informe.

  - A continuación, se genera el informe en `Informe Generado` a partir de los indicadores y se valida su cumplimiento legal. Si es necesario, el informe se ajusta en `Informe Ajustado` antes de ser validado de nuevo en `Informe Validado`. Finalmente, una vez validado, el informe queda listo para su uso.

  - Si en cualquier etapa se detectan errores en los datos, el flujo regresa a la corrección de entradas en `Entradas Corrigidas` antes de continuar.