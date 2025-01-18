[![Inicio](https://img.shields.io/badge/Inicio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main)
[![Modelo de Dominio](https://img.shields.io/badge/Modelo%20de%20Dominio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/modeloDelDominio)
[![Prototipos](https://img.shields.io/badge/Prototipos-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/prototipos)

## 🛠️ **Actores, Casos de Uso y Diagrama de Contexto**

### Actores
![Actores](https://github.com/srgiom/24-25-IdSw1-SDR/raw/main/casosDeUso/actores/actores.png)
> 🗂️ **Detalles:**
> Este diagrama muestra al actor principal del sistema: **el administrador**. Este rol incluye tareas clave como:
> - Gestionar aulas, asignaturas, profesores y estudiantes.
> - Control total sobre el sistema para garantizar su correcto funcionamiento.

---

### Casos de Uso


---

### Diagrama de Contexto
![Diagrama de Contexto](/casosDeUso/diagramaDeContexto/DiagramaDeContexto.svg)
> 🌐 **Contexto del Sistema:**
> Este diagrama presenta una vista general de las interacciones entre el sistema y los actores externos, resaltando las principales funcionalidades administradas por el usuario clave: el administrador.

---

## 🛠️ Casos de Uso Detallados

### Inicio de Sesión
![Inicio de Sesión](/casosDeUso/imagenes/IniciarSesión.svg)
> 🔒 **Ingreso:**
> Este diagrama ilustra el flujo de inicio de sesión:
> - El usuario ingresa sus credenciales.
> - El sistema valida la información:
>   - Si es válida, se muestra un mensaje de bienvenida.
>   - Si no, se notifica un error de "Credenciales incorrectas".

---

### Elegir Grado
![Elegir Grado](/casosDeUso/imagenes/ElegirGrado.svg)
> 🎓 **Selección de Grado:**
> Representa cómo el usuario elige un grado específico:
> - Se muestran todos los grados disponibles.
> - El usuario realiza su selección final.

---

### Registrar Asignatura
![Registrar Asignatura](/casosDeUso/imagenes/RegistrarAsignatura.svg)
> 📝 **Registro de Asignaturas:**
> Este diagrama detalla el registro manual o importación masiva de asignaturas mediante:
> - Introducción de datos manual.
> - Carga de archivos (Excel o CSV).
> - Validación de datos y confirmación.

---

### Asignar Profesor
![Asignar Profesor](/casosDeUso/imagenes/AsignarProfesor.svg)
> 👨‍🏫 **Asignación de Profesor:**
> Muestra el flujo para asignar un profesor a una asignatura. Incluye:
> - Verificación de que el profesor no exceda el límite de 8 asignaturas.
> - Confirmación o cancelación según corresponda.

---

### Consultar Horario de Profesor
![Consultar Horario de Profesor](/casosDeUso/imagenes/ConsultarHorarioProfesor.svg)
> 📅 **Consulta de Horario:**
> Permite visualizar el horario semanal de un profesor:
> - Detalles como asignaturas, horas y aulas ocupadas.
> - Presentación en un formato tabla claro y organizado.

---

### Editar Asignación
![Editar Asignación](/casosDeUso/imagenes/EditarAsignación.svg)
> ✏️ **Edición de Asignaciones:**
> Proceso que permite:
> - Modificar día, hora o aula.
> - Manejar errores si no hay aulas disponibles.
> - Confirmar los cambios realizados.

---

### Vincular Asignatura Horario
![Vincular Asignatura Horario](/casosDeUso/imagenes/VincularAsignaturaHorario.svg)
> 🔗 **Vinculación:**
> Este diagrama detalla cómo vincular una asignatura a un horario, evitando:
> - Conflictos de asignaciones.
> - Duplicidades en las horas asignadas.

---

### Mostrar Asignaturas
![Mostrar Asignaturas](/casosDeUso/imagenes/MostrarAsignaturas.svg)
> 📋 **Visualización:**
> Proporciona una lista filtrable de asignaturas:
> - Permite buscar por grado, profesor o nombre.
> - Opciones para visualizar todo o aplicar filtros.

---

### Ver Disponibilidad de Aulas
![Ver Disponibilidad de Aulas](/casosDeUso/imagenes/VerDisponibilidadDeAulas.svg)
> 🏫 **Consulta de Aulas:**
> El sistema permite consultar aulas disponibles aplicando filtros como:
> - Día y hora.
> - Tamaño (grande/pequeña).
> - Especificaciones (con computadoras).

---

### Seleccionar Aula Automáticamente
![Seleccionar Aula Automáticamente](/casosDeUso/imagenes/SeleccionarAulaAutomaticamente.svg)
> 🤖 **Automatización:**
> Detalla cómo se selecciona automáticamente un aula basada en:
> - Preferencias del usuario.
> - Disponibilidad general en el sistema.
