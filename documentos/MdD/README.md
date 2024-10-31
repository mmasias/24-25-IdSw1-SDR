# 📊 Modelo de Dominio

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

---

## 1. Diagrama de Clases

El diagrama de clases muestra las entidades principales del sistema (como `Profesor`, `Asignatura`, `Titulacion`) y sus relaciones. Es una visión general de la estructura y conexiones del sistema académico de UNEATLANTICO.

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaDeClases.svg) | [Ver código](/modelosUML/diagramaDeClases.puml) |

- **Descripción**: 
  - `Profesor` imparte `Asignatura` y elabora `MemoriaAcademica`.
  - `Asignatura` está vinculada a `Titulacion` y `PlanEstudios`.
  - `PlanEstudios` y `Titulacion` pertenecen a un `Departamento`.

---

## 2. Diagrama de Objetos

Este diagrama representa instancias específicas de las clases, mostrando un escenario concreto en el que interactúan objetos relacionados con asignaturas, profesores y memorias académicas.

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaDeObjetos.svg) | [Ver código](/modelosUML/diagramaDeObjetos.puml) |

- **Descripción**:
  - `Juan Pérez` imparte `Programación` y elabora `Memoria1`.
  - `Programación` pertenece a `Ingeniería Informática` y al `Plan 2024` dentro del `Departamento de Ingeniería Informática`.

---

## 3. Diagrama de Estados

El diagrama de estados muestra el flujo de gestión de la carga de trabajo de los profesores, verificando compatibilidad con contrato y equivalencia en tiempo completo (EQ TC).

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados](/images/modelosUML/MdD/diagramaDeEstados.svg) | [Ver código](/modelosUML/diagramaDeEstados.puml) |

- **Descripción**:

  - **Sin_Asignacion**: Profesor sin carga asignada.
  - **Propuesta_Carga**: Genera carga preliminar (docencia, investigación, gestión).
  - **Verificar_Contrato**: Verifica si el contrato permite la carga.
  - **No_Valido**: Estado final si el contrato o EQ TC no permiten la carga.
  - **Revisión_EQ_TC**: Valida que EQ TC esté dentro de límites permitidos.
  - **Revisión_Carga**: Revisa proporción de carga; pasa a `Aprobada` o `Ajuste_Carga`.
  - **Ajuste_Carga**: Ajusta carga y regresa a `Revisión_EQ_TC`.
  - **Aprobada**: La carga es revisada y aprobada.
  - **Asignada**: Estado final; carga académica asignada y registrada.

--- 
