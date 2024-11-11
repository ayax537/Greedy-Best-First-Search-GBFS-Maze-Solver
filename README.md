# Greedy-Best-First-Search-GBFS-Maze-Solver
# Overview
This Python script implements the Greedy Best-First Search (GBFS) algorithm to solve a maze using the Turtle graphics library. The program visually represents the maze and the search process, allowing users to observe how the algorithm explores paths to find a solution based on heuristic evaluation.

# Key Components
1. Turtle Graphics Setup
The script creates a Turtle graphics window with:
A black background.
A title "A Maze Solving Program."
Dimensions set to 1300x700 pixels.
2. Maze Representation
The maze is defined using a grid of characters:
+ represents walls.
  (space) represents open paths.
s marks the starting position.
e marks the ending position.
3. Turtle Classes
Five turtle classes are defined to represent different elements of the maze:
Maze (white turtle): Stamps the walls of the maze.
Green turtle: Marks cells that have been visited during the search.
Blue turtle: Indicates frontier cells currently being explored.
Red turtle: Represents the starting position.
Yellow turtle: Represents the ending position and the solution path.
4. Maze Setup Function
The setup_maze function initializes the maze based on the provided grid:
It iterates through each character in the grid, determining the positions of walls, paths, the start, and the end points.
Turtles are moved to their respective positions and stamped to visualize the maze layout.
5. Heuristic Function
The heuristic function calculates the Manhattan distance between a cell and the goal:
This distance is used to prioritize which cells to explore based on their proximity to the end point.
6. GBFS Search Function
The search function implements the Greedy Best-First Search algorithm:
It uses a priority queue (implemented with heapq) to explore cells based on their heuristic distance to the goal.
The algorithm explores possible moves (up, down, left, right) and marks cells as visited.
If a cell is part of the path and has not been visited, it is added to the priority queue for exploration.
The search continues until the end position is reached.
7. Backtracking to Find the Solution Path
The backRoute function is called once the end is reached:
It retraces the path from the end back to the start, marking the solution path with the yellow turtle.
8. Execution Flow
The maze is set up, the GBFS search is performed, and the solution path is visualized.
The program ends when the user clicks on the Turtle graphics window.
# Conclusion
This script serves as an educational tool for understanding how the Greedy Best-First Search algorithm works in the context of maze solving. The visual representation through Turtle graphics makes it engaging and illustrates the algorithm's decision-making process based on heuristic evaluation. Users can modify the grid to test different maze configurations, enhancing their understanding of GBFS.

