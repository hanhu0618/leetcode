## DP
- [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)
<br/>
Too hard....
<br/>
Solution:

1. Use two deques for BFS, one to store nodes, the other to store levels.
2. BFS and put all of the nodes into a map.
3. Traverse the map from the min key to the max key and put all of the results into res.
<br/>


1. s.charAt(i) == p.charAt(j) || p.charAt(j) == '.' : dp[i][j] = dp[i - 1][j - 1].
2.p.charAt(j) == '*'.
3.if(p.charAt(j - 1) != s.charAt(i)) dp[i][j] = dp[i][j - 2].
4.if(p.charAt(j - 1) == s.charAt(i)) || p.charAt(j) == '.'.
5.dp[i][j] = dp[i - 1][j].
6.or dp[i][j] = dp[i][j - 1].
7.or dp[i][j] = dp[i][j - 2].

tc O(n^2)
