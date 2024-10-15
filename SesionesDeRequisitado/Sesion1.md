# Sesión de requisitado #1
Fecha: 16 de octubre, 2024

Antes de la reunion: 
## Preguntas clave para la reunión:
### Sobre el proceso actual:

¿Cómo es el proceso actual para crear, mantener y actualizar las guías docentes?

¿Quiénes son los responsables de esta tarea actualmente?

¿Qué herramientas o plataformas usan para gestionarlas?

¿Con qué frecuencia se deben actualizar las guías? 

¿Qué cambios se hacen típicamente cada año?

### Sobre las necesidades del sistema:

¿Qué partes de la guía deben actualizarse automáticamente y cuáles necesitan intervención humana?

¿Existen reglas o plantillas comunes que se puedan automatizar?

¿Es necesario integrar el sistema con otras plataformas, como sistemas de gestión de aprendizaje (LMS), bases de datos de 
currículos o sistemas de administración académica? Ejemplo, panal moodle. 

¿El sistema deberá enviar recordatorios o notificaciones cuando sea necesario realizar una actualización manual?

### Usuarios del sistema:

¿Quiénes interactuarán con el sistema? (Por ejemplo: coordinadores académicos, profesores, administrativos, directores de grado, etc.)

¿Habrá diferentes niveles de acceso para distintos tipos de usuarios?

### Requisitos funcionales específicos:

¿Cómo espera el cliente (Jorge Crespo) que se automatice la actualización anual de las guías? 

¿Se basará en datos previos o será necesario agregar nuevas fuentes de información cada año?

¿Desean incluir un proceso de aprobación para los cambios en las guías antes de que se publiquen?

¿Qué tan personalizables deben ser las guías para adaptarse a diferentes cursos o programas?

### Requisitos no funcionales:

¿Existen requisitos específicos sobre la interfaz de usuario? 

¿Qué tan intuitivo debe ser el sistema para usuarios con diferentes niveles de habilidad tecnológica?

¿Cuáles son las expectativas de tiempo de respuesta y rendimiento del sistema, especialmente en épocas de alta demanda (como el inicio de semestre)?

¿Hay alguna limitación técnica o preferencia de tecnología que tenga en mente?

### Alcance del proyecto:

¿Este proyecto está enfocado solo en automatizar las guías docentes, o se prevén futuras funcionalidades adicionales (por ejemplo, generación de informes, análisis de uso)?

¿Qué tan flexible debe ser el sistema para adaptarse a cambios en las regulaciones académicas o las políticas internas?

## Posibles clases conceptuales para el modelo de dominio:
Con base en la problemática planteada, podemos comenzar a identificar algunas clases clave que representen los elementos más importantes del dominio. Estas clases podrían incluir:

- GuíaDocente:
    - Atributos: nombre, año, estado, fechaUltimaActualización, contenido
    - Métodos: actualizarContenido(), validarGuía(), publicar()

- Usuario:
    - Atributos: nombre, rol (profesor, coordinador, administrativo, directorDeGrado), email, contraseña
    - Métodos: editarGuía(), aprobarGuía(), recibirNotificaciones()

- PlantillaGuía:
    - Atributos: nombre, estructura, version
    - Métodos: crearNuevaPlantilla(), actualizarPlantilla(), asociarConGuía()

- Curso:
    - Atributos: nombreCurso, codigoCurso, coordinador, duración
    - Métodos: asignarGuíaDocente(), actualizarDatosCurso()

- HistorialActualizaciones:
    - Atributos: fechaActualización, usuarioResponsable, cambiosRealizados
    - Métodos: registrarCambio(), consultarHistorial()

- Notificación:
    - Atributos: mensaje, destinatario, tipoNotificación, fechaEnvio
    - Métodos: enviarNotificación(), programarNotificación()

- SistemaExterno (LMS, Sistema de Gestión Académica):
    - Atributos: nombre, tipo, API
    - Métodos: integrarConSistema(), actualizarDatos()
