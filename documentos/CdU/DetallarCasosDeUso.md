# 📝 Detallar Casos de Uso

---

### 1. Crear un Profesor

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | El departamento tiene acceso al sistema. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📝 El sistema solicita la información del profesor (nombre, titulaciones, categoría, experiencia, etc.).<br> 3. ✍️ El departamento ingresa los datos y envía el formulario.<br> 4. ✅ El sistema valida los datos ingresados.<br> 5. 💾 El sistema registra al profesor en la base de datos.<br> 6. ✔️ El sistema confirma que el profesor ha sido creado correctamente. |
| **Flujos Alternativos** | ⚠️ Si los datos ingresados son incorrectos, el sistema muestra un mensaje de error y permite corregir. |

---

### 2. Crear Asignatura

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | Acceso al sistema y datos necesarios para crear una asignatura. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📝 El sistema solicita la información de la asignatura (nombre, semestre, ECTS, tipo).<br> 3. ✍️ El departamento ingresa los datos y confirma.<br> 4. ✅ El sistema valida y registra la asignatura.<br> 5. ✔️ El sistema confirma que la asignatura ha sido creada. |
| **Flujos Alternativos** | ⚠️ Si la asignatura ya existe, el sistema notifica y permite editarla. |

---

### 3. Crear Contrato para un Profesor

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | Acceso al sistema y datos necesarios para crear un contrato. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📝 El sistema solicita los datos del contrato (tipo de contrato, duración, condiciones).<br> 3. ✍️ El departamento ingresa los datos y confirma.<br> 4. ✅ El sistema valida los datos y crea el contrato asociado al profesor.<br> 5. ✔️ El sistema confirma que el contrato ha sido creado correctamente. |
| **Flujos Alternativos** | ⚠️ Si el tipo de contrato no es compatible con la carga docente, el sistema muestra un mensaje de error. |

---

### 4. Registrar Memoria Académica

| **Actor Primario** | Memoria Académica |
|--------------------|-------------------|
| **Precondiciones** | El sistema tiene acceso a los datos académicos de asignaturas y profesores. |
| **Flujo Principal** | 1. 📤 El sistema recibe los datos académicos de las asignaturas y profesores.<br> 2. ✅ El sistema verifica la validez de los datos recibidos.<br> 3. 💾 El sistema registra la información en la memoria académica.<br> 4. ✔️ El sistema confirma que la memoria académica ha sido actualizada. |
| **Flujos Alternativos** | ⚠️ Si los datos son incompletos o incorrectos, el sistema muestra un mensaje de error y solicita corrección. |

--- 

### 5. Consultar Información de un Profesor

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | El departamento tiene acceso al sistema y a los datos del profesor. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📄 El sistema muestra una lista de los profesores registrados.<br> 3. 🔍 El departamento selecciona un profesor para consultar.<br> 4. ℹ️ El sistema muestra la información detallada del profesor (titulación, categoría, experiencia, asignaturas, etc.). |
| **Flujos Alternativos** | ⚠️ Si no hay resultados para el profesor seleccionado, el sistema muestra un mensaje indicando que no se han encontrado coincidencias. |

--- 

### 6. Modificar Información de una Asignatura

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | El departamento tiene acceso al sistema y los datos de la asignatura. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📄 El sistema muestra la lista de asignaturas registradas.<br> 3. ✍️ El departamento selecciona una asignatura para editar.<br> 4. ℹ️ El sistema muestra los datos actuales de la asignatura.<br> 5. 🔄 El departamento modifica la información (por ejemplo, semestre, ECTS) y confirma.<br> 6. ✔️ El sistema valida los cambios y actualiza la asignatura. |
| **Flujos Alternativos** | ⚠️ Si los cambios no son válidos (por ejemplo, asignación incorrecta de ECTS), el sistema muestra un mensaje de error y permite corrección. |

--- 

### 7. Eliminar un Profesor

| **Actor Primario** | Departamento |
|--------------------|--------------|
| **Precondiciones** | El departamento tiene acceso al sistema y al registro del profesor. |
| **Flujo Principal** | 1. 🔐 El departamento inicia sesión en el sistema.<br> 2. 📄 El sistema muestra la lista de profesores registrados.<br> 3. ❌ El departamento selecciona el profesor que desea eliminar.<br> 4. ⚠️ El sistema muestra una confirmación de eliminación.<br> 5. ✅ El departamento confirma la eliminación.<br> 6. 🗑️ El sistema elimina al profesor del registro. |
| **Flujos Alternativos** | ⚠️ Si el profesor está asociado a asignaturas o contratos activos, el sistema muestra un mensaje de advertencia y requiere que el departamento revise dichas asociaciones antes de proceder con la eliminación. |
