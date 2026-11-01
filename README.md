
# Advanced DSA Engineering Sprint

## Overview

This project solves three advanced algorithmic challenges
using graph algorithms, dynamic programming, and optimization.

## 1. Graph Problem - Network Route Optimizer

**Algorithm:** Dijkstra's Shortest Path

- Uses adjacency lists.
- Uses a min-heap for efficient priority selection.
- Reconstructs the shortest path.
- Rejects negative edge weights.

Time: O((V + E) log V)
Space: O(V + E)

## 2. Dynamic Programming - Resource Allocation

**Algorithm:** 0/1 Knapsack

- Maximizes profit under a fixed budget.
- Uses space-optimized 1D DP.
- Selects each project at most once.

Time: O(n * W)
Space: O(W)

## 3. Optimization - Top K Frequent Elements

**Algorithm:** Frequency Counter + Min-Heap

- Counts occurrences using a hash map.
- Maintains only the K most frequent elements.
- Uses deterministic ascending order for frequency ties.

Time: O(n + u log k + k log k)
Space: O(u + k)

## Engineering Decisions

| Problem | Decision | Reason |
|---|---|---|
| Graph | Dijkstra | Efficient non-negative shortest paths |
| DP | 1D Knapsack | Lower memory usage |
| Optimization | Min-Heap | Avoids sorting every unique element |

## Edge Cases

- Disconnected graphs
- Negative graph weights
- Zero budget
- Empty project list
- K = 0
- K greater than unique element count
- Repeated values and frequency ties

## How to Run

python graph_shortest_path.py

python resource_allocation.py

python top_k_frequent.py

## Learning Outcomes

- Graph traversal and shortest paths
- Dynamic programming optimization
- Heap-based optimization
- Complexity analysis
- Edge-case handling
- Engineering tradeoff documentation
- 
