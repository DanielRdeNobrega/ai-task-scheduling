# AI Task Scheduling and Resource Optimization

**Python · Branch and Bound · A* Search · Genetic Algorithms · RCPSP**

## Overview / Descripción

**EN:** Academic team project exploring the Resource-Constrained Project Scheduling Problem (RCPSP). The program schedules tasks with precedence relationships, durations and limited shared resources. It provides exercises based on Branch and Bound, A* search and an evolutionary approach, with makespan as a key evaluation measure.

**ES:** Proyecto académico en equipo que explora el problema de planificación de proyectos con recursos limitados (RCPSP). El programa planifica tareas con dependencias, duraciones y recursos compartidos limitados. Incluye ejercicios basados en Branch and Bound, búsqueda A* y un enfoque evolutivo, utilizando el tiempo total de ejecución (*makespan*) como medida de evaluación.

## Features / Funcionalidades

- Four predefined RCPSP instances (`rcpsp06`, `rcpsp07`, `rcpsp10`, `rcpsp30`). / Cuatro instancias predefinidas del problema.
- Branch and Bound search. / Búsqueda por ramificación y acotación.
- A* search and heuristic scheduling. / Búsqueda A* y planificación heurística.
- Genetic algorithm exercise with selection, crossover and mutation. / Ejercicio de algoritmo genético con selección, cruzamiento y mutación.
- Checks for resource limits and task dependencies in search exercises. / Comprobaciones de recursos y dependencias en los ejercicios de búsqueda.
- Schedule visualization using Matplotlib. / Visualización de la planificación con Matplotlib.

## Technologies / Tecnologías

Python, search algorithms, evolutionary algorithms, Matplotlib.

## Structure / Estructura

```text
src/
├── main.py                            # Interactive menu / Menú interactivo
├── upmproblems/                       # Scheduling problem instances
├── upmsearch/search_exercises.py      # Branch and Bound, A*
├── upmevo/evo_exercises.py            # Evolutionary exercise
└── utils/                             # Helpers, algorithms, plots
```

## How to run / Cómo ejecutarlo

1. Install Python 3 and Matplotlib:

   ```bash
   python -m pip install matplotlib
   ```
2. **From the repository root** (the folder containing `src/`), run:

   ```bash
   python -m src.main
   ```

3. Choose a problem instance and an exercise from the interactive menus. / Selecciona una instancia y un ejercicio mediante los menús.

**Important / Importante:** The included source uses both `src.utils...` and top-level `upmproblems...` imports. Depending on the Python environment, the command may require an adjusted module path or consistent import statements. A commonly useful alternative from the repository root is:

```bash
PYTHONPATH=.:src python src/main.py
```

On Windows PowerShell / En PowerShell:

```powershell
$env:PYTHONPATH=".;src"
python src/main.py
```

The above launch methods are based on inspection of the imports; they are not a claim that every runtime dependency or exercise has been tested. / Estos comandos se basan en la revisión de las importaciones; no implican que se hayan probado todas las dependencias o ejercicios.

## Academic context / Contexto académico

Collaborative university work at Universidad Politécnica de Madrid (UPM). / Trabajo universitario colaborativo de la Universidad Politécnica de Madrid (UPM).

> Note / Nota: This is an educational implementation and does not guarantee an optimal result for every instance or algorithm. / Implementación académica que no garantiza resultados óptimos en todas las instancias o algoritmos.
