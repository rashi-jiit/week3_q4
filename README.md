I found an open-source C project on GitHub that implements Dijkstra's algorithm. The project is called Dijkstra-C by Maximetinu. This implementation supports reading the adjacency matrix from a file or terminal input and provides output in the same manner. It includes features for generating graph visualizations using Graphviz.

## Code Structure and Function Documentation
## dijkstra.h

## Purpose: 
This file contains the core logic for Dijkstra's algorithm.
## Functions:
dijkstra(int n, int startnode, int endnode, int graph[MAX][MAX]): Calculates the shortest path from the start node to the end node.
initialize_single_source(): Initializes the distance and predecessor arrays.
extract_min(): Extracts the node with the minimum distance from the queue.
relax(): Updates the distance and predecessor if a shorter path is found.
IO_dijkstra.h

## Purpose: 
Handles input and output operations.
## Functions:
read_graph_from_file(): Reads the graph's adjacency matrix from a file.
write_result_to_file(): Writes the shortest path results to a file.
print_graph(): Prints the adjacency matrix to the terminal.
print_result(): Prints the shortest path results to the terminal.
graph_drawer.h

## Purpose: 
Interfaces with Graphviz to draw the graph and the shortest path.
## Functions:
draw_graph(): Uses Graphviz to draw the entire graph.
draw_shortest_path(): Uses Graphviz to highlight the shortest path on the graph.
main.c

## Purpose:
The main entry point of the program, managing the overall flow.
## Functions:
main(): Handles command-line arguments, initializes necessary components, and calls functions to execute the algorithm and handle I/O.
