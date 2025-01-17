# Maze Algorithm
Maze generation and solver algorithm. 

The maze have 3 types of map
* Normal maze
* Hexagon maze
* Tunnel maze

The maze generation include 3 algorithm, 
* [Kruskal's Algorithm](https://en.wikipedia.org/wiki/Kruskal%27s_algorithm)
* [Prim's Algorithm](https://en.wikipedia.org/wiki/Prim%27s_algorithm)
* [Recursive Backtracking Algorithm](https://en.wikipedia.org/wiki/Backtracking)

The maze solver algorithm include 2 algorithm, 
* [Recursive Backtracking Algorithm](https://en.wikipedia.org/wiki/Backtracking) 
* [Bidirectional Breadth-First-Search Algorithm](https://en.wikipedia.org/wiki/Bidirectional_search).

### Showcase
***Normal Maze***  
![normal](https://github.com/ZankiMaru/maze_algorithm/blob/master/showcase/normal-maze.png)

***Hexagon Maze***  
![hex](https://github.com/ZankiMaru/maze_algorithm/blob/master/showcase/hex-maze.png)

***Recursive Backtracking Maze Solver Algorithm***  
![recur](https://github.com/ZankiMaru/maze_algorithm/blob/master/showcase/recur-solve.gif)

***Bidirectional Breadth-First-Search Maze Solver Algorithm***  
![bidir](https://github.com/ZankiMaru/maze_algorithm/blob/master/showcase/bidir-solve.gif)

### Built With
* [Eclipse](https://www.eclipse.org/) - Framework and IDE used.
* [Java](https://java.com/en/) - Language used.

### Usage
Update the example.txt in src folder first line into: 
>(normal|tunnel|hex) (modiPrim|kruskal|recurBack) (recurBack|biDir) (map height) (map width) (start row) (start column) (finish row) (finish column)

Example:
> hex kruskal recurBack 50 50 0 0 49 49

For tunnel type map, add new line for each tunnel into:  
> (start row) (start column) (finish row) (finish column)

Example:
> tunnel kruskal recurBack 50 50 0 0 49 49  
> 10 10 42 44  
> 25 25 0 25  
> ...

Run the MazeSolver.java with argument line:
> <example.txt location> <y/n maze visualization>

Example:
> src/example.txt y



