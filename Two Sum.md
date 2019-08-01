# Two Sum

- [1. Two Sum](https://leetcode.com/problems/two-sum/)




Solution: 
1. Implement a HashMap to store the number we have visited.
2. Scan the array, every time encounter a new number, check if we have seen its complement before,  <br>
if true, return res array, else, continue the scanning process until we visit every number.

TimeComplicity: O(n) <br>
SpaceComplicity: O(n)
