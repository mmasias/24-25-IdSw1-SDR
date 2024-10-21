<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Descripción_General-FFF?style=flat&logo=abbrobotstudio&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/docs/modeloDeDominio/) [![](https://img.shields.io/badge/-Actores_y_Casos_de_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/docs/casosDeUso/) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/docs/sesiones/) |
|-:|

</div>

# DOCUTRACE 📄

## 🔰 APUNTES PRIMERA REUNIÓN - 16/10/2024

Aplicación para la gestión documental -- **DOCUTRACE**

- Para todos los trabajadores se necesita diferente tipo de documentación.

### 🔰 COMO SE HACE ACTUALMENTE:
- Se imprime y se le entrega al trabajador y firma de recibido. Ahora se manda por email y el trabajador aun tiene que firmar el recibido en físico.
- También se tiene un App Script en Google Sheets que genera un token para verificar la autenticidad. Se apunta a quién se le envió, la hora, el token y los documentos, generándose un PDF.

### 🔰 PROBLEMA:
- Un email no tiene validez legal completa, por lo que en caso de una disputa, se necesita un respaldo físico que tiene más peso, a menos que tenga cierto tipo de certificado electrónico.

### 🔰 IDEA:
- Crear una aplicación online donde la universidad tenga accesos para publicar en los buzones de los usuarios la documentación a los empleados, dejando un rastro (trace) de lo que se ha hecho.

### 🔰 ROLES:
- **Administrador general**
- **Usuarios de administración por área**
- **Usuarios trabajadores** (tendrán acceso a la documentación)

### 🔰 FLUJO:
1. Un administrador envía un documento a un trabajador.
2. Se marca la fecha de envío y la fecha en que el destinatario abre el documento.
3. Se marca la fecha de confirmación de que se ha abierto el documento si es requerida.
4. Se puede solicitar una especie de firma para validar que el documento ha sido abierto y firmar electrónicamente de recibido si se requiere.

### 🔰 IMPORTANTE:
- Validar la integridad del documento, que no haya sido alterado.
- Tener un respaldo por si ocurre algún incidente con el trabajador, con la firma electrónica que debe tener el mismo peso que una copia física.
- Trazabilidad del proceso de envío y acceso a los documentos.
- Todos los documentos pueden descargarse posteriormente en PDF **PROTEGIDO**.
- **NO TODOS LOS DOCUMENTOS NECESITAN CONFIRMACIÓN DE LECTURA NI FIRMA ELECTRÓNICA**. Si son solo informativos, no se pedirá ni firma ni confirmación, pero puede haber casos en que solo se pida confirmación de lectura sin firma electrónica.
- Al enviar el documento, si el remitente lo requiere, se enviará ya firmado por el remitente.
- Como firma electrónica, puede ser válido un token.
- Los destinatarios tendrán **categorías**, para que los buzones sean más específicos. Los usuarios pueden pertenecer a **más de una categoría** a la vez.
- Los usuarios solo pueden ver los documentos que se les han enviado, no los de nadie más.
- Los administradores de área también pueden recibir documentos.
- El administrador general puede ver el estado de los envíos de todos los trabajadores.
- Hay dos tipos de usuarios: 
  - Usuario que puede enviar y recibir.
  - Usuario que solo recibe.

### 🔰 A TOMAR EN CUENTA:
- No centralizar solo a los trabajadores de las áreas de la universidad, la aplicación puede extenderse a otros actos de la universidad (carros de comida, convenios con empresas, eventos, etc.).
- Tener en cuenta la **gestión de permisos** para crear diferentes buzones de destinatarios.
- Configurar alertas de seguimiento con días seleccionables.
- Diferentes tipos de alertas.
- Límite en la cantidad de documentos.
- Solo documentos en formato **PDF**.
- Al crear un usuario, se le pueden asignar categorías.
- **Buzón personalizado**, donde cada destinatario puede tener compartidas ciertas categorías.

### 🔰 FUNCIONALIDADES/CASOS DE USO POSIBLES:
- Gestión de usuarios (CRUD).
- Gestión de permisos (CRUD).
- Gestión de destinatarios (Personal docente, personal de administración y servicios, etc.).
- Gestión de categorías.
- Gestión de documentos.
- Cambio de estado de archivos (No leído/Leído), incluyendo confirmación de lectura.
- Firma electrónica.
- Subir un archivo.
- Envío de correo como notificación al recibir un documento con enlace al buzón.

### 🔰 PERMISOS:
- El **Administrador general** puede crear usuarios de todo tipo.
- El **Administrador de área** puede crear usuarios que solo reciben documentos.

### 🔰 GLOSARIO:
- **Usuario**: Persona que puede subir documentos.
- **Destinatario**: Solo recibe documentos.
