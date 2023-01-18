# DAA_CIA1
Judah's submission for DAA CIA 1 assignment.

My Choice of Programming Language:
I chose Java as my primary language mainly because of it's portability. All I need to do is write the code once and run it anywhere I want thanks to the Java Virtual Machine. It makes deployment of applications using containers (through an application like docker) so much more easier and faster. I also choose to use Java because of it's memory management and simplicity of using variables through reference as there's no pointers to be confused about.

Algorithm: Prim's
What: Greedy Algorithm
Why: To find minimum spanning tree (MST)
How: From an initialize MST find minimum edges and add it to the tree
Where: Non-Negative weighted undirected graphs
Who: Prim

Algorithm: Kruskal's
What: Greedy Algorithm
Why: To find minimum spanning tree
How: Notes down all weights of pairs and start constructing the MST, if an edge pair forms a cycle in the MST, that edge is not cosidered.
Where: Non-negaltive weighted undirected graphs
Who: Kruskal

Algorithm: Dijkstra's
What: Greedy Algorithm
Why: To find single-source shortest path for a weighted graph
When: Used in Google maps to find the shortest single path between 2 locations
How: One node is vertex, and then checks all adjacent vertices with the lowest weight, then that node connected to the prime vertex with the lowest weight becomes the new prime vertex and so on.
Where: Mostly in Non-Negative weighted directed graphs. But can also work in negative weighted edges as long as while forming a cycle, there's no negative edge.
Who: Dijkstra
Note: Dijkstra's algorithm fails to find the shortest path if in a cycle there exists a negative weight, as the problem with this algorithm is that once a node/vertex is visited it will not be revisited for further more effected path changes.

If none of the above algorithms can effectively solve to find the shortest path from the source node to every other node reliably, which algorithm would be used bring out a reliable outcome?
Ans: Bellman-Ford Algorithm

Even though Dijkstra's algorithm works on negative weighted directed graphs as long as there is no negative weigted cycles being formed, Bellman-Ford is the algorithm that can be used to find the shortest path even if there is a negative weighted cycle being formed. It is worth noting that while Dijkstra's algorithm might be faster, the Belmann-Ford algorithm is more versatile.
