## Binary Tree
- [314. Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal/)
Solution:

1. Use two deques for BFS, one to store nodes, the other to store levels.
2. BFS and put all of the nodes into a map.
3. Traverse the map from the min key to the max key and put all of the results into res.

Be careful, we can't use DFS here, because we may not get the result with vertical order.

## Topological Sort
- [269. Alien Dictionary](https://leetcode.com/problems/alien-dictionary/)

Solution:

1. Use HashMap to store topological order
2. Use BFS to do topogical sort

## Find Shortest Distance
- [317. Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings/)

Solution:

1. Record distance from one buildings to other empty spots and buildings
2. Compute distance from one spot to all buildings.
3. Find the minimum distance sum.
