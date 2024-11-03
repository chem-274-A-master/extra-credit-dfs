# Extra Credit : Finding Rings in Graphs

## Background
For the last Problem Set, you used the Python Library NetworkX to represent a molecule as a graph.
For that Problem Set, you found the number of rings in the molecule by using NetworkX functions. 
Under the hood, NetworkX uses graph algorithms to find the rings in the graph.

In graph theory, a cycle (or ring) is a path that starts and ends at the same vertex.
In the context of molecules, rings are important because they can affect chemical properties.
Finding rings is a common problem in cheminformatics and computational chemistry.

Consider the graph in Figure 1 below (from our first homework and Wikipedia).

<center>
<img src="./images/graph_wiki.png">

**Figure 1** - A depiction of a graph with six nodes and seven edges. [source](https://en.wikipedia.org/wiki/Graph_theory)
</center>

This graph has a cycle (ring) that includes nodes 4, 5, 2, and 3.

This may be determined by using graph traversal algorithms like **Depth-First Search (DFS)** or **Breadth-First Search (BFS)**.  
In these algorthims, you start at a node and explore all possible paths until you find a cycle.

## Task 

For this extra credit assignment, you will implement your own algorithm to find rings in a graph using **Depth-First Search (DFS)**.
Your function should take in a NetworkX graph (general graph, it does not need to be the Molecule graph you created in HW3) and return the number of rings in the graph.

The function signature should be

```python
def find_rings(graph: nx.Graph) -> int:
```

You should reference pseudocode for a depth-first ring-finding algorithm on [Wikipedia](https://en.wikipedia.org/wiki/Depth-first_search).

Write your implementation in a file called `extra_credit.py`.
Create a README.md file that includes typical information about the repository (how to install and run the code) and a reflection on the implementation of the ring-finding algorithm.
In your reflection, focus on explaining choices in Python data types and structures you used in order to implement the algorithm and how you tested your code as you developed it.
