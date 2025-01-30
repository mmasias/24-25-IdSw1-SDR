# **GLOSARIO**  

---
## Conceptos Clave

## Guía Docente
La Guía Docente de una asignatura es un documento público dirigido, fundamentalmente, a los estudiantes y escrito con un lenguaje muy claro, en el que se concreta, para un determinado curso académico, la planificación docente de una asignatura y toda la información necesaria para su seguimiento.

### **Automatización**
Aplicación que minimiza la intervención manual en la actualización de las guías docentes, asegurando mayor eficiencia y control.

### **Roles y Permisos**
Sistema de usuarios con roles definidos y permisos restringidos a ciertos campos, garantizando seguridad y trazabilidad.

- **Profesor**: Edita ciertos campos como nombre, email, contenido de la asignatura, actividades de evaluación y bibliografía.
- **Director de Grado**: Aprueba o rechaza las guías enviadas por los profesores.
- **Técnico de Calidad**: Edita toda la guía, incluyendo contenido estático.
- **Dirección de Calidad**: Supervisa y audita el trabajo de los otros roles.

### **Flexibilidad**
Un usuario puede tener múltiples roles, como un profesor que también sea director de grado.

### **Control de Asignación**
Evita que una persona apruebe su propio trabajo, asegurando integridad en el proceso de validación.

### **Trazabilidad**
Sistema que registra todo el proceso de creación, edición y aprobación de guías para auditorías futuras.

## **Funcionalidades Deseadas**

### **Automatización de Guías**
Generación de guías en PDF y subida automática al panel universitario.

### **Edición Controlada**
Los campos estáticos solo pueden ser editados por el departamento de calidad (Técnico de Calidad), mientras que los dinámicos son modificables por los profesores.

### **Roles y Permisos**
Definición clara de permisos según el rol del usuario.

### **Trazabilidad**
Registro de cada acción realizada por los usuarios para auditoría.

### **API de Verificación**
Uso de IA para validar que los cambios realizados cumplen con la memoria verificada.

## **Requisitos No Funcionales**

### **Interfaz de Usuario**
Debe ser simple, con estados de guías visibles (pendiente, enviado, aprobado).

### **Auditoría**
Generación de informes sobre el estado de las guías.

## **Definición Específica de Roles**

### **1. Profesor**
- **Permisos de edición**: 
  - Nombre del profesor y su email.
  - Contenidos de la asignatura alineados con la memoria verificada.
  - Metodologías docentes y actividades formativas.
  - Tipos y porcentajes de evaluación dentro de los límites establecidos.
  - Bibliografía y recursos generales.

- **Validación por IA**: API de inteligencia artificial revisa los cambios y emite un preaprobado, pero la decisión final la toma el Director de Grado.

### **2. Director de Grado**
- **Responsabilidad**: Revisa y aprueba guías docentes enviadas por los profesores.
- **Notificaciones**: Recibe alertas cuando un profesor envía una guía.
- **Opciones de decisión**: Puede aprobar o solicitar modificaciones con retroalimentación.
- **Trazabilidad**: Registro de cambios, decisiones y generación de PDF.
- **Publicación**: Responsable de garantizar la disponibilidad de las guías a tiempo.

### **3. Técnico de Calidad**
- **Permisos completos**: Puede modificar toda la guía, incluyendo contenido estático.
- **Rol inicial**: Primera instancia en la edición para asegurar la calidad del contenido estático antes de intervención de profesores o directores de grado.
- **Revisión y corrección**: Ajusta, rechaza y reenvía modificaciones para revisión.

### **4. Dirección de Calidad**
- **Supervisión**: Audita el trabajo de todos los roles.
- **API de ordenación académica**: Sincroniza con la base de datos universitaria para validar asignaciones de profesores a asignaturas.
