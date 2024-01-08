# Maze Runner (maze solver)
![Home Page](./images/maze-image.png?)

## Demo 

[Demo Video](https://youtu.be/YEMhajQu8uQ)

## Introduction

This project is designed to solve mazes by treating them as graphs, where each juncture (intersection) in the maze represents a vertex. The graph is constructed by adding edges between adjacent junctures that are not obstructed by walls. The maze always has a starting point in the upper left corner and an ending point in the lower right corner.

The mazes generated for this project include random weights (ranging from 1 to 9) assigned to edges between adjacent junctures. These weights represent the "cost" of traveling from one juncture to another and are utilized in running Dijkstra's algorithm.

Mazes can be created with varying degrees of "density," from very sparse to "100% dense." The density of the maze determines the presence of walls. A sparse maze has few walls, allowing numerous paths from one juncture to another. Conversely, a maze with "100% density" is densely packed with walls, ensuring there is only one path between any two junctures.

## Maze Solving Approaches

The project employs three distinct approaches to solve mazes. It begins by converting the maze into a graph and subsequently applies standard graph algorithms:

1. **Depth-First-Search**
2. **Breadth-First-Search**
3. **Dijkstra's Algorithm**
   - This algorithm finds the optimal path from the "start" to the "end" by considering the minimal total cost of edges. Notably, the effectiveness of this algorithm is more pronounced in sparse graphs, as "100% dense" graphs offer only one path from start to finish.
