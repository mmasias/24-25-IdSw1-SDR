<div align="center">

# 📊 Modelo de Dominio

</div>

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

## 1. Diagrama de Clases

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/DiagramaDeClases.svg) | [Ver código](/modelosUML/MdD/DiagramaDeClases.puml) |

- La `Asignación` asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.
- La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica).
- La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores utilizando [`Indicadores`](/documentos/glosario.md#-indicador), que extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).
- [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador).

## 2. Diagrama de Objetos

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/DiagramaDeObjetos.svg) | [Ver código](/modelosUML/MdD/DiagramaDeObjetos.puml) |

- La `Asignación` (id_asignacion = 1001) asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.
- La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica), asegurándose de que los valores comprometidos se alcancen.
- La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores, como la movilidad y los sexenios, utilizando [`Indicadores`](/documentos/glosario.md#-indicador) (como el código "IND001"). Estos indicadores extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).
- [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) (id_profesor = 001) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador). Además, cumple con las validaciones de movilidad y mantiene destinos de movilidad establecidos.
- La `Asignatura` (codigo = "INF101", nombre = "Programación I") pertenece a la `Titulación` (nombre = "Grado en Ingeniería Informática") y tiene asignado un porcentaje del 50% de carga académica para el curso "2023/2024".

## 3. Diagramas de Estados

### 3.1 Diagrama de Estado de Profesor

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 1](/images/modelosUML/MdD/DiagramaDeEstadosProfesor.svg) | [Ver código](/modelosUML/MdD/DiagramaDeEstadosProfesor.puml) |


---

### 3.2 Diagrama de Estado de Asignatura

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 2](/images/modelosUML/MdD/DiagramaDeEstadosAsignatura.svg) | [Ver código](/modelosUML/MdD/DiagramaDeEstadosAsignatura.puml) |