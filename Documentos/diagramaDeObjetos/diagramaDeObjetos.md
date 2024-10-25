@startuml evas

hide circle
hide empty members

class Profesor {
    nombre = "Ivan"
    apellido ="Gonzalez"
}

class Alumno {
    nombre = "Alejandro"
    apellido = "Higuera"
  edad = "17"
}

class Asignatura {
    nombre = "EVAS"
    codigo = "056"
}

class UnidadesDidacticas {
    titulo = "Cardio"
}

class ClasesPracticas {
    fecha = "12-11-2024"
}

class ClasesTeoricas {
    fecha = "7-11-2024"
}

Profesor -- Alumno : esTutorDe
Profesor -- Asignatura : imparte
Asignatura -- UnidadesDidacticas : tiene
UnidadesDidacticas -- ClasesPracticas : tiene
UnidadesDidacticas -- ClasesTeoricas : tiene
Alumno -- Asignatura : cursa

@enduml
