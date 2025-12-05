# Metaheuristic Optimization for a Real-World Problem

This project applies Genetic Algorithm (GA) and Ant Colony Optimization (ACO) to solve a real-world Traveling Salesman Problem (TSP) instance using the eil76 dataset from TSPLIB. The work follows the CS1463 project requirements and the methodology described in our proposal.

---

##  Project Overview

The Traveling Salesman Problem (TSP) aims to find the shortest route that visits each city exactly once. Because TSP is NP-hard, metaheuristic methods are commonly used to find strong approximate solutions efficiently. In this project, we implement and compare:

- **Genetic Algorithm (GA)**  
- **Ant Colony Optimization (ACO)**  

Both algorithms are implemented from scratch.

---

## Repository Contents
Metaheuristic-Optimization-for-a-Real-World-Problem
- Metaheuristic_Optimization_Proj.ipynb        # Full Colab notebook
- Metaheuristic_Optimization_Proj - Colab.pdf  # PDF version
- metaheuristic_optimization_proj.py           # Python script version

- eil76.tsp                                    # Dataset (76-city TSP)

- Names                                        # Team members
-  README.md                                    # This file
---

## Methods Used

### Genetic Algorithm (GA)
- Representation: permutation of city indices  
- Crossover: order-based crossover  
- Mutation: swap mutation  
- Selection: tournament / roulette-wheel (parameter dependent)  
- Fitness = total tour distance  

### Ant Colony Optimization (ACO)
- Ants construct tours based on pheromone + heuristic visibility  
- Pheromone evaporation and global updates  
- Probabilistic movement between cities  
- Tracks best solution across iterations  

---

## Dataset

**eil76.tsp**  
- 76 cities  
- Euclidean distances  
- Standard TSPLIB benchmark used widely in optimization research  

---

## Results Summary

- GA best tour length ≈ **1736**  
- ACO best tour length ≈ **555** (scaled based on dataset definition)

The notebook includes:
- Convergence plots  
- Final generated tours visualized for both algorithms  

---

## ✔ Requirements Satisfaction

This project fulfills the CS1463 requirements by:

- Choosing a real-world optimization problem (TSP)  
- Implementing two metaheuristic algorithms from scratch  
- Using a real dataset  
- Providing full code, report, and comparison  
- Matching the scope and methods described in the original proposal  

---

##  Team Members

See the **Names** file:  
- Reyam  
- Rana  
- Deema  
- Munira  

---

## How to Run

### Option 1: Google Colab  
Open and run the notebook.

### Option 2: Local Python Script
Ensure `eil76.tsp` is in the same directory, then run:
