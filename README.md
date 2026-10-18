# Minimum Spanning Tree (MST) – Prim's Algorithm

A Python implementation of **Prim's Algorithm** to compute the Minimum Spanning Tree (MST) on undirected, weighted graphs, utilizing both **Adjacency Matrix** and **Adjacency List** representations.

---

## Problem Overview
Given a connected, undirected graph with positive edge weights, the objective is to find a tree subgraph that spans all vertices while minimizing the total sum of edge weights without creating cycles.

---

## Algorithmic Logic: Prim's Greedy Approach
- **Initialization:** Choose an arbitrary starting vertex (e.g. node `'A'`) and mark it as visited.
- **Greedy Step:** At each iteration, identify the minimum-weight edge $(u, v)$ crossing the cut — connecting any visited vertex $u$ to an unvisited vertex $v$.
- **Expansion:** Mark vertex $v$ as visited, add $(u, v)$ to the MST, and accumulate the weight.
- **Termination:** The process repeats until exactly $\vert{}V\vert{} - 1$ edges are selected, spanning all $\vert{}V\vert{}$ vertices.
