## Binary Tree
- [314. Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal/)
Solution:

1. Use two deques for BFS, one to store nodes, the other to store levels.
2. BFS and put all of the nodes into a map.
3. Traverse the map from the min key to the max key and put all of the results into res.

Be careful, we can't use DFS here, because we may not get the result with vertical order.
