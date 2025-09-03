# 🗺️ Pathfinding Algorithms: A* & Best-First Search 🚀  

This project implements and compares two classic heuristic search algorithms for finding optimal paths in a grid map: **A\*** and **Best-First Search**.  
It is developed in **Java** and works with maps represented as matrices loaded from text files.  

---

## 🔍 Project Description  

- **A\* (A-Star)**: An informed search algorithm that uses a heuristic to find the shortest path from a start node to a goal node, considering both the accumulated cost and the estimated remaining distance.  
- **Best-First Search**: A heuristic-based search that prioritizes expanding the node closest to the goal according to a heuristic function, but does not account for accumulated cost like A\*.  

Maps are implemented through the **MapGrid** class, which loads a matrix from a `.txt` file.  
Nodes are represented by the **Node** class, which stores position, cost, and heuristic information.  

---

## 🛠️ How It Works  

- You can choose between running **A\*** or **Best-First Search** by toggling a flag (`Node.setUseAStar(true/false)`).  
- Example maps are provided in `src/data/matrix.txt` and `src/data/matrix2.txt`.  
- The algorithm searches for a path between a start node and a goal node (e.g., `(0,0)` to `(9,9)`).  
- The console displays:
  - The sequence of nodes in the found path  
  - The total cost  
  - The number of iterations the algorithm took  
- The path is also visualized directly on the printed matrix in the console.  

---

## 📂 Main Code Structure  

- **Main.java** → Entry point; configures the map, start/goal nodes, and runs the selected algorithm.  
- **algorithms.AStar** → Implementation of the A\* algorithm.  
- **algorithms.BestFirstSearch** → Implementation of the Best-First Search algorithm.  
- **heuristics.HeuristicImplementation** → Defines the heuristic function used.  
- **utils.MapGrid** → Manages the grid map and prints the path.  
- **models.Node** → Represents nodes with position, cost, and heuristic data.  
