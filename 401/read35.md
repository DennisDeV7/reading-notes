# Graphs

## Vocabulary

- Vertex: a data object that can have zero or more adjacent vertices
- Edge: a connection between two nodes
- Neighbor: nodes that are adjacent to each other and connected by an edge
- Degree: number of edges connected to a vertex
- Undirected Graph: a graph in which the edges are undirected
- Directed Graph: (Digraph) a graph in which every edge has a direction to a node
- Completed Graph: all nodes are connected to all other nodes
- Connected Graph: all vertices have at least one edge
- Disconnected Graph: some nodes do not have edges
- Cycle: when traversing through a graph has the potential to end on the node that it started with
- Acyclic Graph: a graph that does not have cycles
- Cyclic Graph: A graph that has cycles
- Adjacency Matrix: Can be represented through a 2-dimensional array. Each vertex of the data structure is represented by a row and column in the array.
- Adjancency List: a collection of linked lists that show the other vertices that are connected. This is the most common way to represent a graph.
- Weighted Graph: a graph with numbers assigned to the edges

### Traversals

- Breadth first: similar to traversing a tree, using a queue, except a graph can have cycles
- Depth first: Uses a Stack to visit all the children of subtrees