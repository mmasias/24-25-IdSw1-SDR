# Actores

| Diagrama | Código Fuente |
|----------|---------------|
| ![Actores](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/actores_evas.svg) | [Ver codigo](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Actores/Actores.puml) |

# Encontrar casos de uso 

| Diagrama | Código Fuente |
|----------|---------------|
| ![Casos de uso](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/CasosDeUso.svg) | [Ver codigo](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/a3de717ba0a3bb910f5f24562e45d251e74214d3/Documentos/CasosUso/CasosUso.puml) |

# Modelo de Casos de Uso como un Todo

Este modelo de casos de uso describe las funcionalidades y accesos del sistema en función de los diferentes tipos de usuarios. El sistema contempla tres tipos de usuarios registrados y uno no registrado, cada uno con acceso a distintos casos de uso según sus permisos y necesidades:

### Usuario No Registrado
Este actor representa a los visitantes que no tienen acceso completo al sistema. Su única funcionalidad disponible es **Registrarse**, lo cual les permite crear una cuenta y obtener el rol de **Alumno** para acceder a funcionalidades adicionales. Este mecanismo de registro es esencial para asegurar que las personas no accedan a funciones sin la debida autorización o verificación.

### Alumno
Este rol es para los usuarios registrados que participan en las actividades de aprendizaje del sistema. Los alumnos pueden iniciar sesión y realizar tareas como:
- **Ver Información de Asignaturas**
- **Consultar Calificaciones**
- **Usar Rutinas** asignadas por el profesor
- **Participar en Retos/Actividades**

Estas funcionalidades permiten a los alumnos interactuar con el contenido y seguir su progreso académico. La inclusión de retos o actividades adicionales ayuda a fomentar una experiencia de aprendizaje interactiva.

### Profesor
Este rol cuenta con permisos avanzados y permite la gestión directa de alumnos y asignaturas. Los profesores pueden realizar acciones de supervisión y evaluación, tales como:
- **Gestionar Alumnos**
- **Calificar Alumnos**
- **Impartir Asignatura**

Además, tienen la posibilidad de **Asignar Rutinas** y **Evaluar Progreso**, lo cual les proporciona herramientas para personalizar el aprendizaje de cada alumno y ajustar el contenido según su progreso.

### Admin
El administrador tiene el control total del sistema y puede realizar tareas esenciales de mantenimiento y configuración, tales como:
- **Administrar Usuarios** (gestión de permisos, creación o eliminación de cuentas)
- **Configurar Sistema** (ajustes globales)

Este rol garantiza el buen funcionamiento del sistema y asegura que solo usuarios autorizados accedan a funcionalidades críticas.

---

### Interacciones y Flujos Principales
El flujo del sistema comienza con el **Usuario No Registrado**, quien debe registrarse para obtener acceso a las funcionalidades. Una vez registrado, se convierte en **Alumno** y puede realizar tareas relacionadas con su aprendizaje. Los **Profesores**, por su parte, pueden monitorear y gestionar la experiencia educativa de los alumnos, ofreciendo una estructura guiada y personalizada. Finalmente, el **Admin** asegura que el sistema esté adecuadamente configurado y mantenido, permitiendo que todos los roles operen dentro de los límites de sus permisos.

# Diagrama de Contexto del Administrador
| Diagrama | Código Fuente |
|----------|---------------|

# Diagrama de Contexto del Alumno
| Diagrama | Código Fuente |
|----------|---------------|

# Diagrama de Contexto del Profesor
| Diagrama | Código Fuente |
|----------|---------------|

# Diagrama de Contexto del Usuario No Registrado
| Diagrama | Código Fuente |
|----------|---------------|
