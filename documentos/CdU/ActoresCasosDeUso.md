# Actores y Casos de uso

## Actores

| **Cliente**                                                                                           | **Personas con las que se comparte el software**                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| El actor presente en este proyecto sería únicamente nuestro cliente, ya que es la única persona que puede manipular el software para crear una nueva titulación, gestionar la carga de los profesores y todas las demás cuestiones que comprende el software a elaborar. | Este podría ser un actor en el caso futuro de que se le dé acceso a este software a otras personas, ya sea para visualizar la gestión que se lleva a cabo o para realizar algún cambio. Se podría implementar mediante la creación de roles con permisos distintos, así como la creación de cuentas para gestionar el acceso a la plataforma. |

---

## Casos de Uso


### **Revisión de Carga Académica por Profesor**  
   - El Administrador Académico revisa y actualiza la carga de trabajo asignada a cada profesor para cada titulación. Esto incluye la verificación de horas semanales, contratos y dedicación a la docencia e investigación.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso1](/images/modelosUML/CdU/CasoDeUso1.svg) | [Ver código](/modelosUML/CdU/CasoDeUso1.puml) |

### **Generación de Informe Anual de Mejora**  
   - El Coordinador de Titulación genera un informe anual que resume los indicadores de calidad académica, tales como porcentaje de profesorado permanente, doctores acreditados y profesores en programas de movilidad.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso2](/images/modelosUML/CdU/CasoDeUso2.svg) | [Ver código](/modelosUML/CdU/CasoDeUso2.puml) |

### 3. **Actualización de Datos de Profesorado**  
   - Los Profesores o el Personal de Recursos Humanos pueden modificar los datos de los docentes, incluyendo experiencia profesional, experiencia docente virtual, acreditación, y asignación de carga académica.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso3](/images/modelosUML/CdU/CasoDeUso3.svg) | [Ver código](/modelosUML/CdU/CasoDeUso3.puml) |

### 4. **Análisis de Indicadores Académicos**  
   - El Analista de Indicadores extrae datos para realizar análisis detallados, incluyendo indicadores como el porcentaje de profesorado permanente, número de doctores acreditados, y experiencia docente de los profesores.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso4](/images/modelosUML/CdU/CasoDeUso4.svg) | [Ver código](/modelosUML/CdU/CasoDeUso4.puml) |

### 5. **Consulta de Carga Total por Titulación**  
   - Los Coordinadores de Titulación pueden revisar y analizar la carga total asignada a cada titulación, permitiéndoles optimizar la distribución del personal docente en cada programa.

   | **Diagrama** | **Código Fuente** |
   |--------------|--------------------|
   | ![CasoDeUso5](/images/modelosUML/CdU/CasoDeUso5.svg) | [Ver código](/modelosUML/CdU/CasoDeUso5.puml) |
