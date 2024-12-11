<div align="center">

# 📊 Modelo de Dominio

</div>

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

---

## 1. Diagrama de Clases


| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaDeClases.svg) | [Ver código](/modelosUML/MdD/diagramaDeClases.puml) |

- **Descripción**: 
  - `Asignación` asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.  
  - La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica).  
  - La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores utilizando [`Indicadores`](/documentos/glosario.md#-indicador), que extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).  
  - [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador).

---

## 2. Diagrama de Objetos



| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaDeObjetos.svg) | [Ver código](/modelosUML/MdD/diagramaDeObjetos.puml) |

- **Descripción**:
  - La `Asignación` (#1001) asigna al [`Profesor`](documentos/glosario.md#-pdi-personal-docente-e-investigador) (Dr. Juan Pérez), quien imparte la `Asignatura` (Programación I) vinculada al Grado en Ingeniería Informática.
  - La `Asignación` corresponde a la `Asignatura` (INF101), cumple los objetivos establecidos en la [`Memoria Académica`](documentos/glosario.md#-memoria-académica) del curso 2023/2024 y gestiona una [`Carga Académica`](documentos/glosario.md#-carga-académica) de 24 créditos en modalidad Presencial.
  - La [`Memoria Académica`](documentos/glosario.md#-memoria-académica) establece un [`Indicador`](documentos/glosario.md#-indicador) (IND001) con un valor de 75, superando el umbral de alerta establecido en 60, para monitorear metas como la movilidad académica y los [sexenios](documentos/glosario.md#-sexenio) del profesor.
  - El [`Profesor`](documentos/glosario.md#-pdi-personal-docente-e-investigador) (Dr. Juan Pérez) tiene un historial de contrato que incluye períodos como Titular y Catedrático, así como experiencia previa como Investigador y Profesor Asociado.
  - El [`Profesor`](documentos/glosario.md#-pdi-personal-docente-e-investigador) está validado para movilidad en instituciones como (Universidad A) y (Universidad B) y forma parte de la Facultad de Ingeniería en UNEATLANTICO.


---

## 3. Diagrama de Flujo


| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados](/images/modelosUML/MdD/diagramaDeEstados.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados.puml) |

- **Descripción**:

  - Profesor `Sin_Asignacion`. Se hace `Propuesta_Carga` y genera carga inicial.
  - `Verificar_Contrato` revisa compatibilidad con contrato o `No_Valido` rechaza por exceso de carga.
  - `Revisión_EQ_TC` verifica límite EQ TC.
  - `Revisión_Carga` valida carga; pasa a `Aprobada` (Carga adecuada y validada) o `Ajuste_Carga` (Se requieren cambios).
  - `Asignada` es la carga final asignada.