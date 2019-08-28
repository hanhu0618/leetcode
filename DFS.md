Parenthese
[301. Remove Invalid Parentheses]
Solution:

1. Use count to record unpaired open-parentheses. Once count becomes negative, we need to remove one close-parenthese.
2. When enountering consecutive close-parentheses, we remove the first one as to avoid duplicates.
3. Do this recursively.
4. Once no violence appear, we reverse the String and check if any open-parenthese redundancy happens.
5. After the reversing check, we add the result to solution.
