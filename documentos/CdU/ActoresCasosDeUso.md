# Actores y Casos de uso

## Actores

1. **Administrador Académico**  
   - Supervisar el cumplimiento de la carga académica de los profesores y actualizar los datos correspondientes en la hoja de cálculo.

2. **Coordinador de Titulación**  
   - Validar y ajustar la carga académica por titulación y coordinar la asignación de docentes en cada programa educativo.

3. **Profesor**  
   - Acceder a sus datos personales y de experiencia profesional para revisarlos o actualizarlos, incluyendo experiencia docente e investigadora.

4. **Personal de Recursos Humanos**  
   - Revisar, organizar y actualizar la información sobre la experiencia, temporalidad, y asignación principal de cada profesor.

5. **Analista de Indicadores**  
   - Consultar y extraer datos de la hoja de cálculo para generar informes y análisis de indicadores académicos y de recursos humanos.

## Casos de Uso

1. **Revisión de Carga Académica por Profesor**  
   - El Administrador Académico revisa y actualiza la carga de trabajo asignada a cada profesor para cada titulación. Esto incluye la verificación de horas semanales, contratos y dedicación a la docencia e investigación.
   
   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso1](/images/modelosUML/CdU/CasoDeUso1.svg) | [Ver código](/modelosUML/CasoDeUso1.puml) |

2. **Generación de Informe Anual de Mejora**  
   - El Coordinador de Titulación genera un informe anual que resume los indicadores de calidad académica, tales como porcentaje de profesorado permanente, doctores acreditados y profesores en programas de movilidad.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso2](/images/modelosUML/CdU/CasoDeUso2.svg) | [Ver código](/modelosUML/CasoDeUso2.puml) |

3. **Actualización de Datos de Profesorado**  
   - Los Profesores o el Personal de Recursos Humanos pueden modificar los datos de los docentes, incluyendo experiencia profesional, experiencia docente virtual, acreditación, y asignación de carga académica.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso3](/images/modelosUML/CdU/CasoDeUso3.svg) | [Ver código](/modelosUML/CasoDeUso3.puml) |

4. **Análisis de Indicadores Académicos**  
   - El Analista de Indicadores extrae datos para realizar análisis detallados, incluyendo indicadores como el porcentaje de profesorado permanente, número de doctores acreditados, y experiencia docente de los profesores.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso4](/images/modelosUML/CdU/CasoDeUso4.svg) | [Ver código](/modelosUML/CasoDeUso4.puml) |

5. **Consulta de Carga Total por Titulación**  
   - Los Coordinadores de Titulación pueden revisar y analizar la carga total asignada a cada titulación, permitiéndoles optimizar la distribución del personal docente en cada programa.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso5](/images/modelosUML/CdU/CasoDeUso5.svg) | [Ver código](/modelosUML/CasoDeUso5.puml) |