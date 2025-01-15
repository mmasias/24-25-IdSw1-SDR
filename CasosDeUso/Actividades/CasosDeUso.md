<div align=right>

| [![](https://img.shields.io/badge/-Inicio-FFF?style=flat&logo=Emlakjet&logoColor=black)](/README.md) [![](https://img.shields.io/badge/-Modelo_de_Dominio-FFF?style=flat&logo=LiveChat&logoColor=black)](/ModeloDelDominio/modeloDelDominio.md) [![](https://img.shields.io/badge/-Actores-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Actores.md) [![](https://img.shields.io/badge/-Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/CasosDeUso.md) [![](https://img.shields.io/badge/-Detallado_Casos_De_Uso-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Detallar.md) [![](https://img.shields.io/badge/-Diagrama_De_Contexto-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/diagramaDeContexto/diagramaDeContexto.md) [![](https://img.shields.io/badge/-Prototipos-FFF?style=flat&logo=openstreetmap&logoColor=black)](/CasosDeUso/Actividades/Prototipos/README.md) [![](https://img.shields.io/badge/-Sesiones_de_Requisitado-FFF?style=flat&logo=Proton&logoColor=black)](/SesionesDeRequisitado)  |


</div>

# Casos de Uso
---
![](/images/modelosUML/diagramaCasosDeUso.svg) | [Ver código](/CasosDeUso/diagramaCasosDeUso/diagramaCasosDeUso.puml) 

## 1.[Editar Contenido de la Guía](/CasosDeUso/Actividades/Detallar.md#4-editar-contenido-de-la-guía)
- **Actor**: Profesor
- **Descripción**: El profesor realiza actualizaciones en el contenido de una guía docente para una asignatura específica.
- **Objetivo**: Mantener el contenido actualizado y relevante para los estudiantes.

## 2. [Revisar Contenido](/CasosDeUso/Actividades/Detallar.md#5-revisar-contenido)
- **Actor**: Director de Grado
- **Descripción**: Revisión y decisión sobre la aprobación o rechazo del contenido de la guía docente.
- **Objetivo**: Asegurar que el contenido cumple con los estándares académicos y es adecuado para su publicación.

## 3. [Asignar Guías Docentes a Profesor](/CasosDeUso/Actividades/Detallar.md#12-asignar-guías-docentes-a-profesor)
- **Actor**: Técnico de Calidad
- **Descripción**: El técnico se encarga de asignar las guías docentes a los profesores. 
- **Objetivo**: Garantizar que cada profesor tenga asignada al menos una guía docente en el formato y la calidad esperada.

## 4. [Auditar Guías Docentes](/CasosDeUso/Actividades/Detallar.md#2-auditar-guías-docentes)
- **Actor**: Dirección de Calidad
- **Descripción**: Realiza auditorías completas sobre las guías docentes para revisar la calidad del contenido y su alineación con los objetivos institucionales.
- **Objetivo**: Asegurar la máxima calidad en las guías y su adherencia a los objetivos académicos.

## 5. [Crear Nueva Versión de la Guía](/CasosDeUso/Actividades/Detallar.md#6-generar-nueva-versión-de-la-guía)
- **Actor**: Técnico de Calidad
- **Descripción**: Solicita al sistema la creación de una nueva versión de la guía para registrar cambios y actualizaciones en el contenido.
- **Objetivo**: Facilitar la trazabilidad de las modificaciones realizadas en la guía a lo largo del tiempo.

## 6. [Editar plantilla de la guía docente](/CasosDeUso/Actividades/Detallar.md#9-editar-plantilla-de-la-guía-docente)
- **Actor**: Técnico de Calidad
- **Descripción**:  El Técnico de Calidad realiza actualizaciones en el formato de la plantilla de una guía docente para una asignatura específica.
- **Objetivo**: Mantener la estructura organizativa de las plantillas en el sistema.

## 7. [Asignar Guía a Titulación](/CasosDeUso/Actividades/Detallar.md#10-asignar-guía-a-titulación)
- **Actor**: Técnico de Calidad
- **Descripción**: Asigna una guía docente a una titulación específica para organizar las guías por cada programa académico.
- **Objetivo**: Asegurar que las guías estén correctamente asociadas con la titulación correspondiente.

## 8. [Asignar Asignatura a Titulación](/CasosDeUso/Actividades/Detallar.md#11-asignar-asignatura-a-titulación)
- **Actor**: Técnico de Calidad
- **Descripción**: Asocia cada asignatura con su titulación respectiva en el sistema.
- **Objetivo**: Mantener la estructura organizativa de los programas académicos en el sistema.

## 9. [Publicar Guía Docente](/CasosDeUso/Actividades/Detallar.md#3-publicar-guía-docente)
- **Actor**: Director de Grado
- **Descripción**: Autoriza la publicación final de una guía docente, permitiendo que sea accesible para los estudiantes a través del panel universitario.
- **Objetivo**: Permitir que los estudiantes accedan a la versión oficial y aprobada de la guía.

## 10. [Verificar Cumplimiento con Memoria Verificada](/CasosDeUso/Actividades/Detallar.md#1-verificar-cumplimiento-con-memoria-verificada)
- **Actor**: Dirección de Calidad
- **Descripción**: Realiza una verificación de las guías docentes para confirmar su adherencia a la memoria verificada de la titulación, utilizando una API de verificación.
- **Objetivo**: Asegurar que las guías cumplan con los lineamientos y requisitos establecidos por la institución.

## 11. [Ver listado de los estados de las guías docentes](/CasosDeUso/Actividades/Detallar.md#7-ver-listado-de-los-estados-de-las-guías-docentes)
- **Actor**: Técnico de Calidad
- **Descripción**: Pede visualizar los estados en los que se encuentran las guías docentes (aprobado o devuelto para modificación)
- **Objetivo**: Revisar los estados de las guías docentes para mantener la trazabilidad en los procesos.

## 12. [Ver listado de los estados de las guías docentes de un grado](/CasosDeUso/Actividades/Detallar.md#8-ver-listado-de-los-estados-de-las-guías-por-grado)
- **Actor**: Director de Grado
- **Descripción**: Pede visualizar los estados en los que se encuentran las guías docentes de su grado correspondiente (aprobado o devuelto para modificación)
- **Objetivo**: Revisar los estados de las guías docentes de su grado para mantener la trazabilidad en los procesos.

## 13. [Enviar Guía Docente para Revisión](/CasosDeUso/Actividades/Detallar.md#13-enviar-guía-docente-para-revisión)
- **Actor**: Profesor
- **Descripción**: El profesor envía la guía docente editada al Director de Grado para su revisión y posterior aprobación o rechazo.
- **Objetivo**: Garantizar que las guías docentes sean revisadas para verificar su cumplimiento con los estándares de calidad y requisitos académicos.
