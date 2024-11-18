# Actores y Casos de uso

## Actores

1. **Cliente**
   El actor presente en este proyecto sería únicamente nuestro cliente ya que es la única persona que puede manipular el software para la hora de crear una nueva titulación, gestionar la carga de los profesores y todas las demás cuestiones que comprende el software a elaborar.

2. **Personas con las que se comparta el software**
   Este podría ser un actor en el caso futuro de que se le de acceso a este software a demás personas ya vea para visualizar simplemente la gestión que se lleva a cabo o poder realizar algún cambio, aunque como sugerencia esto se podría implementar a traves de la creación de roles en el software que tengan diferentes permisos y la creación de cuentas para poder tener acceso a la plataforma

## Casos de Uso

   Note: Los diagramas ya se cambian con respecto a la confirmación de los casos de uso

1. **CRUD con respecto al profesor**  
   - Corresponde a la creación de un profesor nuevo, actualizar a uno existente como podría ser la carga académica, eliminar un profesor si le han despedido y ver las estadísticas de un profesor (correspondiente al read)


   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso1](/images/modelosUML/CdU/CasoDeUso1.svg) | [Ver código](/modelosUML/CdU/CasoDeUso1.puml) |

2. **Crear Informe Anual**  
   - El Coordinador de Titulación genera un informe anual que resume los indicadores de calidad académica, tales como porcentaje de profesorado permanente, doctores acreditados y profesores en programas de movilidad.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso2](/images/modelosUML/CdU/CasoDeUso2.svg) | [Ver código](/modelosUML/CdU/CasoDeUso2.puml) |

3. **CRUD con respecto a las titulaciones**  
   - Corresponde con la creación de una nueva titulación, eliminar una nueva titulación, actualizarla por ejemplo con asignaturas que puedan cambiar y leer la titulación completa.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso3](/images/modelosUML/CdU/CasoDeUso3.svg) | [Ver código](/modelosUML/CdU/CasoDeUso3.puml) |

4. **Actualizar indicadores académicos**  
   - Proveer una funcionalidad para cargar datos actualizados en el sistema desde el Excel, ajustando indicadores clave relacionados con rendimiento académico, asignación docente y resultados por titulación

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso4](/images/modelosUML/CdU/CasoDeUso4.svg) | [Ver código](/modelosUML/CdU/CasoDeUso4.puml) |

5. **Notificar Cambios a los profesores**  
   - Generar notificaciones automáticas a los profesores cuando se realicen cambios en su asignación de carga académica o en las titulaciones relacionadas.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso5](/images/modelosUML/CdU/CasoDeUso5.svg) | [Ver código](/modelosUML/CdU/CasoDeUso5.puml) |