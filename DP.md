## DP
- [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)
<br/>
Too hard....
Solution:
   s.charAt(i) == p.charAt(j) || p.charAt(j) == '.' : dp[i][j] = dp[i - 1][j - 1]
   p.charAt(j) == '*'
    if(p.charAt(j - 1) != s.charAt(i)) dp[i][j] = dp[i][j - 2]
    if(p.charAt(j - 1) == s.charAt(i)) || p.charAt(j) == '.'
        dp[i][j] = dp[i - 1][j]
     or dp[i][j] = dp[i][j - 1]
     or dp[i][j] = dp[i][j - 2]

tc O(n^2)
