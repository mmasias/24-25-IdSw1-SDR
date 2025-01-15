<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |


</div>

# Casos de Uso Detallados

### 1. [Verificar Cumplimiento con Memoria Verificada](/CasosDeUso/Actividades/Prototipos/README.md#dirección-de-calidad---verificar-cumplimiento-con-memoria-verificada)
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad debe verificar que las guías docentes se adhieren a la memoria verificada de la titulación, asegurando así el cumplimiento de los lineamientos institucionales. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de verificación.<br> 2. El sistema muestra la lista de guías docentes disponibles para verificación.<br> 3. La Dirección de Calidad selecciona una guía para verificar.<br> 4. El sistema utiliza la API de verificación para comparar la guía con la memoria verificada de la titulación.<br> 5. El sistema determina si la guía cumple con los requisitos de memoria verificada.<br> 6. El sistema notifica el resultado de la verificación a la Dirección de Calidad. |
| **Flujos alternativos y excepciones** | Si la guía no cumple con los requisitos, el sistema notifica a la Dirección de Calidad y permite enviar la guía para ajustes. |
| **Precondiciones**                | La Dirección de Calidad debe tener acceso al sistema y a la API de verificación, y la guía debe estar registrada en el sistema. |
| **Postcondiciones**               | El sistema confirma el cumplimiento de la guía con la memoria verificada o notifica las observaciones para ajustes. |

![](/images/modelosUML/VerificarGD.svg)

### 2. [Auditar Guías Docentes](/CasosDeUso/Actividades/Prototipos/README.md#dirección-de-calidad---auditar-guías-docentes)
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad realiza auditorías exhaustivas de las guías docentes para evaluar la calidad del contenido y asegurar que cumplen con los objetivos académicos de la institución. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de auditoría.<br> 2. El sistema muestra la lista de guías docentes disponibles para auditar.<br> 3. La Dirección de Calidad selecciona una guía para revisar su contenido.<br> 4. El sistema despliega la guía seleccionada, permitiendo revisar secciones clave de contenido y alineación con los objetivos institucionales.<br> 5. La Dirección de Calidad realiza comentarios o solicitudes de ajuste, si aplica.<br> 6. El sistema guarda la auditoría y notifica que la revisión se ha completado. |
| **Flujos alternativos y excepciones** | Si se identifican problemas en la guía, el sistema permite a la Dirección de Calidad documentar observaciones y solicitar ajustes antes de aprobar la guía. |
| **Precondiciones**                | Acceso al sistema de auditoría y guías docentes disponibles para revisión. |
| **Postcondiciones**               | La auditoría se completa y se guarda, permitiendo que los ajustes se hagan antes de aprobar la guía. |


![](/images/modelosUML/AuditarGD.svg)

### 3. [Publicar Guía Docente](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---publicar-guía-docente)
-------------
| **Identificación de actores**      | Director de Grado |
|------------------------------------|-------------------|
| **Escenario**                      | El Director de Grado tiene la responsabilidad de autorizar la publicación final de las guías docentes, permitiendo que los estudiantes accedan a una versión oficial y aprobada de la guía. |
| **Flujo de eventos principal**     | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes aprobadas y listas para publicación.<br> 3. El Director de Grado selecciona una guía para publicar.<br> 4. El sistema solicita confirmación de la publicación final.<br> 5. El Director de Grado confirma la publicación.<br> 6. El sistema publica la guía, haciéndola accesible para los estudiantes a través del panel universitario. |
| **Flujos alternativos y excepciones** | Si el Director de Grado cancela la operación, el sistema retorna a la lista de guías sin realizar la publicación. |
| **Precondiciones**                | Acceso al sistema de gestión de guías docentes. La guía debe estar lista y aprobada para su publicación. |
| **Postcondiciones**               | La guía se publica y es accesible a los estudiantes, o la operación es cancelada sin cambios. |


![](/images/modelosUML/PublicarGD.svg) 

### 4. [Editar Contenido de la Guía](/CasosDeUso/Actividades/Prototipos/README.md#profesor---editar-guía)
| **Identificación de actores**      | Profesor |
|------------------------------------|----------|
| **Escenario**                      | El profesor accede al sistema para actualizar el contenido de la guía docente de una asignatura, con el fin de reflejar cambios en el temario, bibliografía, o metodologías de evaluación. |
| **Flujo de eventos principal**     | 1. El profesor inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes asignadas al profesor.<br> 3. El profesor selecciona una guía para editar.<br> 4. El sistema despliega el contenido actual de la guía.<br> 5. El profesor realiza las modificaciones necesarias en el contenido.<br> 6. El sistema guarda los cambios realizados y actualiza la guía. |
| **Flujos alternativos y excepciones** | Si el profesor desea descartar los cambios, el sistema permite cancelar la operación sin guardar.<br> Si se detecta un error en el contenido, el sistema muestra un mensaje indicando el problema antes de guardar. |
| **Precondiciones**                | El profesor debe tener acceso al sistema y permisos para editar la guía asignada. |
| **Postcondiciones**               | La guía queda actualizada con los cambios realizados, o se cancela la edición sin que se guarden modificaciones. |


![](/images/modelosUML/EditarContenidoGD.svg)

### 5. [Revisar Contenido](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---revisar-contenido)

| **Identificación de actores**                          | **Director de Grado**                                                                 |
|--------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| **Escenario**                        | El Director de Grado revisa el contenido de una guía docente y decide si aprueba o rechaza su publicación, asegurando que cumple estándares académicos. |
| **Flujo de eventos principal**       | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías pendientes de aprobación.<br> 3. Selecciona una guía para revisar su contenido.<br> 4. El sistema despliega el contenido completo de la guía.<br> 5. Decide aprobar el contenido.<br> 6. El sistema marca la guía como aprobada y la prepara para publicación. |
| **Flujos alternativos y excepciones**| - Si el Director de Grado decide rechazar el contenido, el sistema permite registrar comentarios de retroalimentación y marca la guía como "Requiere Revisión".<br> - Si ocurre un error en la carga del contenido, el sistema notifica al Director de Grado y cancela la operación. |
| **Precondiciones**                   | - Acceso al sistema y a las guías pendientes de aprobación.<br> - El contenido debe estar completo y listo para revisión.                      |
| **Postcondiciones**                  | - La guía queda aprobada y lista para publicación.<br> - O se marca como "Requiere Revisión" con comentarios para ajustes.                      |

![](/images/modelosUML/RevisarContenidoGD.svg)

### 6. [Generar Nueva Versión de la Guía](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---generar-nueva-versión)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad solicita al sistema la creación de una nueva versión de una guía docente para registrar cambios recientes en el contenido y mantener un historial de versiones. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de versiones de guías.<br> 2. El sistema muestra la lista de guías con opción de crear nueva versión.<br> 3. El Técnico de Calidad selecciona una guía y solicita generar una nueva versión.<br> 4. El sistema crea una nueva versión de la guía, basada en el contenido existente.<br> 5. El Técnico de Calidad confirma la creación de la nueva versión.<br> 6. El sistema guarda la nueva versión y la marca como la versión activa. |
| **Flujos alternativos y excepciones** | Si ocurre un error durante la generación de la nueva versión, el sistema notifica al Técnico de Calidad y permite reintentar o cancelar la operación. |
| **Precondiciones**                | El técnico debe tener acceso al sistema de gestión de versiones y permisos para generar nuevas versiones de las guías. |
| **Postcondiciones**               | Una nueva versión de la guía queda registrada y disponible para futuras ediciones o revisiones. |


![](/images/modelosUML/GenerarVersiónGD.svg)

### 7.[Ver listado de los estados de las guías docentes](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---ver-listado-de-estado-de-guías)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad solicita al sistema visualizar los estados en los que se encuentran las guías docentes, para mantener la trazabilidad de los procesos y tomar decisiones informadas. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de guías.<br> 2. El sistema presenta el menú principal con las opciones disponibles.<br> 3. El Técnico de Calidad selecciona la opción "Ver listado de estados de las guías docentes".<br> 4. El sistema visualiza una tabla con los siguientes datos para cada guía docente:<br>&nbsp;&nbsp;&nbsp;&nbsp;- Título de la guía<br>&nbsp;&nbsp;&nbsp;&nbsp;- Estado actual (aprobado, devuelto para modificación, pendiente, etc.)<br>&nbsp;&nbsp;&nbsp;&nbsp;- Responsable actual<br>&nbsp;&nbsp;&nbsp;&nbsp;- Fecha de última modificación.<br> 5. El Técnico de Calidad filtra o ordena la información según sea necesario. |
| **Flujos alternativos y excepciones** | Si no hay guías registradas, el sistema muestra un mensaje indicando que no hay datos disponibles.<br> Si ocurre un error técnico al intentar cargar la información, el sistema notifica al Técnico de Calidad y permite reintentar la operación. |
| **Precondiciones**                | El Técnico de Calidad debe tener acceso al sistema y permisos para visualizar el listado de estados de las guías docentes. |
| **Postcondiciones**               | El Técnico de Calidad obtiene información actualizada sobre el estado de las guías docentes para realizar un seguimiento adecuado. |

![](/images/modelosUML/VerListadoEstadosGD.svg)


### 8. [Ver listado de los estados de las guías por grado](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---ver-listado-de-guías)
| **Identificación de actores**      | Director de Grado |
|------------------------------------|--------------------|
| **Escenario**                      | El Director de Grado solicita al sistema visualizar los estados en los que se encuentran las guías docentes de su grado, para asegurar la trazabilidad y gestionar adecuadamente el proceso de aprobación. |
| **Flujo de eventos principal**     | 1. El Director de Grado accede al sistema de gestión de guías.<br> 2. El sistema presenta el menú principal con las opciones disponibles.<br> 3. El Director de Grado selecciona la opción "Ver listado de estados de las guías de mi grado".<br> 4. El sistema visualiza una tabla con los siguientes datos para cada guía docente del grado:<br>&nbsp;&nbsp;&nbsp;&nbsp;- Título de la guía<br>&nbsp;&nbsp;&nbsp;&nbsp;- Estado actual (aprobado, devuelto para modificación, pendiente, etc.)<br>&nbsp;&nbsp;&nbsp;&nbsp;- Responsable actual<br>&nbsp;&nbsp;&nbsp;&nbsp;- Fecha de última modificación.<br> 5. El Director de Grado filtra o ordena la información según los criterios necesarios. |
| **Flujos alternativos y excepciones** | Si no hay guías registradas para el grado, el sistema muestra un mensaje indicando que no hay datos disponibles.<br> Si ocurre un error técnico al intentar cargar la información, el sistema notifica al Director de Grado y permite reintentar la operación. |
| **Precondiciones**                | El Director de Grado debe tener acceso al sistema y permisos para visualizar el listado de estados de las guías docentes de su grado correspondiente. |
| **Postcondiciones**               | El Director de Grado obtiene información actualizada sobre el estado de las guías docentes de su grado para realizar un seguimiento adecuado. |

![](/images/modelosUML/VerListadoEstadosGradoGD.svg)


### 9.[Editar plantilla de la guía docente](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---editar-plantilla)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad solicita al sistema realizar modificaciones en el formato de la plantilla de una guía docente para garantizar que se ajusta a las normas académicas y organizativas. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de plantillas.<br> 2. El sistema presenta una lista de plantillas disponibles para las guías docentes.<br> 3. El Técnico de Calidad selecciona la plantilla que desea editar.<br> 4. El sistema muestra el contenido editable de la plantilla, incluyendo secciones como introducción, objetivos, metodología, etc.<br> 5. El Técnico de Calidad realiza las modificaciones necesarias en las secciones de la plantilla.<br> 6. El sistema valida los cambios realizados para garantizar que cumplen con los formatos requeridos.<br> 7. El Técnico de Calidad guarda los cambios realizados en la plantilla.<br> 8. El sistema actualiza la plantilla y notifica al Técnico de Calidad que los cambios se han guardado correctamente. |
| **Flujos alternativos y excepciones** | Si el Técnico de Calidad intenta guardar cambios con un formato inválido, el sistema muestra un mensaje de error indicando el problema y permite corregirlo antes de guardar.<br> Si ocurre un error técnico durante el guardado, el sistema notifica al Técnico de Calidad y permite reintentar o cancelar la operación. |
| **Precondiciones**                | El Técnico de Calidad debe tener acceso al sistema y permisos para editar plantillas de guías docentes. La plantilla seleccionada debe existir en el sistema. |
| **Postcondiciones**               | La plantilla queda actualizada en el sistema y disponible para su uso en la creación de nuevas guías docentes. |

![](/images/modelosUML/EditarPlantillaGD.svg)


### 10. [Asignar Guía a Titulación](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---asignar-guía-a-titulación)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad asigna una guía docente a una titulación específica para facilitar su organización en el sistema. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de guías.<br> 2. El sistema muestra una lista de guías disponibles.<br> 3. El Técnico de Calidad selecciona una guía para asignar a una titulación.<br> 4. El sistema muestra una lista de titulaciones disponibles.<br> 5. El Técnico de Calidad selecciona la titulación correspondiente.<br> 6. El sistema asocia la guía con la titulación seleccionada y guarda la relación. |
| **Flujos alternativos y excepciones** | Si la guía ya está asignada a una titulación, el sistema notifica al Técnico de Calidad y solicita confirmación para cambiar la asignación.<br> Si ocurre un error, el sistema permite reintentar o cancelar la operación. |
| **Precondiciones**                | Acceso al sistema de gestión de guías y titulaciones. |
| **Postcondiciones**               | La guía queda asociada a la titulación seleccionada. |

![](/images/modelosUML/AsignarATitulacionGD.svg)

---
### 11. [Asignar Asignatura a Titulación](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---asignar-asignatura-a-titulación)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad asocia una asignatura con su titulación correspondiente en el sistema, asegurando una correcta organización del plan académico. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión académica.<br> 2. El sistema muestra una lista de asignaturas registradas.<br> 3. El Técnico de Calidad selecciona una asignatura para asignarla a una titulación.<br> 4. El sistema muestra una lista de titulaciones disponibles.<br> 5. El Técnico de Calidad selecciona la titulación correspondiente.<br> 6. El sistema asocia la asignatura con la titulación seleccionada y guarda la relación. |
| **Flujos alternativos y excepciones** | Si la asignatura ya está asociada a una titulación, el sistema notifica al Técnico de Calidad y solicita confirmación para actualizar la asignación.<br> Si ocurre un error, el sistema muestra un mensaje y permite reintentar o cancelar la operación. |
| **Precondiciones**                | El Técnico de Calidad debe tener acceso al sistema de gestión académica y permisos para asignar asignaturas. |
| **Postcondiciones**               | La asignatura queda correctamente asociada a la titulación seleccionada en el sistema. |

![](/images/modelosUML/AsignarAsignaturaTitulacionGD.svg)


### 12. [Asignar Guías Docentes a Profesor](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---asignar-guía-a-profesor)
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad solicita al sistema asignar una guía docente a un profesor para garantizar que este pueda trabajar en su contenido. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de guías docentes.<br> 2. El sistema presenta una lista de guías docentes disponibles para asignar.<br> 3. El Técnico de Calidad selecciona una guía docente de la lista.<br> 4. El sistema muestra una lista de profesores disponibles.<br> 5. El Técnico de Calidad selecciona un profesor al cual asignar la guía.<br> 6. El sistema valida la asignación y registra la relación entre el profesor y la guía.<br> 7. El sistema notifica al Técnico de Calidad que la asignación se ha realizado exitosamente. |
| **Flujos alternativos y excepciones** | Si la guía docente ya está asignada a otro profesor, el sistema muestra un mensaje de error indicando que la guía no está disponible para una nueva asignación.<br> Si no hay profesores disponibles, el sistema notifica al Técnico de Calidad y permite buscar o registrar un nuevo profesor antes de proceder. |
| **Precondiciones**                | El Técnico de Calidad debe tener acceso al sistema y permisos para asignar guías docentes. Debe existir al menos un profesor registrado y una guía docente disponible en el sistema. |
| **Postcondiciones**               | La guía docente queda asignada al profesor seleccionado, quien puede comenzar a trabajar en ella. |

![](/images/modelosUML/AsignarProfesorGD.svg)

## 13. [Enviar Guía Docente para Revisión](/CasosDeUso/Actividades/Prototipos/README.md#profesor---enviar-guía)
| **Identificación de actores**      | Profesor |
|------------------------------------|----------|
| **Escenario**                      | El profesor envía la guía docente editada al Director de Grado para su revisión y posterior aprobación o rechazo, asegurándose de que cumpla con los estándares académicos y de calidad. |
| **Flujo de eventos principal**     | 1. El profesor inicia sesión en el sistema de gestión de guías.   <br> 2. El sistema muestra el menú principal con las guías asignadas.  <br>3. El profesor selecciona una guía a enviar.  <br> 4. El sistema despliega la guía seleccionada. <br> 5. El profesor selecciona la opción de enviar la guía para revisión.  <br>6. El sistema solicita confirmación del envío.  <br>7. El profesor confirma el envío.  <br>8. El sistema envía la guía al Director de Grado para revisión y muestra una notificación de éxito. |
| **Flujos alternativos y excepciones** | Si el profesor cancela el envío, el sistema regresa al menú principal sin enviar la guía.  <br> Si ocurre un error durante el envío (por ejemplo, falla en la conexión), el sistema notifica el error y permite reintentar. |
| **Precondiciones**                | El profesor debe haber iniciado sesión en el sistema y tener acceso a las guías asignadas.  <br> La guía debe estar completamente editada antes del envío. |
| **Postcondiciones**               | La guía queda marcada como "enviada para revisión" en el sistema, notificando al Director de Grado. |

![](/images/modelosUML/EnviarParaRevisionGD.svg)
