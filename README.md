
# Maze RL

This project implements a maze-solving algorithm using Q-Learning, a reinforcement learning technique. The main objective is to navigate through a maze, finding the optimal path from the starting point to the exit. The agent learns this path through repeated trials, gradually improving its decisions by maximizing the cumulative reward.

## Tech Stack

**Lang:** C++

**GUI:** Raylib


## Demo

![alt text](https://github.com/11jolek11/MazeRL/blob/master/maze1.gif)


## How it works

**Maze Representation**: The maze is represented as a grid of cells, where each cell can be either empty (walkable), a wall (non-walkable), a starting point, or an exit.

**Q-Learning**: The agent starts by exploring the maze randomly, updating a Q-table that stores the expected future rewards for each action (moving up, down, left, right) from every state (position in the maze). Over time, the agent learns which actions lead to better outcomes and starts favoring those that maximize rewards.

**Training Process**: The agent undergoes multiple episodes of training. In each episode, it starts from the initial position and tries to reach the exit. The Q-table is updated using the Bellman equation, and exploration is balanced with exploitation using an epsilon-greedy strategy.

**Convergence**: As the training progresses, the agent becomes more adept at finding the optimal path to the exit, eventually being able to solve the maze efficiently.
