[![Inicio](https://img.shields.io/badge/Inicio-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main)  
[![Actores, Diagrama de Contexto y Casos de Uso](https://img.shields.io/badge/Casos%20de%20Uso-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/casosDeUso)  
[![Prototipos](https://img.shields.io/badge/Prototipos-blue?style=for-the-badge)](https://github.com/srgiom/24-25-IdSw1-SDR/tree/main/prototipos)  

## 🛠️ **Modelo de Dominio**  
Usamos las siguientes herramientas para definir las entidades principales de nuestro sistema:

---

### **Diagrama de Clases**  
![Diagrama de Clases](/modeloDelDominio/imagenes/DiagramaDeClases.svg)  
> **Descripción:**  
> - A cada `Asignatura` se le asigna un `Grado` en `AsignaturaGrado`.  
> - A esa `AsignaturaGrado` se le asigna un `Profesor` para que sea impartida en `AsignaturaGradoProfesor`.  
> - `AsignaturaGradoProfesor` se vincula a un `Horario` y más tarde se asigna un `Aula`, todo ello reflejado en `HorarioAsignaturaAula`.  

---

### **Diagrama de Objetos**  
![Diagrama de Objetos](/modeloDelDominio/imagenes/DiagramaDeObjetos.svg)  
> **Descripción:**  
> - La `Asignatura` (Programación Avanzada) es asignada al `Grado` de Ingeniería Informática en `AsignaturaGrado`.  
> - A `AsignaturaGrado` se le asigna un `Profesor` (María López) para que sea impartida en `AsignaturaGradoProfesor`.  
> - Se vincula a un `Horario` (Lunes de 10:00 a 12:00) y más tarde se asigna el `Aula` 501, todo ello reflejado en `HorarioAsignaturaAula`.  

---

### **Estados de Asignatura**  
![Diagrama de Estados](/modeloDelDominio/imagenes/diagramaEstadosAsignatura.svg)  
> **Descripción:**  
> - Partes de cero en el estado `SinAsignar` y asignas un `Grado` a la `Asignatura` (AsignaturaGrado), creando el estado `GrupoDefinido`.  
> - Se le asigna un `Profesor` (AsignaturaGradoProfesor) para completar el estado `ProfesorAsignado`.  
> - Se le asigna un `Aula` en el estado `AulaAsignada`. Hasta este momento existe la opción de cancelar asignación que nos llevará al estado de `Cancelado`.  
> - Confirmamos la asignación para llegar al estado `Confirmado` para completar la operación.  

---

### **Estados de Profesor**  
![Diagrama de Estados Profesor](/modeloDelDominio/imagenes/DiagramaDeEstadosProfesor.svg)  
> **Descripción:**  
> - Un `Profesor` comienza en el estado `SinAsignar`.  
> - Se le asigna un `Grupo` de `AsignaturaGrado` para pasar al estado `AsignadoAGrupo`.  
> - Posteriormente, se asigna un aula en `AsignadoConAula`.  
> - La asignación puede cancelarse en cualquier momento, llevando al estado `Cancelado`.  
> - Al confirmar la asignación, el `Profesor` pasa al estado final `Confirmado`.  

---

### **Estados de Aula**  
![Diagrama de Estados Aula](/modeloDelDominio/imagenes/DiagramaDeEstadosAula.svg)  
> **Descripción:**  
> - Un `Aula` comienza en el estado `Disponible`.  
> - Se asigna un aula a un horario reflejado en `HorarioAsignaturaAula`, pasando al estado `Asignada`.  
> - Posteriormente, la asignación se confirma, alcanzando el estado `Confirmada`.  
> - La asignación puede ser cancelada en cualquier momento, regresando al estado `Cancelada`.  

---

### **Estados de Grado**  
![Diagrama de Estados Grado](/modeloDelDominio/imagenes/DiagramaDeEstadosGrado.svg)  
> **Descripción:**  
> - Un `Grado` comienza en el estado `SinDefinir`.  
> - Se registra el grado en `Definido`.  
> - Se asignan `Asignaturas` al grado, pasando al estado `AsignaturasAsignadas`.  
> - La configuración puede ser cancelada en cualquier momento, llevándolo al estado `Cancelado`.  
> - Finalmente, al confirmar la asignación de asignaturas, el `Grado` pasa al estado final `Confirmado`.  

---
