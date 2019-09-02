# String

- [953. Verifying an Alien Dictionary](https://leetcode.com/problems/verifying-an-alien-dictionary/)




Solution: 
1. Use HashMap to store the alien language alphabet order.
2. Implement compare method to compare two different String.
3. Use compare to verify the order of words. 

Optimization: Use array instead of HashMap to store the new order.

# Union Find

- [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/)
We used union-find to group all emails.

Solution:
1. Initialization the union-find structure
2. Union all emails
3. Put emails with the same parent to the same treeset
4. get result

tc O()

# Bucket Sort

- [791. Custom Sort String](https://leetcode.com/problems/custom-sort-string/)

solution:
1. Using bucket sort to sort.
2. We divide 26 letters in serveral buckets, there's order between each bucket according to S
3. Put all letters in T into these bucket and we need to record how many times a letter occur in a bucket. Letters don't occur in S will be put to the same bucket and this bucket will be put at the tail.
4. Construct a string according to these buckets

tc O(n + m) We scan S, T once for each and to output the string, we counter O(m) time cost, so the final tc is O(n + m)


# Hard to Find Corner Case

- [794. Valid Tic-Tac-Toe State](https://leetcode.com/problems/valid-tic-tac-toe-state/)

solution:
1. Use cols, rows, diag and antidiag to store Xs and Os
2. Check the corner cases, such as turns can only be 0 or 1, the other player cannot make a move after one player wins

tc O(1)

# Sliding Window

- [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)

solution:
1. Use two pointer to mark the start and end.
2. Use an array or HashMap to store state, which will tell if we meet the requirement
3. Find a valid substring
4. Move the start pointer, to find the minimum window

tc O(n)

# Sliding Window

- [340. Longest Substring with At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/)

solutions:
1. Nearly the same as 76.
