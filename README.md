The Floyd Warshall algorithm implements dynamic programming to calculate the length of all shortest paths between two nodes of a graph and efficiently solves complex all-pairs shortest path problems.
This project uses the imperative version of the Floyd Warshall Algorithm and rewrite the code to use recursion. 
The code works with the following input graph matrix and computes the shortest path from start node i to end node j passing through intermediate node k.
input graph = [[0, 7, INF, 8],
               [INF, 0, 5, INF],
               [INF, INF, 0, 2],
               [INF, INF, INF, 0]]

The Pseudo-Code for Floyd Warshall algorithm is as follows:
for k = 0 to n-1
for i = 0 to n-1
for j = 0 to n-1
Distance[i,j] = min(dist[i,j],dist[i,k] + dist[k,j]
where i = tart node, j = end node, k = intermediate node.

The solution graph is as follows:

output graph = [[0, 7, 12, 8],
                [INF, 0, 5, 7],
                [INF, INF, 0, 2],
                [INF, INF, INF, 0]]
