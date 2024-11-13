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


### 5. Aprobar o Rechazar Contenido


### 6. Supervisar Guías Docentes


### 7. Generar Nueva Versión de la Guía


### 8. Utilizar Plantilla Multititulación


### 9. Asignar Guía a Titulación


### 10. Asignar Asignatura a Titulación

