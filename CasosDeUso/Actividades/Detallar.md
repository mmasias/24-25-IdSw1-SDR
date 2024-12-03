# Casos de Uso Detallados

### 1. Verificar Cumplimiento con Memoria Verificada
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad debe verificar que las guías docentes se adhieren a la memoria verificada de la titulación, asegurando así el cumplimiento de los lineamientos institucionales. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de verificación.<br> 2. El sistema muestra la lista de guías docentes disponibles para verificación.<br> 3. La Dirección de Calidad selecciona una guía para verificar.<br> 4. El sistema utiliza la API de verificación para comparar la guía con la memoria verificada de la titulación.<br> 5. El sistema determina si la guía cumple con los requisitos de memoria verificada.<br> 6. El sistema notifica el resultado de la verificación a la Dirección de Calidad. |
| **Flujos alternativos y excepciones** | Si la guía no cumple con los requisitos, el sistema notifica a la Dirección de Calidad y permite enviar la guía para ajustes. |
| **Precondiciones**                | La Dirección de Calidad debe tener acceso al sistema y a la API de verificación, y la guía debe estar registrada en el sistema. |
| **Postcondiciones**               | El sistema confirma el cumplimiento de la guía con la memoria verificada o notifica las observaciones para ajustes. |

![](/images/modelosUML/VerificarGD.svg)

### 2. Auditar Guías Docentes
-------------
| **Identificación de actores**      | Dirección de Calidad |
|------------------------------------|----------------------|
| **Escenario**                      | La Dirección de Calidad realiza auditorías exhaustivas de las guías docentes para evaluar la calidad del contenido y asegurar que cumplen con los objetivos académicos de la institución. |
| **Flujo de eventos principal**     | 1. La Dirección de Calidad inicia sesión en el sistema de auditoría.<br> 2. El sistema muestra la lista de guías docentes disponibles para auditar.<br> 3. La Dirección de Calidad selecciona una guía para revisar su contenido.<br> 4. El sistema despliega la guía seleccionada, permitiendo revisar secciones clave de contenido y alineación con los objetivos institucionales.<br> 5. La Dirección de Calidad realiza comentarios o solicitudes de ajuste, si aplica.<br> 6. El sistema guarda la auditoría y notifica que la revisión se ha completado. |
| **Flujos alternativos y excepciones** | Si se identifican problemas en la guía, el sistema permite a la Dirección de Calidad documentar observaciones y solicitar ajustes antes de aprobar la guía. |
| **Precondiciones**                | Acceso al sistema de auditoría y guías docentes disponibles para revisión. |
| **Postcondiciones**               | La auditoría se completa y se guarda, permitiendo que los ajustes se hagan antes de aprobar la guía. |


![](/images/modelosUML/AuditarGD.svg)

### 3. Publicar Guía Docente
-------------
| **Identificación de actores**      | Director de Grado |
|------------------------------------|-------------------|
| **Escenario**                      | El Director de Grado tiene la responsabilidad de autorizar la publicación final de las guías docentes, permitiendo que los estudiantes accedan a una versión oficial y aprobada de la guía. |
| **Flujo de eventos principal**     | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes aprobadas y listas para publicación.<br> 3. El Director de Grado selecciona una guía para publicar.<br> 4. El sistema solicita confirmación de la publicación final.<br> 5. El Director de Grado confirma la publicación.<br> 6. El sistema publica la guía, haciéndola accesible para los estudiantes a través del panel universitario. |
| **Flujos alternativos y excepciones** | Si el Director de Grado cancela la operación, el sistema retorna a la lista de guías sin realizar la publicación. |
| **Precondiciones**                | Acceso al sistema de gestión de guías docentes. La guía debe estar lista y aprobada para su publicación. |
| **Postcondiciones**               | La guía se publica y es accesible a los estudiantes, o la operación es cancelada sin cambios. |


![](/images/modelosUML/PublicarGD.svg) 

### 4. Editar Contenido de la Guía
| **Identificación de actores**      | Profesor |
|------------------------------------|----------|
| **Escenario**                      | El profesor accede al sistema para actualizar el contenido de la guía docente de una asignatura, con el fin de reflejar cambios en el temario, bibliografía, o metodologías de evaluación. |
| **Flujo de eventos principal**     | 1. El profesor inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes asignadas al profesor.<br> 3. El profesor selecciona una guía para editar.<br> 4. El sistema despliega el contenido actual de la guía.<br> 5. El profesor realiza las modificaciones necesarias en el contenido.<br> 6. El sistema guarda los cambios realizados y actualiza la guía. |
| **Flujos alternativos y excepciones** | Si el profesor desea descartar los cambios, el sistema permite cancelar la operación sin guardar.<br> Si se detecta un error en el contenido, el sistema muestra un mensaje indicando el problema antes de guardar. |
| **Precondiciones**                | El profesor debe tener acceso al sistema y permisos para editar la guía asignada. |
| **Postcondiciones**               | La guía queda actualizada con los cambios realizados, o se cancela la edición sin que se guarden modificaciones. |


![](/images/modelosUML/EditarContenidoGD.svg)

### 5. Revisar Contenido
| **Identificación de actores**      | Director de Grado |
|------------------------------------|-------------------|
| **Escenario**                      | El Director de Grado revisa el contenido de una guía docente y decide si aprueba o rechaza su publicación, asegurando que el material cumple con los estándares académicos establecidos. |
| **Flujo de eventos principal**     | 1. El Director de Grado inicia sesión en el sistema de gestión de guías.<br> 2. El sistema muestra la lista de guías docentes pendientes de aprobación.<br> 3. El Director de Grado selecciona una guía para revisar su contenido.<br> 4. El sistema despliega el contenido completo de la guía para su revisión.<br> 5. El Director de Grado elige aprobar el contenido.<br> 6. El sistema marca la guía como aprobada y la prepara para publicación. |
| **Flujos alternativos y excepciones** | Si el Director de Grado decide rechazar el contenido, el sistema permite registrar comentarios de retroalimentación para el profesor y marca la guía como "Requiere Revisión".<br> Si ocurre un error en la carga del contenido, el sistema notifica al Director de Grado y cancela la operación. |
| **Precondiciones**                | Acceso al sistema y a las guías pendientes de aprobación. El contenido debe estar completo y listo para revisión. |
| **Postcondiciones**               | La guía queda aprobada y lista para publicación, o se marca como "Requiere Revisión" con comentarios para ajustes. |


![](/images/modelosUML/RevisarContenidoGD.svg)

### 6. Generar Nueva Versión de la Guía
| **Identificación de actores**      | Técnico de Calidad |
|------------------------------------|--------------------|
| **Escenario**                      | El Técnico de Calidad solicita al sistema la creación de una nueva versión de una guía docente para registrar cambios recientes en el contenido y mantener un historial de versiones. |
| **Flujo de eventos principal**     | 1. El Técnico de Calidad accede al sistema de gestión de versiones de guías.<br> 2. El sistema muestra la lista de guías con opción de crear nueva versión.<br> 3. El Técnico de Calidad selecciona una guía y solicita generar una nueva versión.<br> 4. El sistema crea una nueva versión de la guía, basada en el contenido existente.<br> 5. El Técnico de Calidad confirma la creación de la nueva versión.<br> 6. El sistema guarda la nueva versión y la marca como la versión activa. |
| **Flujos alternativos y excepciones** | Si ocurre un error durante la generación de la nueva versión, el sistema notifica al Técnico de Calidad y permite reintentar o cancelar la operación. |
| **Precondiciones**                | El técnico debe tener acceso al sistema de gestión de versiones y permisos para generar nuevas versiones de las guías. |
| **Postcondiciones**               | Una nueva versión de la guía queda registrada y disponible para futuras ediciones o revisiones. |


![](/images/modelosUML/GenerarVersiónGD.svg)

### 7. Ver listado de los estados de las guías docentes

### 8. Ver listado de los estados de las guías por grado

### 9. Editar plantilla de la guía docente

### 10. Utilizar Plantilla Multititulación

### 11. Asignar Guía a Titulación

### 12. Asignar Asignatura a Titulación

### 12. Asignar Asignatura a Titulación

### 13. Asignar Guías Docentes a Profesor
