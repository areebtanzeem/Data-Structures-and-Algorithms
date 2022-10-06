# Graphs

A graph (also called a network) is a data structure that is designed to show relationship between objects. A tree is a specific type of Graph.
Graph Also have noded just like tree but don't have a root node means it suppports cycle.

In Graphs instead just nodes storing the data edges can also store data. Edges often contain data about the strength of a connection.

##  Directions and Cycles

Edges can have a direction, meaning the relationship between two nodes only applies one way and not the other.

**Directed Graph** is a term for graph where the edges have a sense of direction.

Graph can also have **Cycles** in them unlike tress which must not have cycle in them. But it's very dangerous to have a cycle in the graph as when iterating 
through your graph you can run an infinite loop which runs over and over again on a cycle. The graph that don't have any cycle is called **acyclic**
