## DP
- [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)
<br/>
Too hard....
<br/>
Solution:


1. S s.charAt(i) == p.charAt(j) || p.charAt(j) == '.' : dp[i][j] = dp[i - 1][j - 1]
2. S p.charAt(j) == '*'
3. S   if(p.charAt(j - 1) != s.charAt(i)) dp[i][j] = dp[i][j - 2]
4. S   if(p.charAt(j - 1) == s.charAt(i)) || p.charAt(j) == '.'
5. S     dp[i][j] = dp[i - 1][j]
6. S     or dp[i][j] = dp[i][j - 1]
7. S     or dp[i][j] = dp[i][j - 2]

tc O(n^2)
