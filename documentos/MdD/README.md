# 📊 Modelo de Dominio

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

---

## 1. Diagrama de Clases


| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaDeClases.svg) | [Ver código](/modelosUML/diagramaDeClases.puml) |

- **Descripción**: 
  - `Profesor` imparte `Asignatura` y elabora `MemoriaAcademica`.
  - `Asignatura` está vinculada a `Titulacion` y `PlanEstudios`.
  - `PlanEstudios` y `Titulacion` pertenecen a un `Departamento`.

---

## 2. Diagrama de Objetos



| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaDeObjetos.svg) | [Ver código](/modelosUML/diagramaDeObjetos.puml) |

- **Descripción**:
  - `Juan Pérez` imparte `Programación` y elabora `Memoria1`.
  - `Programación` pertenece a `Ingeniería Informática` y al `Plan 2024` dentro del `Departamento de Ingeniería Informática`.

---

## 3. Diagrama de Estados


| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados](/images/modelosUML/MdD/diagramaDeEstados.svg) | [Ver código](/modelosUML/diagramaDeEstados.puml) |

- **Descripción**:

  - Profesor `Sin_Asignacion`. Se hace `Propuesta_Carga` y genera carga inicial.
  - `Verificar_Contrato` revisa compatibilidad con contrato o `No_Valido` rechaza por exceso de carga.
  - `Revisión_EQ_TC` verifica límite EQ TC.
  - `Revisión_Carga` valida carga; pasa a `Aprobada` (Carga adecuada y validada) o `Ajuste_Carga` (Se requieren cambios).
  - `Asignada` es la carga final asignada.

--- 
