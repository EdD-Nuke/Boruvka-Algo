# Boruvka-Algo
The provided code implements Boruvka's algorithm to find the Minimum Spanning Tree (MST) of a given connected, undirected, and weighted graph.
Boruvka's Algorithm for Minimum Spanning Tree (MST)
This Python code implements Boruvka's algorithm to find the Minimum Spanning Tree (MST) of a given connected, undirected, and weighted graph. The MST is a subset of edges that connects all vertices in the graph with the minimum possible total edge weight.

Overview
This code defines a Graph class to represent a graph and find its MST using Boruvka's algorithm.
The algorithm starts with each vertex in its own component and repeatedly merges components by adding the cheapest edge connecting them until only one component (the MST) remains.

Usage
Create a Graph object by specifying the number of vertices:
python
Copy code
g = Graph(4)  # Create a graph with 4 vertices
Add edges to the graph using the addEdge method. Each edge should include the source vertex, destination vertex, and edge weight:
python
Copy code
g.addEdge(0, 1, 10)  # Add an edge between vertices 0 and 1 with weight 10
g.addEdge(0, 2, 6)   # Add an edge between vertices 0 and 2 with weight 6
# Add more edges as needed
Calculate and print the Minimum Spanning Tree and its weight using the boruvkaMST method:
python
Copy code
g.boruvkaMST()
Example
In the provided example, a Graph object g is created with 4 vertices, and edges with weights are added to it. Then, the boruvkaMST method is called to find and print the Minimum Spanning Tree and its weight.

Structure
Graph class: Represents the graph and contains methods for adding edges, finding components, and computing the MST.
addEdge: Adds edges to the graph.
find and union: Utility functions for component management.
boruvkaMST: The main function that constructs the MST using Boruvka's algorithm.
Output
The code prints the edges included in the MST along with their weights and the total weight of the MST.

License
This code is provided under the MIT License.

Credits
Adapted from an original implementation.
