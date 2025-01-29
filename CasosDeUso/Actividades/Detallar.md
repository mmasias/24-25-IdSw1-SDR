<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |


</div>

# Casos de Uso Detallados

## Técnico de calidad


### [Generar Nueva Versión de la Guía](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---generar-nueva-versión)
![](/images/modelosUML/GenerarVersiónGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/GenerarVersionGD.puml)

### [Asignar Guías Docentes a Profesor](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---asignar-guía-a-profesor)
![](/images/modelosUML/AsignarProfesorGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/AsignarProfesorGD.puml)

### [Editar contenido estático de guía docente](/CasosDeUso/Actividades/Prototipos/README.md#técnico-de-calidad---editar-plantilla) ** cambiar a editar contenido estatico
![](/images/modelosUML/EditarContenidoEstaticoGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/EditarContenidoEstaticoGD.puml)




## Profesor

### 4. [Editar Contenido de la Guía](/CasosDeUso/Actividades/Prototipos/README.md#profesor---editar-guía)
| **Identificación de actores**      | Profesor |
|------------------------------------|----------|
| **Escenario**                      | El profesor accede al sistema para actualizar el contenido de la guía docente de una asignatura, con el fin de reflejar cambios en el temario, bibliografía, o metodologías de evaluación. |
| **Flujo de eventos principal**     | 1. El profesor inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes asignadas al profesor.<br> 3. El profesor selecciona una guía para editar.<br> 4. El sistema despliega el contenido actual de la guía.<br> 5. El profesor realiza las modificaciones necesarias en el contenido.<br> 6. El sistema guarda los cambios realizados y actualiza la guía. |
| **Flujos alternativos y excepciones** | Si el profesor desea descartar los cambios, el sistema permite cancelar la operación sin guardar.<br> Si se detecta un error en el contenido, el sistema muestra un mensaje indicando el problema antes de guardar. |
| **Precondiciones**                | El profesor debe tener acceso al sistema y permisos para editar la guía asignada. |
| **Postcondiciones**               | La guía queda actualizada con los cambios realizados, o se cancela la edición sin que se guarden modificaciones. |


![](/images/modelosUML/EditarContenidoGD.svg)  | [Ver Código](/CasosDeUso/Actividades/Detallados/EditarContenidoGD.puml)

## 13. [Enviar Guía Docente para Revisión](/CasosDeUso/Actividades/Prototipos/README.md#profesor---enviar-guía)
| **Identificación de actores**      | Profesor |
|------------------------------------|----------|
| **Escenario**                      | El profesor envía la guía docente editada al Director de Grado para su revisión y posterior aprobación o rechazo, asegurándose de que cumpla con los estándares académicos y de calidad. |
| **Flujo de eventos principal**     | 1. El profesor inicia sesión en el sistema de gestión de guías.   <br> 2. El sistema muestra el menú principal con las guías asignadas.  <br>3. El profesor selecciona una guía a enviar.  <br> 4. El sistema despliega la guía seleccionada. <br> 5. El profesor selecciona la opción de enviar la guía para revisión.  <br>6. El sistema solicita confirmación del envío.  <br>7. El profesor confirma el envío.  <br>8. El sistema envía la guía al Director de Grado para revisión y muestra una notificación de éxito. |
| **Flujos alternativos y excepciones** | Si el profesor cancela el envío, el sistema regresa al menú principal sin enviar la guía.  <br> Si ocurre un error durante el envío (por ejemplo, falla en la conexión), el sistema notifica el error y permite reintentar. |
| **Precondiciones**                | El profesor debe haber iniciado sesión en el sistema y tener acceso a las guías asignadas.  <br> La guía debe estar completamente editada antes del envío. |
| **Postcondiciones**               | La guía queda marcada como "enviada para revisión" en el sistema, notificando al Director de Grado. |

![](/images/modelosUML/EnviarParaRevisionGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/EnviarParaRevisionGD.puml)


## Director de grado

### 3. [Publicar Guía Docente](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---publicar-guía-docente)
-------------
| **Identificación de actores**      | Director de Grado |
|------------------------------------|-------------------|
| **Escenario**                      | El Director de Grado tiene la responsabilidad de autorizar la publicación final de las guías docentes, permitiendo que los estudiantes accedan a una versión oficial y aprobada de la guía. |
| **Flujo de eventos principal**     | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes aprobadas y listas para publicación.<br> 3. El Director de Grado selecciona una guía para publicar.<br> 4. El sistema solicita confirmación de la publicación final.<br> 5. El Director de Grado confirma la publicación.<br> 6. El sistema publica la guía, haciéndola accesible para los estudiantes a través del panel universitario. |
| **Flujos alternativos y excepciones** | Si el Director de Grado cancela la operación, el sistema retorna a la lista de guías sin realizar la publicación. |
| **Precondiciones**                | Acceso al sistema de gestión de guías docentes. La guía debe estar lista y aprobada para su publicación. |
| **Postcondiciones**               | La guía se publica y es accesible a los estudiantes, o la operación es cancelada sin cambios. |


![](/images/modelosUML/PublicarGD.svg)  | [Ver Código](/CasosDeUso/Actividades/Detallados/PublicarGD.puml)



### 5. [Revisar Contenido](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---revisar-contenido)

| **Identificación de actores**                          | **Director de Grado**                                                                 |
|--------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| **Escenario**                        | El Director de Grado revisa el contenido de una guía docente y decide si aprueba o rechaza su publicación, asegurando que cumple estándares académicos. |
| **Flujo de eventos principal**       | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías pendientes de aprobación.<br> 3. Selecciona una guía para revisar su contenido.<br> 4. El sistema despliega el contenido completo de la guía.<br> 5. Decide aprobar el contenido.<br> 6. El sistema marca la guía como aprobada y la prepara para publicación. |
| **Flujos alternativos y excepciones**| - Si el Director de Grado decide rechazar el contenido, el sistema permite registrar comentarios de retroalimentación y marca la guía como "Requiere Revisión".<br> - Si ocurre un error en la carga del contenido, el sistema notifica al Director de Grado y cancela la operación. |
| **Precondiciones**                   | - Acceso al sistema y a las guías pendientes de aprobación.<br> - El contenido debe estar completo y listo para revisión.                      |
| **Postcondiciones**                  | - La guía queda aprobada y lista para publicación.<br> - O se marca como "Requiere Revisión" con comentarios para ajustes.                      |

![](/images/modelosUML/RevisarContenidoGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/RevisarContenidoGD.puml)


### 8. [Ver listado de los estados de las guías por grado](/CasosDeUso/Actividades/Prototipos/README.md#director-de-grado---ver-listado-de-guías)
| **Identificación de actores**      | Director de Grado |
|------------------------------------|--------------------|
| **Escenario**                      | El Director de Grado solicita al sistema visualizar los estados en los que se encuentran las guías docentes de su grado, para asegurar la trazabilidad y gestionar adecuadamente el proceso de aprobación. |
| **Flujo de eventos principal**     | 1. El Director de Grado accede al sistema de gestión de guías.<br> 2. El sistema presenta el menú principal con las opciones disponibles.<br> 3. El Director de Grado selecciona la opción "Ver listado de estados de las guías de mi grado".<br> 4. El sistema visualiza una tabla con los siguientes datos para cada guía docente del grado:<br>&nbsp;&nbsp;&nbsp;&nbsp;- Título de la guía<br>&nbsp;&nbsp;&nbsp;&nbsp;- Estado actual (aprobado, devuelto para modificación, pendiente, etc.)<br>&nbsp;&nbsp;&nbsp;&nbsp;- Responsable actual<br>&nbsp;&nbsp;&nbsp;&nbsp;- Fecha de última modificación.<br> 5. El Director de Grado filtra o ordena la información según los criterios necesarios. |
| **Flujos alternativos y excepciones** | Si no hay guías registradas para el grado, el sistema muestra un mensaje indicando que no hay datos disponibles.<br> Si ocurre un error técnico al intentar cargar la información, el sistema notifica al Director de Grado y permite reintentar la operación. |
| **Precondiciones**                | El Director de Grado debe tener acceso al sistema y permisos para visualizar el listado de estados de las guías docentes de su grado correspondiente. |
| **Postcondiciones**               | El Director de Grado obtiene información actualizada sobre el estado de las guías docentes de su grado para realizar un seguimiento adecuado. |

![](/images/modelosUML/VerListadoEstadosGradoGD.svg)  | [Ver Código](/CasosDeUso/Actividades/Detallados/VerListadoEstadosGradoGD.puml)






## Director de calidad


### 1. [Verificar Cumplimiento con Memoria Verificada](/CasosDeUso/Actividades/Prototipos/README.md#dirección-de-calidad---verificar-cumplimiento-con-memoria-verificada)
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad debe verificar que las guías docentes se adhieren a la memoria verificada de la titulación, asegurando así el cumplimiento de los lineamientos institucionales. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de verificación.<br> 2. El sistema muestra la lista de guías docentes disponibles para verificación.<br> 3. La Dirección de Calidad selecciona una guía para verificar.<br> 4. El sistema utiliza la API de verificación para comparar la guía con la memoria verificada de la titulación.<br> 5. El sistema determina si la guía cumple con los requisitos de memoria verificada.<br> 6. El sistema notifica el resultado de la verificación a la Dirección de Calidad. |
| **Flujos alternativos y excepciones** | Si la guía no cumple con los requisitos, el sistema notifica a la Dirección de Calidad y permite enviar la guía para ajustes. |
| **Precondiciones**                | La Dirección de Calidad debe tener acceso al sistema y a la API de verificación, y la guía debe estar registrada en el sistema. |
| **Postcondiciones**               | El sistema confirma el cumplimiento de la guía con la memoria verificada o notifica las observaciones para ajustes. |

![](/images/modelosUML/VerificarGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/VerificarGD.puml)

### 2. [Auditar Guías Docentes](/CasosDeUso/Actividades/Prototipos/README.md#dirección-de-calidad---auditar-guías-docentes)
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad realiza auditorías exhaustivas de las guías docentes para evaluar la calidad del contenido y asegurar que cumplen con los objetivos académicos de la institución. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de auditoría.<br> 2. El sistema muestra la lista de guías docentes disponibles para auditar.<br> 3. La Dirección de Calidad selecciona una guía para revisar su contenido.<br> 4. El sistema despliega la guía seleccionada, permitiendo revisar secciones clave de contenido y alineación con los objetivos institucionales.<br> 5. La Dirección de Calidad realiza comentarios o solicitudes de ajuste, si aplica.<br> 6. El sistema guarda la auditoría y notifica que la revisión se ha completado. |
| **Flujos alternativos y excepciones** | Si se identifican problemas en la guía, el sistema permite a la Dirección de Calidad documentar observaciones y solicitar ajustes antes de aprobar la guía. |
| **Precondiciones**                | Acceso al sistema de auditoría y guías docentes disponibles para revisión. |
| **Postcondiciones**               | La auditoría se completa y se guarda, permitiendo que los ajustes se hagan antes de aprobar la guía. |


![](/images/modelosUML/AuditarGD.svg) | [Ver Código](/CasosDeUso/Actividades/Detallados/AuditarGD.puml)




