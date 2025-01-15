[![Inicio](https://img.shields.io/badge/Inicio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main)
[![Modelo de Dominio](https://img.shields.io/badge/Modelo%20de%20Dominio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/modeloDelDominio)
[![Prototipos](https://img.shields.io/badge/Prototipos-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/prototipos)

## 🛠️ **Actores y Diagrama de Contexto**

### Actores
![Actores](https://github.com/srgiom/24-25-IdSw1-SDR/raw/main/casosDeUso/actores/actores.png)
> 🗂️ **Detalles:**
> Este diagrama muestra al actor principal del sistema: **el administrador**. Este rol incluye tareas clave como:
> - Gestionar aulas, asignaturas, profesores y estudiantes.
> - Control total sobre el sistema para garantizar su correcto funcionamiento.

---


### Diagrama de Contexto
![Diagrama de Contexto](/casosDeUso/diagramaDeContexto/DiagramaDeContexto.svg)
> 🌐 **Contexto del Sistema:**
> Este diagrama presenta una vista general de las interacciones entre el sistema y los actores externos, resaltando las principales funcionalidades administradas por el usuario clave: el administrador.

---

## 🛠️ Casos de Uso Representados mediante Diagramas (Ordenados)

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

### Vincular Asignatura Horario
![Vincular Asignatura Horario](/casosDeUso/imagenes/VincularAsignaturaHorario.svg)

### Mostrar Asignaturas
![Mostrar Asignaturas](/casosDeUso/imagenes/MostrarAsignaturas.svg)

### Ver Disponibilidad de Aulas
![Ver Disponibilidad de Aulas](/casosDeUso/imagenes/VerDisponibilidadDeAulas.svg)

### Seleccionar Aula Automáticamente
![Seleccionar Aula Automáticamente](/casosDeUso/imagenes/SeleccionarAulaAutomaticamente.svg)
