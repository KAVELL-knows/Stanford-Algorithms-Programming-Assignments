# Generic-Code-for-Datastructures-and-Algorithms
This repository comprises of all my Programming Assignments for the 4 courses on Stanford Algorithms Specialization Course


# Strongly Connected Components

Implementation of **Kosaraju's algorithm** for finding strongly connected
components in a directed graph.

## Algorithm

Kosaraju's algorithm uses two DFS passes:

1. Reverse all edges in the graph.
2. Run DFS on the reversed graph and record vertices by finishing time.
3. Process vertices in decreasing order of finishing time.
4. Run DFS on the original graph.
5. Each DFS in the second pass finds one strongly connected component.

## Complexity

- Time: O(V + E)
- Space: O(V + E)

## Implementation

The implementation uses iterative DFS instead of recursion to avoid
recursion-depth problems on large graphs.
