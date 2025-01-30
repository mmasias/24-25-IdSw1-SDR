<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Priorización_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Priorizacion.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |

</div>


# 🚀 **Priorizar Casos de Uso**
En este apartado se muestran los casos de uso en una lista donde el número **1** tiene más prioridad. Esta matriz presenta un análisis detallado de los casos de uso de un sistema, evaluados en función de diversos criterios como el **riesgo técnico**, la **contribución a la arquitectura**, las **dependencias**, el **costo/esfuerzo**, el **valor para el negocio** y la **visibilidad**.

> 🎯 **Objetivo:** Identificar y priorizar los casos de uso más críticos para el éxito del proyecto.  

---

## 📊 **Matriz de Priorización de Casos de Uso**  

| 🔢 | 📝 **Caso de Uso**                                     | 🎭 **Actor**               | ⚠️ **Riesgo Técnico** | 🏗 **Arquitectura** | 🔗 **Dependencias** | 💰 **Costo/Esfuerzo** | 💼 **Valor Negocio** | 👀 **Visibilidad** | 🚦 **Prioridad** |
|----|------------------------------------------------------|-------------------------|--------------------|---------------------|------------------|---------------------|------------------|-------------|------------|
| 1  | **✅ Verificar Cumplimiento con Memoria Verificada**  | Dirección de Calidad    | 🔴 Alto            | 🔴 Alto              | 🟠 Medio          | 🔴 Alto             | 🔴 Alto          | 🔴 Alto      | **🔥 🔴 Alta**  |
| 2  | **🔍 Auditar Guía**                                   | Dirección de Calidad    | 🟠 Medio           | 🔴 Alto              | 🟠 Medio          | 🔴 Alto             | 🔴 Alto          | 🔴 Alto      | **🔥 🔴 Alta**  |
| 3  | **📢 Publicar Guía**                                  | Director de Grado       | 🟢 Bajo            | 🟠 Medio             | 🔴 Alto          | 🟢 Bajo             | 🔴 Alto          | 🔴 Alto      | **🔥 🔴 Alta**  |
| 4  | **✔️ Aprobar Guía**                                   | Director de Grado       | 🟢 Bajo            | 🟠 Medio             | 🟠 Medio          | 🟠 Medio            | 🔴 Alto          | 🟠 Medio     | **⚡️ 🟠 Media-Alta**  |
| 5  | **📄 Revisar Guía**                                   | Director de Grado       | 🟢 Bajo            | 🟠 Medio             | 🟠 Medio          | 🟠 Medio            | 🟠 Medio          | 🟠 Medio     | **⚡️ 🟠 Media-Alta**  |
| 6  | **📩 Enviar Guía Docente para Revisión**             | Profesor                | 🟢 Bajo            | 🟠 Medio             | 🟠 Medio          | 🟠 Medio            | 🟠 Medio          | 🟠 Medio     | **⚡️ 🟠 Media-Alta**  |
| 7  | **📝 Editar Contenido Dinámico**                     | Profesor                | 🟢 Bajo            | 🟠 Medio             | 🟢 Bajo          | 🟠 Medio            | 🟠 Medio          | 🟠 Medio     | **🔅 🟡 Media**  |
| 8  | **📝 Editar Contenido Estático**                     | Técnico de Calidad      | 🟢 Bajo            | 🟠 Medio             | 🟢 Bajo          | 🟠 Medio            | 🟠 Medio          | 🟠 Medio     | **🔅 🟡 Media**  |
| 9  | **🔄 Generar Nueva Versión de la Guía**              | Técnico de Calidad      | 🟢 Bajo            | 🟠 Medio             | 🟢 Bajo          | 🟠 Medio            | 🟠 Medio          | 🟢 Bajo      | **🔅 🟡 Media**  |
| 10 | **📂 Asignar Guía a Profesor**                      | Técnico de Calidad      | 🟢 Bajo            | 🟢 Bajo              | 🟢 Bajo          | 🟢 Bajo             | 🟠 Medio          | 🟠 Medio     | **🔅 🟡 Media**  |
| 11 | **🔑 Iniciar Sesión**                                | Usuario                 | 🟢 Bajo            | 🔴 Alto              | 🟢 Bajo          | 🟢 Bajo             | 🔴 Alto          | 🔴 Alto      | **🔥 🔴 Alta**  |
| 12 | **🚪 Cerrar Sesión**                                 | Usuario                 | 🟢 Bajo            | 🟢 Bajo              | 🟢 Bajo          | 🟢 Bajo             | 🟠 Medio          | 🟠 Medio     | **✅ 🟢 Baja**  |
| 13 | **⛔ Rechazar Guía**                                 | Director de Grado       | 🟢 Bajo            | 🟠 Medio             | 🟠 Medio          | 🟠 Medio            | 🟠 Medio          | 🟠 Medio     | **🔅 🟡 Media**  |

---
