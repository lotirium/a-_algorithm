# A* Path Finding Algorithm Project

This project implements the A* pathfinding algorithm using Python and Pygame. The A* algorithm is widely used for pathfinding and graph traversal, which is the process of finding the most efficient path between multiple points, called nodes.

## Features

- **Visual Grid**: A grid layout that allows users to visualize the algorithm in action.
- **Interactive Nodes**: Users can interact with the grid to set start and end points, and create barriers.
- **Color-coded Nodes**: Each node type (start, end, barrier, path, etc.) has a unique color for easy identification.
- **Real-time Pathfinding**: Watch the algorithm find the shortest path in real-time.

## Requirements

- Python
- Pygame library

## Installation

1. Ensure Python is installed on your system.
2. Install Pygame: `pip install pygame`
3. Download the project files to your local machine.

## Usage

Run the script using Python:

```bash
python main.py
```

### Controls

- **Left Mouse Click**: Set start node, end node, or draw barriers.
- **Right Mouse Click**: Remove nodes or barriers.
- **Space Bar**: Start the algorithm.
- **C Key**: Clear the grid and reset.

## Code Explanation

- `Node` class: Represents each node in the grid.
- `make_grid`: Creates a grid of `Node` objects.
- `draw_grid`: Draws grid lines on the window.
- `draw`: Handles drawing the grid and nodes.
- `get_clicked_pos`: Translates a mouse position to grid coordinates.
- `main`: Main loop for running the application.

### Algorithm Function

- `algorithm`: Contains the implementation of the A* algorithm.
- `heuristic_function`: Calculates the Manhattan distance, used as the heuristic in A*.
- `reconstruct_path`: Reconstructs the path from the end node to the start node.
