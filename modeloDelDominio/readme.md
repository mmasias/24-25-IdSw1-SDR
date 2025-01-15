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

### Estados de Asignatura
![Diagrama de Estados](/modeloDelDominio/imagenes/DiagramaDeEstados.svg)
