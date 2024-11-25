# Actores

| Diagrama | Código Fuente |
|----------|---------------|
| ![Actores](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/Actores/Actores.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Actores/Actores.puml) |

# Encontrar casos de uso 

| Diagrama | Código Fuente |
|----------|---------------|
| ![Casos de uso](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/CasosDeUso/CasosDeUso.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/CasosUso/CasosUso.puml) |

# Casos de uso detallados

## Usuario No Registrado
### Registrarse 
| Diagrama | Código Fuente |
|----------|---------------|
| ![Casos de uso](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DetallarCasosDeUso/Registrarse.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/DetallarCasosDeUso/Registrarse.puml) |

## Usuario 
### Iniciar Sesión 
| Diagrama | Código Fuente |
|----------|---------------|
| ![Casos de uso](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DetallarCasosDeUso/IniciarSesion.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/DetallarCasosDeUso/IniciarSesion.puml) |

### Cerrar Sesión 
| Diagrama | Código Fuente |
|----------|---------------|
| ![Casos de uso](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DetallarCasosDeUso/CerrarSesion.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/DetallarCasosDeUso/CerrarSesion.puml) |

## Funcionalidades Comunes (Alumno, Profesor, Admin)
### Iniciar Sesión (UC_IniciarSesion)
- **Actores**: Alumno, Profesor, Admin
- **Descripción**: Permite acceder a la página principal según el rol del usuario
- **Flujo Principal**: 
  1. El usuario introduce credenciales
  2. Accede a su página principal correspondiente

### Cerrar Sesión (UC_CerrarSesion)
- **Actores**: Alumno, Profesor, Admin
- **Descripción**: Finaliza la sesión del usuario
- **Flujo Principal**: 
  1. El usuario selecciona cerrar sesión
  2. Vuelve a la pantalla de inicio

### Volver al Inicio (UC_VolverInicio)
- **Actores**: Alumno, Profesor, Admin
- **Descripción**: Permite regresar a la página principal desde cualquier menú
- **Flujo Principal**: 
  1. Usuario selecciona "Volver página principal"
  2. Sistema muestra la página principal según rol

## Alumno
### Ver Clasificaciones (UC_VerClasificaciones)
- **Descripción**: Acceso al menú de clasificación
- **Flujo Principal**:
  1. Accede al MENU_CLASIFICACION desde página principal
  2. Visualiza las clasificaciones
  3. Puede volver a la página principal

### Usar Rutinas (UC_UsarRutinas)
- **Descripción**: Acceso al menú de rutinas
- **Flujo Principal**:
  1. Accede al MENU_RUTINAS
  2. Puede realizar cualquier rutina
  3. Vuelve al menú de rutinas o página principal

### Completar Retos Obligatorios (UC_CompletarRetosObligatorios)
- **Descripción**: Participación en retos obligatorios
- **Flujo Principal**:
  1. Accede al MENU_RETOS
  2. Selecciona RETOS_OBLIGATORIOS
  3. Completa el reto
  4. Vuelve al menú de retos

### Completar Retos Opcionales (UC_CompletarRetosOpcionales)
- **Descripción**: Participación en retos opcionales
- **Flujo Principal**:
  1. Accede al MENU_RETOS
  2. Selecciona RETOS_OPCIONALES
  3. Completa el reto si lo desea
  4. Vuelve al menú de retos

### Inscribirse en Clases (UC_InscribirseClases)
- **Descripción**: Proceso de inscripción en clases
- **Flujo Principal**:
  1. Accede al MENU_PERFIL
  2. Selecciona INSCRIPCION_CLASE
  3. Realiza la inscripción
  4. Vuelve al perfil

### Utilizar QR para Centros Deportivos (UC_UsarQR)
- **Descripción**: Uso de códigos QR para acceso
- **Flujo Principal**:
  1. Accede al MENU_PERFIL
  2. Selecciona QR_CENTROS_DEPORTIVOS
  3. Utiliza el código QR para poder acceder al centro deseado
  4. Vuelve al perfil

## Profesor
### Crear Nuevas Rutinas (UC_CrearRutinas)
- **Descripción**: Creación de rutinas para alumnos
- **Flujo Principal**:
  1. Accede al MENU_RUTINAS
  2. Selecciona CREAR_RUTINAS
  3. Crea la rutina
  4. Vuelve al menú de rutinas

### Crear Retos Obligatorios (UC_CrearRetosObligatorios)
- **Descripción**: Creación de retos obligatorios
- **Flujo Principal**:
  1. Accede al MENU_RETOS
  2. Selecciona RETOS_OBLIGATORIOS
  3. Crea y valida el reto obligatorio
  4. Vuelve al menú de retos

### Crear Retos Opcionales (UC_CrearRetosOpcionales)
- **Descripción**: Creación de retos opcionales
- **Flujo Principal**:
  1. Accede al MENU_RETOS
  2. Selecciona RETOS_OPCIONALES
  3. Crea y valida el reto opcional
  4. Vuelve al menú de retos

### Ver Clases y Alumnos (UC_VerClasesAlumnos)
- **Descripción**: Visualización de clases y alumnos asignados
- **Flujo Principal**:
  1. Accede al MENU_PERFIL
  2. Selecciona CLASES
  3. Visualiza información
  4. Vuelve al perfil

## Administrador
### Administrar Usuarios (UC_AdministrarUsuarios)
- **Descripción**: Gestión completa de usuarios
- **Flujo Principal**:
  1. Accede al MENU_USUARIOS
  2. Puede crear, modificar, eliminar o consultar usuarios
  3. Vuelve al inicio

### Gestionar Clases (UC_GestionarClases)
- **Descripción**: Administración de clases
- **Flujo Principal**:
  1. Accede desde página principal
  2. Gestiona las clases
  3. Vuelve al inicio

### Gestionar Rutinas (UC_GestionarRutinas)
- **Descripción**: Administración de rutinas
- **Flujo Principal**:
  1. Accede al MENU_RUTINAS
  2. Puede crear, modificar, eliminar o consultar rutinas
  3. Puede modificar batería de ejercicios
  4. Vuelve al inicio

### Gestionar Retos (UC_GestionarRetos)
- **Descripción**: Administración de retos
- **Flujo Principal**:
  1. Accede al MENU_RETOS
  2. Puede modificar o eliminar retos
  3. Vuelve al inicio

### Administrar Asignaturas (UC_AdministrarAsignaturas)
- **Descripción**: Gestión de asignaturas
- **Flujo Principal**:
  1. Accede desde página principal
  2. Administra las asignaturas
  3. Vuelve al inicio

### Configuración del Sistema (UC_ConfigurarSistema)
- **Descripción**: Configuración general del sistema
- **Flujo Principal**:
  1. Accede al MENU_CONFIGURACION
  2. Puede configurar sistema, administrar permisos y ajustes generales
  3. Vuelve al inicio

### Ver Reportes (UC_VerReportes)
- **Descripción**: Visualización de reportes
- **Flujo Principal**:
  1. Accede al MENU_REPORTES
  2. Consulta reportes
  3. Vuelve al inicio

### Descargar Estadísticas (UC_DescargarEstadisticas)
- **Descripción**: Exportación de estadísticas
- **Flujo Principal**:
  1. Accede al MENU_REPORTES
  2. Selecciona descargar estadísticas
  3. Vuelve al inicio

---

# Diagrama de Contexto del Administrador
| Diagrama | Código Fuente |
|----------|---------------|
| ![Modelo de Contexto Alumno](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DiagramasContexto/AdminContexto.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/ModeloDeContexto/AdministradorContexto.puml) |

# Diagrama de Contexto del Alumno
| Diagrama | Código Fuente |
|----------|---------------|
| ![Modelo de Contexto Alumno](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DiagramasContexto/AlumnoContexto.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/ModeloDeContexto/AlumnosContexto.puml) |

# Diagrama de Contexto del Profesor
| Diagrama | Código Fuente |
|----------|---------------|
| ![Profesores](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DiagramasContexto/ProfesorContexto.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/ModeloDeContexto/ProfesorContexto.puml) |

# Diagrama de Contexto del Usuario No Registrado
| Diagrama | Código Fuente |
|----------|---------------|
| ![Usuario No Registrado](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/Imagenes/DiagramasContexto/UsuarioNoRegistradoContexto.svg) | [Ver código](https://github.com/celiabecerril/24-25-IdSw1-SDR/blob/main/Documentos/ModeloDeContexto/UsuarioNoRegistradoContexto.puml) |

