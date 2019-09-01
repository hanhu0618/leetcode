## Backtracking
- [282. Expression Add Operators](https://leetcode.com/problems/expression-add-operators/)
Solution:

1. backtracking, use String rather than List to store path for convenience.
2. The tricky part is to store the cur value in order to do multiply.
3. Besides, we need to eliminate numbers start with 0.
