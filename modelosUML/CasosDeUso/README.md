# Identificación y Priorización de Actores y Casos de Uso

## 1. Identificar Actores y Casos de Uso

### Actores
- **Administrador**: Actor clave para la gestión y validación de ofertas de trabajo.
- **Alumni**: Usuario que interactúa con la plataforma para buscar y postular a ofertas.
- **Empresa**: Protagonista en la creación, modificación y cierre de ofertas.

### Casos de Uso
1. **Crear oferta de trabajo** *(Empresa)*: La empresa solicita registrar una nueva oferta en el sistema.
2. **Buscar oferta de trabajo** *(Alumni)*: Los alumni pueden buscar ofertas que coincidan con sus intereses.
3. **Aceptar oferta de trabajo** *(Administrador)*: El administrador valida las ofertas creadas para que sean públicas.
4. **Postular para la oferta de trabajo** *(Alumni)*: Los alumni pueden enviar su solicitud para una oferta de trabajo específica.
5. **Cerrar oferta de trabajo** *(Administrador, Empresa)*: Una oferta se finaliza porque ya no está disponible.
6. **Cancelar oferta de trabajo** *(Administrador)*: El administrador cancela una oferta de trabajo.

---

## 2. Priorizar Casos de Uso

La prioridad debe basarse en su importancia estratégica, valor para el cliente, complejidad, riesgo... En este caso, se priorizan los casos de uso según su relevancia para el funcionamiento básico del sistema.

1. **Crear oferta de trabajo** *(Alta prioridad)*  
   Es el primer paso en el flujo de trabajo; sin ofertas, el sistema no tiene utilidad.

2. **Buscar oferta de trabajo** *(Alta prioridad)*  
   Es la función principal para los alumni y uno de los puntos más críticos de la plataforma.

3. **Postular para la oferta de trabajo** *(Media/Alta prioridad)*  
   Una vez que las ofertas están disponibles, esta funcionalidad permite que los alumni interactúen activamente con el sistema.

4. **Aceptar oferta de trabajo** *(Media prioridad)*  
   La validación de ofertas es importante, pero depende del flujo de creación de ofertas.

5. **Cerrar oferta de trabajo** *(Media prioridad)*  
   Su importancia varía dependiendo de la actividad en la plataforma.

6. **Cancelar oferta de trabajo** *(Baja prioridad)*  
   Este caso de uso se activa en escenarios específicos, pero no es central en el funcionamiento básico del sistema.

## 3. Detallar casos de uso

Para cada caso de uso, se completa una plantilla con la información esencial.

### Crear oferta de trabajo:

1. Identificación de los actores
   Actor Principal: Empresa
   Actor Secundario: Administrador (recibe notificación para validar la oferta)

2. Definición del escenario
   La empresa desea publicar una nueva oferta de trabajo en la plataforma. Para ello, acceda al sistema, llene el formulario con los datos necesarios y envíe la solicitud. La oferta queda registrada en el sistema con el estado "Pendiente de Validación" y el administrador es notificado para revisarla.

3. Documentación del flujo de eventos principales
    1. La empresa inicia sesión en la plataforma.
    2. Accede a la sección "Crear oferta de trabajo".
    3. Llena los campos requeridos del formulario, que incluyen:
    4. Título de la oferta.
    5. Descripción.
    6. Requisitos.
    7. Duración o vigencia de la oferta.
    8. Ubicación (opcional).
    9. Presiona el botón "Guardar".
    10. El sistema valida que todos los campos obligatorios estén completos.
    11. El sistema guarda la oferta como "Pendiente de Validación".
    12. El administrador recibe una notificación para revisar la oferta.

4. Especificación de flujos alternativos y excepciones
   Datos incompletos:
   La empresa intenta guardar la oferta sin completar todos los campos obligatorios.
   La empresa corrige los errores y vuelve a intentar.
   Autenticación fallida:
   La empresa no tiene una sesión activa o intenta acceder al formulario sin autenticarse.
   El sistema redirige a la página de inicio de sesión.

5. Precondiciones y postcondiciones:

   Precondiciones:

   La empresa debe estar registrada y autenticada en la plataforma.
   Deben existir reglas de negocio claras para validar los datos ingresados.

   Postcondiciones:

   La oferta queda registrada con el estado "Pendiente de Validación".
   El administrador es notificado sobre la nueva oferta.

6. Requisitos especiales
   Restricciones de tiempo:
   La oferta debe incluir una fecha de vigencia que no supere los 6 meses.
   Condiciones de error:
   Manejo de errores de conexión y validación de datos.
   Requisitos de interfaz de usuario:
   El formulario debe ser claro y accesible, con validaciones visuales para errores en los campos obligatorios.
   Debe incluir un botón "Cancelar" para descartar cambios.

### Buscar oferta de trabajo:

1. Identificación de los actores
   Actor Principal: Antiguos Alumnos

2. Definición del escenario
   Un alumni accede al sistema para buscar ofertas de trabajo, realiza una búsqueda, revisa los resultados y puede seleccionar una oferta.

3. Documentación del flujo de eventos principales
    1. El alumni inicia sesión en la plataforma.
    2. Accede a la sección "Buscar ofertas de trabajo".
    3. Introduzca criterios de búsqueda, como: ubicación, tipo de jornada, salario, etc.
    4. El sistema procesa la consulta y muestra una lista de ofertas que cumplen con los criterios.
    5. El alumni selecciona una oferta para ver más detalles.
    6. El sistema muestra la información completa de la oferta.

4. Especificación de flujos alternativos y excepciones
   Sin resultados:
   Si no se encuentran ofertas que coinciden con los criterios, el sistema muestra un mensaje como "No se encontraron ofertas que coinciden con tu búsqueda".
   El alumni puede ajustar los filtros o realizar una nueva búsqueda.
   Falta de autenticación:
   Si el alumni no tiene una sesión activa, el sistema redirige a la página de inicio de sesión antes de permitir la búsqueda.

5. Precondiciones y postcondiciones:

   Precondiciones:

   El exalumno debe estar registrado y autenticado en el sistema.
   Debes haber ofertas publicadas y validadas disponibles en la plataforma.

   Postcondiciones:

   El alumni puede visualizar una lista de ofertas que coinciden con sus intereses.
   Si selecciona una oferta, se guarda un registro de actividad (opcional).

6. Requisitos especiales

   Condiciones de error:
   Manejo adecuado de errores de conexión o problemas con la base de datos.
   Requisitos de interfaz de usuario:
   El sistema debe proporcionar filtros claros y accesibles para la búsqueda.
   Los resultados deben mostrarse en un formato legible, con paginación si hay muchas ofertas.

### Aceptar oferta de trabajo:

1. Identificación de los actores
   Actor Principal: Administrador

2. Definición del escenario
   Un administrador revisa las ofertas de trabajo creadas para verificar que cumplen con las políticas de la plataforma. Si la oferta es válida, se aprueba y queda visible para los alumni.

3. Documentación del flujo de eventos principales
    1. El administrador inicia sesión en la plataforma.
    2. Accede a la sección "Ofertas Pendientes de Validación".
    3. Visualiza una lista de ofertas con estado "Pendiente de Validación".
    4. Selecciona una oferta para revisarla en detalle.
    5. Evalúa si la oferta cumple con los criterios establecidos.
    6. Si la oferta es válida, presiona el botón "Aceptar".
    7. El sistema actualiza el estado de la oferta a "Publicada" y la hace visible para los exalumnos.
    8. El sistema notifica a la empresa que su oferta ha sido aceptada.

4. Especificación de flujos alternativos y excepciones

   Oferta rechazada:

   Si la oferta no cumple con los criterios, el administrador puede optar por rechazarla.
   Presiona el botón "Rechazar", el sistema cambia el estado de la oferta a "Rechazada" y notifica a la empresa los motivos del rechazo.

   Error al guardar el estado:

   Si ocurre un error interno al intentar actualizar el estado de la oferta, el sistema muestra un mensaje de error y permite al administrador reintentar.

   Falta de acceso:
   Si un usuario no autorizado intenta acceder a la sección de validación, el sistema redirige a la página de inicio con un mensaje de acceso denegado.


5. Precondiciones y postcondiciones:

   Precondiciones:

   El administrador debe estar registrado y autenticado en el sistema.
   Deben existir ofertas con estado "Pendiente de Validación".
   El sistema debe contar con criterios claros de aceptación para las ofertas.

   Postcondiciones:

   La oferta queda registrada con el estado "Publicada" y es visible para los exalumnos.
   La empresa creadora recibe una notificación de que su oferta ha sido aceptada.

6. Requisitos especiales

   Restricciones de tiempo:
   La validación de la oferta debe completarse en un tiempo razonable (por ejemplo, 48 horas).
   Condiciones de error:
   Manejo adecuado de errores relacionados con la actualización del estado de las ofertas.
   Requisitos de interfaz de usuario:
   La interfaz debe permitir al administrador visualizar la información completa de la oferta, con botones claros para aceptar o rechazar.
   Debe incluir un campo opcional para agregar comentarios en caso de rechazo.

### Postular para la oferta de trabajo:

1. Identificación de los actores
   Actor Principal: Antiguos Alumnos

2. Definición del escenario
   Un exalumno encuentra una oferta de trabajo de interés y deseo postular. Proporciona su información de contacto, adjunta su currículum vitae y envía la solicitud a la empresa que publicó la oferta.

3. Documentación del flujo de eventos principales

    1. El alumni inicia sesión en la plataforma.
    2. Busca y selecciona una oferta de trabajo publicada.
    3. Acceda al detalle de la oferta y presione el botón "Postular".
    4. El sistema muestra un formulario que incluye:
    5. Información del alumni (prellenada desde su perfil, si está disponible).
    6. Campo para adjuntar su currículum vitae (en formato PDF, DOC o DOCX).
    7. Campo opcional para agregar un mensaje personalizado para la empresa.
    8. El alumni revisa los datos, adjunta su currículum y presiona el botón "Enviar".
    9. El sistema valida que toda la información requerida esté completa.
    10. El sistema registra la postulación en la base de datos y notifica a la empresa sobre la nueva solicitud.
    11. El alumni recibe una confirmación de que la postulación se ha enviado correctamente.

4. Especificación de flujos alternativos y excepciones

   Falta de datos:

   Si el exalumno intenta enviar la postulación sin completar los campos obligatorios o sin adjuntar un currículum, el sistema muestra un mensaje indicando el error y permite corregirlo.

   Error en la carga del archivo:

   Si el archivo adjunto no es válido (formato incorrecto o tamaño excesivo), el sistema muestra un mensaje de error y permite adjuntar un nuevo archivo.

   Error al enviar la postulación:

   Si ocurre un problema interno durante el envío, el sistema muestra un mensaje indicando el problema y permite reintentar.

5. Precondiciones y postcondiciones:

   Precondiciones:

   El exalumno debe estar registrado y autenticado en el sistema.
   Debe existir al menos una oferta publicada visible para el alumni.

   Postcondiciones:

   La solicitud queda registrada en la base de datos con el estado "Enviada".
   La empresa recibe una notificación de la postulación.
   El alumni recibe una confirmación de que su solicitud se envió exitosamente.

6. Requisitos especiales
   Condiciones de error:
   Manejo de errores al cargar archivos o al registrar la postulación en la base de datos.
   Requisitos de interfaz de usuario:
   La interfaz debe ser intuitiva y permitir al alumni previsualizar su currículum antes de enviarlo.
   Debe incluir un botón "Cancelar" para salir del proceso de postulación sin guardar cambios.


### Cerrar oferta de trabajo:

1. Identificación de los actores

   Actor Secundario: Administrador

2. Definición del escenario
   El administrador desea cerrar una oferta de trabajo cuando ya no está disponible, ya sea porque se ha cubierto la vacante, ha caducado o se decide retirarla del sistema.

3. Documentación del flujo de eventos principales:

    1. El administrador inicia sesión en la plataforma.
    2. Accede a la sección "Gestión de Ofertas".
    3. Visualiza una lista de ofertas con estado "Publicada".
    4. Selecciona la oferta que deseas cerrar.
    5. Presiona el botón "Cerrar Oferta".
    7. El sistema actualiza el estado de la oferta a "Cerrada".
    8. La oferta deja de ser visible para los alumni en la búsqueda.
    9. El sistema notifica a la empresa.

4. Especificación de flujos alternativos y excepciones:

   Fallo en la confirmación:

   Si el actor cancela la confirmación, el sistema no realiza cambios y vuelve a la lista de ofertas.

   Error en el cierre:

   Si ocurre un problema interno durante el cambio de estado de la oferta, el sistema muestra un mensaje indicando el error y permite reintentar.

   Acceso no autorizado :

   Si un actor no autorizado intenta cerrar una oferta (por ejemplo, una empresa intentando cerrar una oferta de otra empresa), el sistema bloquea la acción y muestra un mensaje de acceso denegado.

5. Precondiciones y postcondiciones:

   Precondiciones:

   El actor debe estar registrado y autenticado en el sistema.
   La oferta debe estar en estado "Publicada".

   Postcondiciones:

   La oferta queda registrada con el estado "Cerrada".
   La oferta ya no es visible para los alumni en la búsqueda.
   Se notifica al actor correspondiente sobre el cierre.

6. Requisitos especiales
   Condiciones de error:
   Manejo adecuado de errores relacionados con la actualización del estado de las ofertas.

   Requisitos de interfaz de usuario:
   La interfaz debe mostrar una confirmación clara antes de realizar el cierre.
   Debe incluir la opción de "Cancelar" durante el proceso de cierre.

### Cancelar oferta de trabajo:

1. Identificación de los actores
   Actor Principal: Administrador

2. Definición del escenario
   El administrador detecta que una oferta de trabajo publicada no cumple con las políticas de la plataforma o contiene errores significativos y decide cancelarla para que no sea visible para los alumni ni accesible para la empresa.

3. Documentación del flujo de eventos principales
    1. El administrador inicia sesión en la plataforma.
    2. Accede a la sección "Gestión de Ofertas" .
    3. Visualiza una lista de ofertas con estado "Publicada".
    4. Selecciona la oferta que desea cancelar.
    5. Presiona el botón "Cancelar Oferta".
    6. El sistema muestra un cuadro de diálogo solicitando al administrador que proporcione un motivo para la cancelación.
    7. El administrador ingresa el motivo y confirma la acción.
    8. El sistema actualiza el estado de la oferta a "Cancelada".
    9. La oferta deja de ser visible tanto para los alumni como para la empresa que la creó.
    10. El sistema notifica a la empresa creadora sobre la cancelación, incluyendo el motivo proporcionado por el administrador.

4. Especificación de flujos alternativos y excepciones

   Fallo en la confirmación:

   Si el administrador cancela la acción en el cuadro de diálogo, la oferta permanece en estado "Publicada" y no se realizan cambios.

   Error en el proceso:

   Si ocurre un problema interno al intentar actualizar el estado de la oferta, el sistema muestra un mensaje de error y permite al administrador reintentar.

   Acceso no autorizado:

   Si un usuario no autorizado intenta acceder a la funcionalidad de cancelación, el sistema redirige a la página de inicio con un mensaje de acceso denegado.

5. Precondiciones y postcondiciones

   Precondiciones:

   El administrador debe estar registrado y autenticado en el sistema.
   La oferta debe estar en estado "Publicada".

   Postcondiciones:

   La oferta queda registrada con el estado "Cancelada".
   La oferta deja de ser visible para los alumni y la empresa creadora.
   La empresa creadora recibe una notificación con el motivo de la cancelación.

6. Requisitos especiales

   Condiciones de error:
   El sistema debe manejar adecuadamente los errores relacionados con la base de datos o la conexión.

   Requisitos de interfaz de usuario:
   La interfaz debe incluir un cuadro de diálogo para que el administrador proporcione un motivo antes de confirmar la cancelación.
   El sistema debe permitir al administrador visualizar todos los detalles de la oferta antes de cancelarla.


## **Prototipar Casos de Uso**

---

### **Crear Oferta de Trabajo**

1. **La empresa inicia sesión en la plataforma**

2. **Accede a la sección "Crear oferta de trabajo"**
    - Un botón redirige al formulario correspondiente.

3. **Llena los campos requeridos del formulario, que incluyen:**
    - Título de la oferta.
    - Descripción.
    - Requisitos.
    - Duración o vigencia de la oferta.
    - Ubicación (opcional).

   Una vez completado, se presiona el botón **"Guardar"**.

4. **El sistema valida que todos los campos obligatorios estén completos.**

5. **El sistema guarda la oferta como "Pendiente de Validación".**
    - La oferta se almacena en una base de datos.
    - Un botón **"Pendiente de Validación"** estará habilitado para acceder a estas ofertas.

6. **El administrador recibe una notificación para revisar la oferta.**
    - El sistema notifica que hay una oferta pendiente y el administrador puede acceder desde el botón correspondiente.

---

### **Buscar Oferta de Trabajo**

1. **El alumni inicia sesión en la plataforma**

2. **Accede a la sección "Buscar ofertas de trabajo".**
    - Un botón habilitado en el perfil del alumni redirige a esta sección, mostrando todas las ofertas almacenadas en la base de datos.

3. **Introduce criterios de búsqueda, como:**
    - Ubicación.
    - Tipo de jornada.
    - Salario.

4. **El sistema procesa la consulta y muestra una lista de ofertas que cumplen con los criterios.**

5. **El alumni selecciona una oferta para ver más detalles.**
    - Al seleccionar una oferta, se muestra la descripción completa.

---

### **Aceptar Oferta de Trabajo**

1. **El administrador inicia sesión en la plataforma**

2. **Accede a la sección "Ofertas Pendientes de Validación".**
    - Desde su interfaz, un botón redirige al apartado de ofertas pendientes.

3. **Visualiza una lista de ofertas con estado "Pendiente de Validación".**

4. **Selecciona una oferta para revisarla en detalle.**

5. **Valida o rechaza la oferta:**
    - Si la oferta es válida, presiona el botón **"Aceptar"**, y la oferta se publica para los alumni.
    - Si la oferta no es válida, presiona el botón **"No validar"**, y la oferta se elimina del sistema.

6. **El sistema notifica a la empresa que su oferta ha sido aceptada.**

---

### **Postular para la Oferta de Trabajo**

1. **El alumni inicia sesión en la plataforma**

2. **Busca y selecciona una oferta publicada.**
    - Puede buscar ofertas mediante palabras clave o explorar la lista de ofertas publicadas.

3. **Accede al detalle de la oferta y presiona el botón "Postular".**
    - El sistema muestra un formulario con los siguientes campos:
        - **Información del alumni.**
        - **Adjuntar currículum vitae** (formatos permitidos: PDF, DOC, DOCX).
        - Campo opcional para agregar un mensaje personalizado a la empresa.

4. **El sistema valida que toda la información requerida esté completa.**

5. **El sistema registra la postulación y notifica a la empresa.**
    - La postulación queda registrada en una base de datos accesible para la empresa.
    - La empresa recibe una notificación sobre la nueva solicitud.

6. **El alumni recibe una confirmación.**
    - El sistema confirma que la postulación se ha enviado correctamente.
    - Además, se envía un correo electrónico con la misma información.

---

### **Cerrar Oferta de Trabajo**

1. **El administrador inicia sesión en la plataforma**

2. **Accede a la sección "Gestión de Ofertas".**
    - Desde esta sección, visualiza una lista de ofertas con estado **"Publicada"**.

3. **Selecciona una oferta y presiona el botón "Cerrar Oferta".**
    - Al cerrar la oferta, esta deja de estar visible para los alumni.
    - El sistema actualiza el estado de la oferta como **"Cerrada"**.

4. **El sistema notifica a la empresa.**
    - La empresa recibe una notificación interna y un correo electrónico informando que la oferta ha sido cerrada.

---
