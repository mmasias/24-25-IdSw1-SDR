# Caso de Uso - Actualizar Datos del Usuario

|![Diagrama de Clases](/documentos/imagenes/casos_de_uso/usuario/actualizar_datos_usuario.svg)|[Código](/casos_de_uso/casos_de_uso/usuarios/actualizar_datos_usuario/actualizar_datos.puml)|
|---|---|

# Caso de Uso: Actualizar datos del Usuario

## Actor Principal
Usuario (incluye Becarios PROFER).

## Propósito
Permitir al usuario actualizar su información personal en el sistema.

---

## Flujo Principal
1. El usuario selecciona la opción para actualizar datos.
2. El sistema solicita los siguientes datos:
   - **Datos generales:** Foto, nombre, apellido, fecha de nacimiento, email, contraseña.
   - **Solo Becarios PROFER:** Dirección, teléfono, año de ingreso.
3. El usuario introduce los datos solicitados.
4. El sistema valida los datos:
   - **Si son correctos:** Los guarda y muestra un mensaje de confirmación.
   - **Si contienen errores:** Muestra un mensaje de error y permite corregirlos.
5. El sistema regresa a la pantalla de configuración.

---

## Reglas
1. Los campos obligatorios deben completarse.
2. Los datos deben tener el formato correcto.

---

## Precondiciones
1. El usuario debe estar autenticado.

---

## Postcondiciones
1. Los datos actualizados se almacenan correctamente.
