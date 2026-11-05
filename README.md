# Heuristic Optimization — Gurobi, Genetic Algorithm & Simulated Annealing

**Yuan Ze University | Term Project | June 2025**

A course group project studying an optimization problem involving salespersons, cities, and depots. The project compares a mathematical optimization approach implemented with **Gurobi** against **Genetic Algorithm (GA)** and **Simulated Annealing (SA)** approaches, and visualizes selected route solutions for benchmark **Instances 0 and 3**.

## Project overview

The supplied Gurobi notebooks read datasets describing cities, depots, and salespersons. Model data includes geographic coordinates, salesperson travel speeds, service durations, and color/assignment attributes. The mathematical model formulates route-selection decisions and minimizes a sum of travel and service times subject to modeled constraints. The accompanying GA/SA visualization notebook plots routes from stored chromosome solutions.

## Methods and tools

| Area | Method / technology |
| --- | --- |
| Mathematical optimization | Gurobi (`gurobipy`) |
| Heuristic approaches | Genetic Algorithm (GA), Simulated Annealing (SA) |
| Programming | Python, Jupyter notebooks exported as HTML |
| Data processing | pandas, NumPy |
| Visualization | Matplotlib |
| Benchmarks | Instance 0 and Instance 3 |

## Repository contents

```text
Heuristic-Optimization-Gurobi-GA-SA/
├── Gurobi/
│   ├── SourceCodeGurobi_Instance0.html
│   └── SourceCodeGurobi_Instance3.html
├── GA-SA/
│   ├── SourceCode_GAAndSA_Instance0.txt          # add if available
│   └── SourceCode_GAAndSA_Instance3.txt          # add if available
├── Visualization/
│   └── Visualization_GAAndSA_Instance0andInstance3.html
└── README.md
```

*The three HTML exports were available for review. The GA/SA source TXT files and the final PDF report were named in the course submission record but were not supplied for verification here. Remove missing entries or upload those files to match this structure.*

## Project workflow

1. **Prepare benchmark inputs:** Read cities, depots, and salesperson data for each instance.
2. **Formulate a mathematical model:** Define the routing decisions and constraints, then solve using Gurobi.
3. **Explore heuristic solutions:** Apply GA and SA as alternative solution methods (see source TXT files when added).
4. **Visualize routes:** Display routes, city positions, and depot positions for Instances 0 and 3.
5. **Compare results:** Use the course report to document solution quality, run time, and observations, when available.

## Viewing and reproducing the work

- Open the `.html` files in a web browser to inspect the exported notebooks and visualizations.
- To execute the Python code, work from the original notebooks or extract the code into `.py`/`.ipynb` files.
- Install relevant libraries in your Python environment:

  ```bash
  pip install numpy pandas matplotlib gurobipy
  ```

- A **valid Gurobi license** may be required to solve the optimization models.
- Obtain the corresponding instance input files (for example, `Cities_0.txt`, `Depots_0.txt`, `Salespersons_0.txt`, and their Instance 3 equivalents).
- Replace the original author-machine absolute file paths in the code with paths on your computer.
- The visualization notebook also expects output files containing final chromosome/route solutions. Those files need to be available to reproduce the plots.

## Notes and limitations

- These are **HTML exports** of notebooks, not standalone web applications.
- The provided source contains local absolute paths; the repository alone is not yet a one-click runnable package.
- Quantitative claims about which method performs best should be taken from the final project report and confirmed against the original results; no improvement percentage is asserted here.
- This was a **group term project**. Individual contributions should be credited accurately rather than attributing all work to one person.

## Academic context

Submitted as a **Term Project Report**, due **June 22, 2025**, with a report, Gurobi source exports, GA/SA source files, and route visualizations. Upload the final report only if all team members agree to public sharing.
