## DP
- [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)
<br/>
Too hard....
<br/>
Solution:
   1. s.charAt(i) == p.charAt(j) || p.charAt(j) == '.' : dp[i][j] = dp[i - 1][j - 1]
   2. p.charAt(j) == '*'
   3.  if(p.charAt(j - 1) != s.charAt(i)) dp[i][j] = dp[i][j - 2]
   4.  if(p.charAt(j - 1) == s.charAt(i)) || p.charAt(j) == '.'
   5.      dp[i][j] = dp[i - 1][j]
   6.   or dp[i][j] = dp[i][j - 1]
   7.   or dp[i][j] = dp[i][j - 2]

tc O(n^2)
