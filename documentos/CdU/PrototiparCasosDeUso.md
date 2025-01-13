# 📝 Prototipar Casos de Uso

| [⬅️ Detallar Casos de Uso](DetallarCasosDeUso.md) | [Estructurar el Modelo de Casos de Uso ➡️](EstructurarCasosDeUso.md) |
|:--|--:|

## 🎯 **Objetivo**
El objetivo de este paso es **prototipar los casos de uso** siguiendo las [pautas teóricas](https://github.com/mmasias/IdSw1/blob/main/temario/contenidos/CdU.ICdU.md) de la asignatura.

## 👁️ Vista General por Actores

Debido a que este proyecto tiene direfentes actores, en primer lugar se mostrara las pantallas de inicio correspondientes a cada actor, lo que reflejará las acciones que puede hacer cada uno de ellos.

| **Actor**                | **Prototipo**                                      |
|--------------------------|----------------------------------------------------|
| Inicio de Sesión         | ![InicioSesion](/images/Prototipar/Inicio.png) |
| Admin                    | ![UsuarioAdmin](/images/Prototipar/Admin.png)  |
| Ordenación Académica     | ![UsuarioOrdenacion](/images/Prototipar/Ordenacion.png) |
| Recursos Humanos         | ![UsuarioRRHH](/images/Prototipar/RRHH.png)    |
| Profesor                 | ![UsuarioProfesor](/images/Prototipar/Profesor.png) |
| Técnico de Calidad       | ![UsuarioCalidad](/images/Prototipar/Calidad.png)  |

## 🛠️ Casos de Uso

A continuación se presentan los casos de uso prototipados.

### 📂 Gestión de Datos del Profesorado

#### Modificación y Validación

| **Caso de Uso**  | **Prototipo**        |
|------------------|--------------------|
| ![](/images/modelosUML/CdU/Individuales/ModificarDatos.svg)            | ![ModificarDatosProfesorado](/images/Prototipar/ModificacionDatosProfesorado.png) |
| ![](/images/modelosUML/CdU/Individuales/ValidarDatos.svg)              | ![ValidarDatosProfesorado](/images/Prototipar/ValidacionDatosProfesorado.png)     |
| ![](/images/modelosUML/CdU/Individuales/ValidarMemoriaTitulacion.svg)  | ![ValidaciónMemoria](/images/Prototipar/ValidaciónCumplimientoMemoria.png)        |

#### Consulta de Datos

| **Caso de Uso**   | **Prototipo**    |                                      
|-------------------|----------------|
| ![](/images/modelosUML/CdU/Individuales/ClaustroDocente.svg)           |         ![ClaustroDocente](/images/Prototipar/ConsultarClaustroDocente.png)                    |
| ![](/images/modelosUML/CdU/Individuales/ConsultarProfesor.svg)         | ![ConsultaAsignacionDocenteProfesor](/images/Prototipar/ConsultaAsignaciónDocenteProfesor.png) |
| ![](/images/modelosUML/CdU/Individuales/ConsultarVarios.svg)           | ![ConsultarAsignacionDocente](/images/Prototipar/AsignaciónDocenteTitulacion.png)              |
| ![](/images/modelosUML/CdU/Individuales/ConsultarDatosPersonales.svg)  | ![ConsultarDatosyContrato](/images/Prototipar/DatosContratoPersonales.png)                     |

#### Introducción de Datos

| **Caso de Uso**    | **Prototipo**  |
|--------------------|--------------|
| ![](/images/modelosUML/CdU/Individuales/IntroducirDatosLaborales.svg)  | ![IntroducirDatos](/images/Prototipar/DatosLaborales.png)                                      |
| ![](/images/modelosUML/CdU/Individuales/IntroducirDatosAcademicos.svg) | ![DatosAcademicos](/images/Prototipar/DatosAcademicos.png)                                     |

---

### 📚 Gestión de Carga Docente

#### Revisión de Cumplimiento

| **Caso de Uso**     | **Prototipo**   |   
|---------------------|---------------|
| ![](/images/modelosUML/CdU/Individuales/RevisarListadoProfesores.svg)  | ![RevisarCargaProfesoresNoAjustada](/images/Prototipar/RevisionCargaDocente.png)               |

#### Asignaciones

| **Caso de Uso**    | **Prototipo**   |
|--------------------|---------------|
| ![](/images/modelosUML/CdU/Individuales/AsignarCargaDocente.svg)       | ![AsignacionAsignaturasProfesor](/images/Prototipar/AsignacióndeCargaDocente.png)              |
| ![](/images/modelosUML/CdU/Individuales/AsignarValores.svg)            |    ![AsignarValores](/images/Prototipar/AsignarValores.png)                                    |
| ![](/images/modelosUML/CdU/Individuales/AsignarSIIUyDGU.svg)           |              ![AsignarSIIU](/images/Prototipar/AsignarSIIU.png)                                |

---

### 📊 Generación de Indicadores e Informes

| **Caso de Uso**        | **Prototipo**    |
|------------------------|----------------|
| ![](/images/modelosUML/CdU/Individuales/EmitirInforme.svg)             | ![Emitir Informe](/images/Prototipar/EmitirInformeProfesorado.png)                             |
| ![](/images/modelosUML/CdU/Individuales/ObtenerIndicadores.svg)        | ![Obtener indicadores](/images/Prototipar/IndicadoresSistemaGestion.png)                       |
