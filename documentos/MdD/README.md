<div align="center">

# 📊 Modelo de Dominio

</div>

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

## 1. Diagrama de Clases

| **Diagrama** | **Descripción** |
|--------------|------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/DiagramaClases.svg) | - La `Asignación` asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`. <br> - La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica). <br> - La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores utilizando [`Indicadores`](/documentos/glosario.md#-indicador), que extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador). <br> - [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador). |


## 2. Diagrama de Objetos

| **Diagrama** | **Descripción** |
|--------------|------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/DiagramaObjetos.svg) | - La `Asignación` (id_asignacion = 1001) asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`. <br> - La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica), asegurándose de que los valores comprometidos se alcancen. <br> - La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores, como la movilidad y los sexenios, utilizando [`Indicadores`](/documentos/glosario.md#-indicador) (como el código "IND001"). Estos indicadores extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador). <br> - [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) (id_profesor = 001) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador). Además, cumple con las validaciones de movilidad y mantiene destinos de movilidad establecidos. <br> - La `Asignatura` (codigo = "INF101", nombre = "Programación I") pertenece a la `Titulación` (nombre = "Grado en Ingeniería Informática") y tiene asignado un porcentaje del 50% de carga académica para el curso "2023/2024". |


## 3. Diagramas de Estados 

| **Diagrama** | **Descripción**  |
|--------------|--------------------|
| ![Diagrama de Estados Profesor](/images/modelosUML/MdD/DiagramaEstadosProfesor.svg) | Representa el ciclo de estados de un `Profesor` en el sistema, comenzando desde un estado `Libre` hasta alcanzar un estado `Lleno`. <br> - En `Libre`, se verifica que la carga docente del profesor no esté completa (`CargaVerificada`). <br> - Durante el estado `EnProceso`, se valida la asignatura antes de asignarla al profesor (`AsignaturaValidada` y `AsignaturaAsignada`). <br> - Al completar la asignación, el estado pasa a `Lleno`, indicando que la carga docente máxima ha sido alcanzada. <br> - Se puede reiniciar el proceso mediante un reset o cancelar asignaciones en progreso. |
| ![Diagrama de Estados Asignatura](/images/modelosUML/MdD/DiagramaEstadosAsignatura.svg) | Representa el ciclo de estados de una `Asignatura`, desde estar `Libre` hasta estar `Completa`. <br> - En el estado `Libre`, se verifica que aún queden horas por asignar a una asignatura (`CapacidadVerificada`). <br> - Durante el estado `EnProceso`, se valida al profesor antes de asignarlo (`ProfesorValidado` y `ProfesorAsignado`). <br> - Cuando la asignación de profesores está completa, la asignatura pasa al estado `Completa`, indicando que todas las horas han sido cubiertas. <br> - Es posible realizar un reset o cancelar el proceso de asignación en progreso. |