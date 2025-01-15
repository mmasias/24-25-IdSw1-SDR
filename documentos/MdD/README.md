<div align="center">

# 📊 Modelo de Dominio

</div>

Este documento presenta los diagramas principales del modelo de dominio: el **diagrama de clases**, **diagrama de objetos**, y **diagrama de estados**. Para cada uno, se muestra una representación visual en SVG y un enlace al código fuente en formato `.puml`.

## 1. Diagrama de Clases

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Clases](/images/modelosUML/MdD/diagramaDeClases.svg) | [Ver código](/modelosUML/MdD/diagramaDeClases.puml) |

- La `Asignación` asigna a un [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador), quien imparte una `Asignatura` que pertenece a una `Titulación`.
- La `Asignación` también corresponde a una `Asignatura` y cumple con la [`Memoria Académica`](/documentos/glosario.md#-memoria-académica).
- La [`Memoria Académica`](/documentos/glosario.md#-memoria-académica) establece metas y valores utilizando [`Indicadores`](/documentos/glosario.md#-indicador), que extraen datos del [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador).
- [`Profesor`](/documentos/glosario.md#-pdi-personal-docente-e-investigador) imparte las `Asignaturas` relacionadas y contribuye a los datos que evalúan los [`Indicadores`](/documentos/glosario.md#-indicador).

## 2. Diagrama de Objetos

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Objetos](/images/modelosUML/MdD/diagramaDeObjetos.svg) | [Ver código](/modelosUML/MdD/diagramaDeObjetos.puml) |

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

- **`Profesor_Seleccionado`**: Verifica que el profesor esté disponible y cumpla los requisitos iniciales.  
- **`Asignatura_Asignada`**: Evalúa la compatibilidad de grupos y carga asignada al profesor.  
- **`Carga_Validada`**: Revisa el balance de carga académica para garantizar su distribución adecuada.  
- **`Ajuste_Necesario`**: Realiza ajustes en caso de que la carga esté incorrectamente distribuida.  
- **`Revisión_Legal`**: Asegura el cumplimiento de normativas educativas antes de finalizar la asignación.  
- **`Asignacion_Completa`**: Representa el registro final del proceso exitoso.


---

### 3.2 Diagrama de Estado para Gestión de Asignaturas

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 2](/images/modelosUML/MdD/diagramaDeEstados2.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados2.puml) |

- **`Asignatura_Seleccionada`**: Revisa los requisitos y compatibilidad de los grupos para la asignatura.  
- **`Profesor_Asignado`**: Confirma que el profesor seleccionado sea adecuado para la asignatura.  
- **`Asignatura_Validada`**: Verifica la proporción y balance de carga para asegurar que la asignación sea correcta.  
- **`Ajuste_Profesor`**: Permite reasignar profesores en caso de problemas detectados en la validación.  
- **`Revisión_Legal`**: Valida el cumplimiento normativo para proceder con la asignación final.  
- **`Asignacion_Completada`**: Marca la finalización del proceso con todos los requisitos cumplidos.

---

### 3.3 Diagrama de Estado para Validación de Indicadores e Informes

| **Diagrama** | **Código Fuente** |
|--------------|--------------------|
| ![Diagrama de Estados 3](/images/modelosUML/MdD/diagramaDeEstados3.svg) | [Ver código](/modelosUML/MdD/diagramaDeEstados3.puml) |

- **`Entradas_Preparadas`**: Comprueba que las memorias y asignaciones iniciales estén listas para el proceso.  
- **`Entradas_Validadas`**: Asegura la consistencia y corrección de los datos iniciales antes de avanzar.  
- **`Indicadores_Generados`**: Calcula los indicadores a utilizar, como información de memorias y cargas académicas.
- **`Informe_Generado`**: Crea el informe con los datos e indicadores revisados.  
- **`Informe_Ajustado`**: Permite modificar el informe si se detectan errores o necesidades de mejora.  
- **`Informe_Validado`**: Representa el informe final validado y listo para exportación.