# Genetic Algorithm for the Traveling Salesman Problem (TSP)

**Java · Evolutionary Computing · Route Optimization · Maven**

## Overview / Descripción

**EN:** Academic team project exploring an evolutionary approach to the Traveling Salesman Problem. Each candidate solution represents an ordering of cities to visit, and the program evaluates the route distance, including departure from and return to Madrid. The implementation evolves a population with inversion and swap operations, retaining improved candidates. It also implements uniform crossover and displays the resulting offspring for inspection.

**ES:** Proyecto académico en equipo que explora un enfoque evolutivo para el problema del viajante. Cada solución representa un orden de visita de ciudades y el programa evalúa la distancia de la ruta, incluyendo la salida y el regreso a Madrid. La implementación modifica una población mediante operaciones de inversión e intercambio, conservando las soluciones mejoradas. También implementa un cruzamiento uniforme y muestra los descendientes obtenidos para su análisis.

## Features / Funcionalidades

- Reads a distance matrix, cities and algorithm parameters from a text file. / Lee una matriz de distancias, ciudades y parámetros desde un fichero de texto.
- Generates a randomized initial population of routes. / Genera una población inicial aleatoria de rutas.
- Applies inversion and swap operators to candidate routes. / Aplica operadores de inversión e intercambio.
- Compares distances and retains non-worsening candidate routes. / Compara distancias y conserva candidatos que no empeoran el recorrido.
- Implements uniform crossover and prints offspring; **the generated offspring are not inserted into the population in the current code**. / Implementa cruzamiento uniforme y muestra descendientes; **en el código actual estos descendientes no se incorporan a la población**.
- Reports generation statistics and final results. / Muestra estadísticas por generación y resultados finales.

## Technologies / Tecnologías

Java, Maven, object-oriented programming, evolutionary operators.

## Structure / Estructura

```text
├── pom.xml
├── DatosPru1.txt
├── DatosPru2.txt
├── DatosPru3.txt
└── src/main/java/es/upm/etsisi/SI/
    ├── Viajante.java    # Evolution loop, input parsing and entry point
    └── Individuo.java   # Candidate route representation and operators
```

## How to run / Cómo ejecutarlo

1. Install **JDK 23** (the supplied `pom.xml` sets Java source/target to 23) and Maven, or adjust the compiler version after checking compatibility.
2. From the repository root, compile:

   ```bash
   mvn compile
   ```
3. Run the program **from the repository root**, where `DatosPru1.txt` is located:

   ```bash
   java -cp target/classes es.upm.etsisi.SI.Viajante
   ```

The current `main` method loads `DatosPru1.txt` directly. To use `DatosPru2.txt` or `DatosPru3.txt`, change the filename in `Viajante.main` and recompile. / El método `main` carga directamente `DatosPru1.txt`. Para utilizar otro fichero, cambia el nombre en `Viajante.main` y vuelve a compilar.

## Academic context / Contexto académico

Collaborative university coursework in artificial intelligence / evolutionary optimization at Universidad Politécnica de Madrid (UPM). / Trabajo académico colaborativo de la Universidad Politécnica de Madrid (UPM).

> Note / Nota: This is an educational implementation; no optimality guarantee or benchmarking results are claimed. / Se trata de una implementación académica; no se afirma que garantice un óptimo ni se atribuyen resultados experimentales no documentados.
