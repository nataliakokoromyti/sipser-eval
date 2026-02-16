# Solution: Exercise 0.14

## Solution
Step 1:
Consider the graph G. A clique is a subgraph of G in which every pair of vertices are connected. An anti-clique is a subgraph in which in which every
pair of vertices are not connected.

Step 2:
In order to show that every graph with n vertices contains either clique or anti-clique with at least vertices, create two piles A and B to store
the vertices of a graph. Here, the pile A contains the vertices of a clique whereas the pile B contains the vertices of an anti-clique.
Procedure to identify a clique or an anti-clique is as follows:
• Take each vertex v of the graph G.
• If the degree of the vertex is greater than one half of the remaining vertices then add the vertex to pile A. Otherwise, add the vertex to the pile B.
• Discard all vertices to which v is not connected if it was added to the pile A.
• Discard all vertices to which v is connected if it was added to the pile B.
• Continue this procedure until no vertices left.
Consider the whole procedure as a step. For each step, at most half of the vertices are discarded. Thus, at least steps occur before
completion of the process. Each step adds a vertex to one of the piles. Thus, one of the piles contains at least vertices.
Therefore, it is proved that that every graph with n vertices contains either clique or anti-clique with at least vertices.
