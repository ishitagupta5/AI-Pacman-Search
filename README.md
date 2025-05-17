# AI-Pacman-Search
A Python AI project implementing classical search algorithms like DFS, BFS, UCS, and A* to solve pathfinding problems in the Pacman world and the 8-puzzle. Based on UC Berkeley’s CS188: Introduction to AI.

## Overview

You will implement the following algorithms:

- Depth-First Search (DFS)
- Breadth-First Search (BFS)
- Uniform Cost Search (UCS)
- A* Search (with heuristics like Manhattan distance)

These algorithms are used to control agents that solve navigation problems in a grid-based maze and the sliding tile 8-puzzle.

## Directory Structure

- `search.py`: Core search algorithm implementations (to be completed by students)
- `search_agents.py`: Agents that use your search algorithms to solve mazes
- `eight_puzzle.py`: Logic for the 8-puzzle problem
- `pacman.py`: Main game logic and entry point for running the Pacman environment
- `game.py`, `layout.py`, `ghost_agents.py`, `pacman_agents.py`, `keyboard_agents.py`: Game infrastructure
- `graphics_display.py`, `graphics_utils.py`, `text_display.py`: Graphical and text-based UI rendering
- `autograder.py`, `grading.py`, `test_classes.py`, `test_parser.py`, `search_test_classes.py`, `submission_autograder.py`: Autograder and test infrastructure
- `util.py`: Utility classes and functions including data structures
- `project_params.py`: Configuration for the autograder
- `layouts/`: Maze layout definitions
- `test_cases/`: XML test case files
- `commands.txt`: Example command-line instructions

## Getting Started

To run Pacman using DFS:
```bash

python pacman.py -l tinyMaze -p SearchAgent -a fn=depth_first_search
```
To run Pacman using BFS:
```bash
python pacman.py -l mediumMaze -p SearchAgent -a fn=breadth_first_search
```
To run Pacman using UCS:
```bash
python pacman.py -l mediumMaze -p SearchAgent -a fn=uniform_cost_search
```
To run Pacman using A* Search with Manhattan heuristic:
```bash
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar_search,heuristic=manhattan_heuristic
```
To run the 8-puzzle:
```bash
python eight_puzzle.py
```

To run all autograder tests:
```bash
python autograder.py
```
