# Lista-de-vuelos-Prueba-Tecnica-2

# Descripción

Este proyecto es una aplicacion sencilla desarrollada en Java que permite filtrar una lista de vuelos segun distintos criterios de busqueda basados en fechas.
El programa primero muetra la lista completa de vuelos creados en el sistema. 
Después aplica el filtro según las fechas indicadas y muestra los vuelos que cumplen con el criterio.

## Tecnologia utilizadas
-Java
-JDK 17
-API "LocalDate"
-Streams de Java
-IntelliJ IDEA

## Estructura del proyecto

El proyecto está organizado en diferentes paquetes para separar responsabilidades:

# Entities
Contine la clase "Vuelo", que representa la entidad del sistema con toda la informacion de cada vuelo.

# Utils
Contiene la clase "VueloUtils" que incluye la logica para filtrar los vuelos segun las fechas indicadas.

# Main
Es la clase principal del programa donde:
- se definen las fechas de filtrado
- se creanlos vuelos de prueba
- se ejecuta la funcion de filtrado
- se muestra los resultados en la terminal
  
## Funcionamiento del filtro
El programa utiliza dos constantes de fecha en la clase "Main":
-fechaInicio
-fechaFin

Dependiendo de si estas fechas están definidias o son "null" el filtro se comporta de la siguiente manera: 

- si no se envia ninguna fecha, se devuelven todos los vuelos.
- Si solo se envia fechaFin, se devuelven los vuelos hasta esa fecha.
- Si solo se envia fechaInicio, se devuelven los vuelos desde esa fecha en adelante.
- Si se envian ambas fechas, se devuelven los vuelos dentro de ese rango.

## Ejecucion del programa
1. Abrir el proyectoen un IDE de Java
2. Ejecutar la clase "Main"
3. Los vuelos filtrados se mostrarán en la consola.
