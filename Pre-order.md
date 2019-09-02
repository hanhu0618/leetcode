## Pre-order

- [297. Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/)

Solution:<br>
1. Use pre-order traverse to serilize and deserilize

- TimeComplicity: O(n)
- SpaceComplicity: O(n)


- [449. Serialize and Deserialize BST](https://leetcode.com/problems/serialize-and-deserialize-bst/)

Solution:<br>
similar to 297, except for that we can take advange of bst's feature that all nodes left than root has value equal to or smaller than root.
1. Use pre-order traverse to serilize and deserilize

- TimeComplicity: O(n)
- SpaceComplicity: O(n)

## Bottom-up DFS

- [124. Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/)

solution:

1. Bottom-up DFS.
2. We memorize the max sum and compare it with current sum when returning to a subtree root.
3. We we need to return, we choose the max subpath(left or right).
