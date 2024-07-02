# NEAT

## Description

This repository contains an implementation of the NEAT algorithm (NeuroEvolution of Augmenting Topologies) from scratch. NEAT is a genetic algorithm for the generation of evolving artificial neural networks. The implementation is modular and flexible, allowing you to easily pass a custom fitness function to evolve neural networks tailored to your specific problem.

## Features

- **Modular Design:** Easily integrate your own fitness function to customize the evolutionary process.
- **NeuroEvolution:** Evolve neural networks using genetic algorithms.
- **Topological Innovation:** Supports dynamic growth and complexity of neural networks through mutation operations that add nodes and connections.
- **NumPy Powered:** Efficient numerical computations using the NumPy library.

## Getting Started

### Prerequisites

- Python 3.x
- NumPy
- TensorFlow
- TQDM
- Matplotlib
- Gymnasium
- NetworkX

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/larrie1/neat.git
   cd neat

2. Install the required dependencies:

   ```bash
   pip install numpy tensorflow tqdm matplotlib gymnasium networkx

### Usage

1. Define your fitness function:
   
   ```bash
   def fitness_function(genome):
    # Your custom fitness logic here
    return fitness_score
   
3. Initialize the NEAT algorithm:
   
   ```bash
   neat = NEAT(fitness_function=fitness_function, population_size=100, input_size=5, output_size=2)
   
4. Run the evolutionary process:
   
   ```bash
   best = neat.fit(generations=10, selection_size=20)

5. Plot the results of the best network:

   ```bash
   plot_genom(best, fitness)
