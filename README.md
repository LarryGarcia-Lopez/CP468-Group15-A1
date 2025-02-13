This repository contains Python scripts designed to solve two classic sliding puzzles, the 8-puzzle and the 15-puzzle, using the A* search algorithm with three different heuristics. The aim is to evaluate the effectiveness of each heuristic in solving randomly generated puzzles of increasing complexity.

Project Files
1. task1.py: Solves the 8-puzzle using A* algorithm with three different heuristics.
2. task2.py: Solves the 15-puzzle using A* algorithm with three different heuristics.

Heuristics Used
1. Misplaced Tiles (h1): Counts the number of tiles that are not in their correct position.
2. Manhattan Distance (h2): Calculates the total Manhattan distance (sum of vertical and horizontal distances) of all tiles from their goal positions.
3. Euclidean Distance (h3): Computes the Euclidean distance (straight-line distance) for all tiles from their target positions.

Features
1. PuzzleState Class: Represents the state of a puzzle, including its board configuration, number of moves made, and previous state.
2. A Search Implementation*: Utilizes the A* search algorithm to find the shortest path from a given puzzle state to the goal state using the specified heuristic.
3. Random State Generation: Generates random, solvable states for the puzzles to test the efficiency of the heuristics.

Usage
- To use either script, ensure Python is installed on your system and run the desired script via the command line:
    python task1.py
    python task2.py

Performance Analysis
- Each script generates 100 random solvable states of the puzzle and solves them using each of the three heuristics. The scripts measure and output the average number of steps to solve the puzzles and the average number of nodes expanded during the search process. This data is used to compare the efficiency of the heuristics in terms of computational resources and time complexity.

Requirements
- Python 3.x
- NumPy library