In this repository, I added 2 of my AI mini-projects for the Artificial Intelligence course. The first one is PacMan game using Q-learning and the second one is CuttongStockProblem with approximate algorithms. Here is the more detailed explanation:

---------------------------------------

# Pacman Q-Learning Project

## Overview

This project demonstrates how to solve the Pacman game using Q-learning, a reinforcement learning technique. The objective is to guide an agent through a grid-based environment, collecting all the dots while avoiding walls and ghosts.
The environment is discretized into small unit squares, and the agent must navigate these squares to achieve the goal.

## Project Structure

- **Agent:** Represents Pacman, which moves within the environment.
- **Environment:** Consists of dots to collect, walls to avoid, and ghosts to evade.
- **Q-Learning:** The algorithm used to train the agent to make optimal decisions based on the state and rewards.

## Environment Details

- **W:** Wall - impassable blocks.
- **A:** Agent - the starting position of Pacman.
- **D:** Dot - collectible items that Pacman must gather.
- **G:** Ghost - enemies that Pacman must avoid.
- **E:** Empty cell - a cell becomes empty after the dot is collected.

## Key Concepts

1. **States:**
   - Defined by the position of the agent, the remaining dots, and the position of the ghosts.
   - The number of states depends on the grid size and the number of dots and ghosts.

2. **Actions:**
   - Possible movements for the agent: Up, Down, Left, Right.
   - Actions are chosen based on the Q-values, which are updated through the Q-learning algorithm.

3. **Rewards:**
   - Positive reward for collecting a dot.
   - Negative reward for hitting a wall or encountering a ghost.
   - The goal is to maximize the cumulative reward by collecting all dots while avoiding penalties.

4. **Q-Table:**
   - A table that stores the Q-values for each state-action pair.
   - The agent uses the Q-table to decide the best action to take in a given state.

5. **Gamma (γ):**
   - The discount factor, which determines the importance of future rewards.
   - Analyze the effect of different gamma values (e.g., 0.25, 0.5, 1) on the learning process.

6. **Alpha (α):**
   - The learning rate, which controls how much new information overrides old information.
   - Experiment with different alpha values to observe the impact on learning efficiency.

- **Graphical Representation:**
  - Display the environment as a weighted graph, with vertices representing states and edges labeled with corresponding actions and rewards.

- **Episode and Reward Visualization:**
  - Graphically display the rewards and episodes resulting from different actions in each state.


## Usage

- **Training:**
  - The agent will be trained using Q-learning to navigate the environment and collect all dots.
  - The impact of different gamma and alpha values can be analyzed by modifying the parameters in the code.

- **Testing:**
  - Test the trained agent on various environments to observe its performance.

## Results

- The Q-Table is generated during training, showing the optimal action for each state.
- Graphical representations of the environment and the agent's actions are available.
- Performance can be evaluated based on the cumulative rewards and the agent's success in collecting all dots.


----------------------------------------
# Cutting Stock Problem

## Overview

This project solves the Cutting Stock Problem, a classic optimization challenge that involves cutting stock materials (e.g., rolls of paper) into specified sizes while minimizing material wastage. 
This problem is NP-hard, making it computationally complex. The objective is to fulfill specific size requests using the minimum number of stock materials.

The project implements three optimization algorithms: **Genetic Algorithm, Simulated Annealing,** and **Hill Climbing** to find efficient cutting strategies for different sets of requests.

## Project Structure

- **Input:** Stock material rolls of standard lengths.
- **Requests:** Specific sizes of rolls that need to be cut from the stock.
- **Objective:** Minimize the number of stock rolls used while fulfilling all requests.

## Algorithms Used

1. **Genetic Algorithm:**
   - Mimics the process of natural selection by evolving a population of solutions over generations.
   - Uses crossover, mutation, and selection operators to improve the cutting strategies.

2. **Simulated Annealing:**
   - Inspired by the annealing process in metallurgy, where a material is heated and then slowly cooled to remove defects.
   - Uses a probabilistic approach to escape local optima and find a global optimum solution.

3. **Hill Climbing:**
   - An iterative optimization algorithm that starts with an arbitrary solution and makes small changes to improve it.
   - Continues to climb "uphill" until no better solution is found.

## Problem Instructions

The task is to find cutting solutions for the following inputs:

- **Input 1:** Find a way to cut that uses less than 56 rolls.
- **Input 2:** Find a way to cut that uses less than 80 rolls.
- **Input 3:** Find a way to cut that uses less than 115 rolls.
- **Input 4:** Find a way to cut that uses less than 235 rolls.

Each input represents a different level of complexity, requiring the algorithms to generate efficient cutting patterns that meet the specified roll limits.

