**Floyd Warshall Algorithm**

The Floyd Warshall algorithm implements dynamic programming to calculate the length of all shortest paths between two nodes of a graph 
and efficiently solves complex all-pairs shortest path problems.

**The Pseudo-Code for Floyd Warshall algorithm is as follows:**

for k = 0 to n-1
for i = 0 to n-1
for j = 0 to n-1

Distance[i,j] = min(distance[i,j], distance[i,k] + distance[k,j])

where i = start node, j = end node, k = intermediate node.

**The project**

This project uses the imperative version of the Floyd Warshall Algorithm and rewrite the code to use recursion. 

The code works with the following input graph matrix:

**input graph** = [[0, 7, INF, 8],
                * [INF, 0, 5, INF],
                * [INF, INF, 0, 2],
                * [INF, INF, INF, 0]]


**How to run the code?**

Before you run the source code, install the requirements listed in requirements.txt. 
Use the following command in your shell: pip install -r requirements.txt

The folder 'Source code' contains three codes:
1. floyd_imperative_pdf, which is the imperative version provided by the university;
2. floyd_imperative_website, which is the imperative version provided by Geeksforgeeks (available at:
   https://www.geeksforgeeks.org/floyd-warshall-algorithm-dp-16/).
3. floyd_recursive, which is the recursive version of the code.

To run the recursive version of the code, change directory to Source code on your shell terminal and execute $ ./floyd_recursive.py.

The solution graph will be printed in your terminal. It will be as follows:

**solution graph** = [[0, 7, 12, 8],
             *      [INF, 0, 5, 7],
             *      [INF, INF, 0, 2],
             *      [INF, INF, INF, 0]]
