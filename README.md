# 🧬 Genetic Algorithm Text Evolver

This project simulates a **Genetic Algorithm** designed to evolve a random string into a predefined **TARGET** using biological-inspired operations like selection, crossover, and mutation.

> **Course:** Computational Cognitive Science – AI-332  
> **University:** Cairo University – Faculty of Computer Science and AI  
> **Year:** 2024  

---

## 📋 Assignment Overview

The Genetic Algorithm (GA) operates on a population of strings ("chromosomes") and attempts to evolve them into the TARGET string using:

- ✅ **Initialization** – Generate a population of random chromosomes using predefined characters.
- 🧠 **Fitness Calculation** – Evaluate how close each chromosome is to the TARGET.
- 🥇 **Selection** – Choose the top 50% based on fitness.
- 🔀 **Crossover** – Mate selected chromosomes to create offspring.
- 🧬 **Mutation** – Introduce random gene changes based on a mutation rate.
- 🔁 **Replacement** – Combine best old chromosomes with new generation.

The cycle repeats until the TARGET string is matched exactly.

---

## 🔧 How It Works

### Constants
- `GENES`: Characters used to form chromosomes.
- `TARGET`: The string we want the algorithm to evolve.
- `POP_SIZE`: Number of chromosomes in the population.
- `MUT_RATE`: Mutation probability for each gene.

### Key Functions

| Function       | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `initialize_population()` | Creates an initial population of random chromosomes.                   |
| `calculate_fitness(pop)` | Computes fitness as the number of character mismatches with TARGET. |
| `select(pop_with_fitness)` | Keeps the top 50% based on fitness score.                            |
| `crossover(parents)`       | Mates selected chromosomes to create offspring.                     |
| `mutate(children)`         | Randomly changes genes based on `MUT_RATE`.                         |
| `replace(old, new)`        | Combines best individuals from old and new generations.             |

---

## ▶️ How to Run

```bash
python genetic_algorithm.py

