[![Inicio](https://img.shields.io/badge/Inicio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main)
[![Actores, Diagrama de Contexto y Casos de Uso](https://img.shields.io/badge/Casos%20de%20Uso-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/casosDeUso)
[![Prototipos](https://img.shields.io/badge/Prototipos-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/prototipos)

## 🛠️ **Modelo de Dominio**
Usamos las siguientes herramientas para definir las entidades principales de nuestro sistema:

### Diagrama de Clases
![Diagrama de Clases](/modeloDelDominio/imagenes/DiagramaDeClases.svg)
> **Descripción:**
> - A cada `Asignatura` se le asigna un `Grado` en `AsignaturaGrado`.
> - A esa `AsignaturaGrado` se le asigna un `Profesor` para que sea impartida en `AsignaturaGradoProfesor`.
> - `AsignaturaGradoProfesor` se vincula a un `Horario` y más tarde se asigna un `Aula`, todo ello reflejado en `HorarioAsignaturaAula`.

### Diagrama de Objetos
![Diagrama de Objetos](/modeloDelDominio/imagenes/DiagramaDeObjetos.svg)
> **Descripción:**
> - La `Asignatura`(Programación Avanzada) es asignada al `Grado` de Ingeniería Informática en `AsignaturaGrado`.
> - A `AsignaturaGrado` se le asigna un `Profesor`(María López) para que sea impartida en `AsignaturaGradoProfesor`.
> - Se vincula a un `Horario`(Lunes de 10:00 a 12:00) y más tarde se asigna el `Aula` 501, todo ello reflejado en `HorarioAsignaturaAula`.

### Estados de Asignatura
![Diagrama de Estados](/modeloDelDominio/imagenes/DiagramaDeEstados.svg)
> **Descripción:**
> - Partes de cero en el estado `SinAsignar` y asignas un `Grado` a la `Asignatura`(AsignaturaGrado), creando el estado `GrupoDefinido`.
> - Se le asigna un `Profesor`(AsignaturaGradoProfesor) para completar el estado `ProfesorAsignado`.
> - Se le asigna un `Aula` en el estado `AulaAsignada`. Hasta este momento existe la opción de cancelar asignación que nos llevará al estado de `Cancelación`.
> - Confirmamos la asignación para llegar al estado de `Confirmación` para completar la operación.
