<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/docs/modeloDeDominio/) [![](https://img.shields.io/badge/-Actores_y_Casos_de_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/docs/casosDeUso/) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/docs/sesiones/) |
|-:|

</div>


# DOCUTRACE 📄

## 🔰APUNTES CUARTA REUNIÓN - 5/12/2024

### Apuntes del grupo

#### Cuales son los datos necesarios para la creación de un usuario.
-   correo
-   contraseña generada por el sistema y se envie al correo
-   estado (activo, suspendido)
-   nombre y apellido
-   cargo (profesar, contable, etc.)
-   timestamps
-   opcion para filtrar
-   IDEA: AGREGAR VENTANA DE CONFIGURACION DE USUARIOS
####  Datos necesarios para un grupo
-   nombre
-   usuarios dentro del grupo
-   estado
-   filtrar
#### Datos necesarios para un mensaje
-   remitente
-   destinatario (puede ser grupo o sea un array)
-   estado (borrador, enviado, pendiente, etc.)
-   documento adjunto
-   acciones que se pedirán (firma / confirmacion)
-   fecha limite
-   filtrar por rangos de envio o recibido
-   Las firmas son por envio, no por documento
-   IDEA: LAS NOTIS SE TIENEN QUE ENVIAR UN CORREO CON LA NOTIFICACION PENDIENTE
-   IDEA: IMPLEMENTAR SOFTDELETE, mensajes se envían a una papelera, si un mensaje ya esta enviado, no se puede eliminar, solo archivar, los borradores si se pueden eliminar por completo
#### Audítoria
-   usuario
-   mensajes enviados (ver mensajes y que envio)
-   filtrar por usuario o por asuntos o por contenido del mensaje
-   filtar por rangos de fechas
-   acciones de grupos, usuarios, etc.
#### ALERTAS
-   alerta sobre los mensajes enviados o recordatorios