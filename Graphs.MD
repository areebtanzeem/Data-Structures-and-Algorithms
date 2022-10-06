# Graphs

A graph (also called a network) is a data structure that is designed to show relationship between objects. A tree is a specific type of Graph.
Graph Also have noded just like tree but don't have a root node means it suppports cycle.

In Graphs instead just nodes storing the data edges can also store data. Edges often contain data about the strength of a connection.

##  Directions and Cycles

Edges can have a direction, meaning the relationship between two nodes only applies one way and not the other.

**Directed Graph** is a term for graph where the edges have a sense of direction.

Graph can also have **Cycles** in them unlike tress which must not have cycle in them. But it's very dangerous to have a cycle in the graph as when iterating 
through your graph you can run an infinite loop which runs over and over again on a cycle. The graph that don't have any cycle is called **acyclic**

## Connectivity

The term connectivity has a specific meaning  in the study of graphs called **Graph Theory**. Principle of connectivity measures the minimum number of elements that need to be removed for a graph to become disconnected.

### Disconnected

Disconnected graphs are very similar whether the graph's directed or undirected—there is some vertex or group of vertices that have no connection with the rest of the graph.

### Weakly Connected

A directed graph is weakly connected when only replacing all of the directed edges with undirected edges can cause it to be connected. Imagine that your graph has several vertices with one outbound edge, meaning an edge that points from it to some other vertex in the graph. There's no way to reach all of those vertices from any other vertex in the graph, but if those edges were changed to be undirected all vertices would be easily accessible. 

### Connected

Here we only use "connected graph" to refer to undirected graphs. In a connected graph, there is some path between one vertex and every other vertex.

### Strongly Connected

Strongly connected directed graphs must have a path from every node and every other node. So, there must be a path from A to B **AND** B to A.

## Graph Representation

### Edge List

An Edge liist contains list of nodes number which have edge between them or we can say connecting them. This list is the list that ecompasses all the smaller lists. It's also called 2D list. Example of edge list shown below

```
[[1,2],[1,3],[3,4]]
```

This above example states that an edge is in between node 1 and 2, 1 and 4 and so on.

### Adjancy List

An Adjancy list is another way to represent edges in the graph. In this list your vertices have an ID number which corresponds to the index in a array

TO BE COMPLETED FROM OTHER SOURCES

## Eulerian Path

A path that travels through every edge in a graph atlease once. In the basic Eulerian path you start with one node traverse through all edges and might end up in a different node.

Not every Graph is capable of having an Eulerian path

### Eulerian Cycle

In Eulerian Cycle, you must tranverse every edge only once and end up at the same node that you started with. 

## Hamiltonian Path

It is another type of path that must go through every vertex once. Simirlarly a Hamiltonian Cycle will start and end with the same vertex

