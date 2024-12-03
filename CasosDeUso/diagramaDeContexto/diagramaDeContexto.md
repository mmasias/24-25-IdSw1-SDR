# 📚 Diagrama de Contexto - Sistema de Automatización de Guías Docentes  

Este documento describe el **Diagrama de Contexto** del sistema de Automatización de Guías Docentes. El diagrama ilustra los principales flujos de interacción entre los actores y el sistema, detallando los procesos esenciales y las actividades relevantes para garantizar la gestión eficaz de las guías.  

## 📝 Descripción General  

El **Diagrama de Contexto** ofrece una representación general del sistema, organizando los componentes clave y destacando cómo los actores interactúan con las diferentes funcionalidades del sistema. Facilita la comprensión de las responsabilidades de cada actor y los flujos entre procesos.  

---  

## 🖇️ Componentes del Diagrama de Contexto  

### 1. **Acceso al Sistema**  
   - **Descripción:** Proceso inicial donde los actores inician o cierran sesión en el sistema.  
   - **Actores involucrados:** Profesores, Técnicos de Calidad, Directores de Grado, Dirección de Calidad.  
   - **Objetivo:** Garantizar que los usuarios autenticados accedan a las funciones del sistema según sus roles.  

---  

### 2. **Edición de Contenido**  
   - **Descripción:** Permite a los Técnicos de Calidad realizar ajustes en el contenido estático de las guías.  
   - **Actor principal:** Técnico de Calidad.  
   - **Subprocesos relacionados:**  
     - Guardar cambios en las guías.  
     - Preparar el documento para revisión.  

---  

### 3. **Revisión y Aprobación de Contenido**  
   - **Descripción:** Proceso de evaluación de las guías para su aprobación o rechazo.  
   - **Actor principal:** Director de Grado.  
   - **Flujos relevantes:**  
     - Retroalimentación sobre cambios.  
     - Confirmación de decisiones (aprobación o rechazo).  

---  

### 4. **Supervisión de Guías**  
   - **Descripción:** Monitoreo y control de las guías en proceso por parte del Técnico de Calidad.  
   - **Actor principal:** Técnico de Calidad.  
   - **Objetivo:** Asegurar que las guías cumplan con los requisitos antes de la revisión formal.  

---  

### 5. **Auditoría de Guías**  
   - **Descripción:** Evaluación realizada por la Dirección de Calidad para verificar el cumplimiento con estándares establecidos.  
   - **Actor principal:** Dirección de Calidad.  
   - **Objetivo:** Garantizar la calidad final de las guías antes de su publicación.  

---  

### 6. **Asignación y Gestión**  
   - **Descripción:** Permite asignar guías a titulaciones y asignaturas a titulaciones.  
   - **Actor principal:** Técnico de Calidad.  
   - **Flujos relevantes:**  
     - Confirmar asignación de guías.  
     - Vincular asignaturas correctamente.  

---  

### 7. **Publicación y Generación de Nuevas Versiones**  
   - **Descripción:** Proceso final para publicar las guías aprobadas y crear nuevas versiones cuando sea necesario.  
   - **Actores involucrados:** Director de Grado, Técnico de Calidad.  
   - **Objetivo:** Hacer disponibles las guías aprobadas mientras se conserva el historial de versiones.  

---  

### 8. **Verificación con Memoria**  
   - **Descripción:** Validación de que las guías cumplen con la memoria académica verificada.  
   - **Actor principal:** Dirección de Calidad.  
   - **Objetivo:** Confirmar que las guías se ajusten a los parámetros de la memoria académica aprobada.  

---

## 🌟 Representación Gráfica

![Diagrama de Contexto](/images/modelosUML/DiagramaDeContexto.svg)  

| [Ver código fuente](/CasosDeUso/diagramaDeContexto/DiagramaDeContexto.puml)
