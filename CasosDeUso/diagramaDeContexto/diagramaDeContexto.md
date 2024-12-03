# 📚 Diagrama de Contexto - Sistema de Automatización de Guías Docentes

Este documento describe el **Diagrama de Contexto** del sistema de Automatización de Guías Docentes. El diagrama detalla las interacciones clave entre los actores externos y el sistema, así como los flujos principales de datos y actividades relevantes.

## 📝 Descripción General

El **Diagrama de Contexto** proporciona una visión global del sistema, organizando sus principales componentes y procesos. Permite identificar de manera clara cómo los actores interactúan con el sistema y cómo se conectan los distintos subsistemas internos.

---

## 🖇️ Componentes del Diagrama de Contexto

### 1. **Autenticación**
   - **Descripción:** Proceso inicial donde los usuarios inician sesión en el sistema.
   - **Actores involucrados:** Profesores, Técnicos de Calidad, Directores de Grado, Dirección de Calidad.
   - **Objetivo:** Garantizar que solo usuarios autorizados accedan al sistema y sus funciones.

---

### 2. **Edición de Guías Docentes**
   - **Descripción:** Permite a los profesores crear, editar y ajustar guías docentes.
   - **Actor principal:** Profesor.
   - **Subprocesos relacionados:**
     - Ajustes de contenido.
     - Revisión interna por Técnicos de Calidad.

---

### 3. **Revisión de Guías**
   - **Descripción:** Proceso en el que el contenido es revisado y validado por el Director de Grado.
   - **Actor principal:** Director de Grado.
   - **Flujos relevantes:**
     - Identificación de observaciones.
     - Retroalimentación y reenvío a profesores.

---

### 4. **Validación**
   - **Descripción:** Validación técnica y de calidad realizada por los Técnicos de Calidad y el sistema automatizado.
   - **Actores involucrados:** Técnico de Calidad, Sistema IA.
   - **Objetivo:** Asegurar que las guías cumplan con estándares de calidad y formato.

---

### 5. **Publicación y Archivado**
   - **Descripción:** Una vez aprobada, la guía se publica y versiones previas se archivan para su consulta.
   - **Actores involucrados:** Director de Grado, Sistema.
   - **Objetivo:** Hacer que las guías estén disponibles para los estudiantes mientras se preservan versiones anteriores.

---

### 6. **Consulta de Guías**
   - **Descripción:** Acceso a guías publicadas y archivadas por estudiantes o administradores.
   - **Actor principal:** Sistema.
   - **Objetivo:** Proveer acceso rápido y eficiente a la información académica.

---

## 🌟 Representación Gráfica

![Diagrama de Contexto](/images/modelosUML/DiaghramaDeContexto.svg)  

| [Ver código fuente](/DiagramaDeContexto.puml)

---

Este diagrama de contexto es una herramienta clave para entender las dinámicas generales del sistema de Automatización de Guías Docentes, identificando a los actores y procesos críticos para el flujo de trabajo. ¿Hay algo más que quieras ajustar o añadir? 😊
