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
