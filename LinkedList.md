## LinkedList

- [2. Add Two Numbers]

Solution:<br>
1. Use fakedHead to ensure we can always have a reference to get the result head.
2. Add two numbers from the least digit. At the end of one pass, we want l1 and l2 to point to their next nodes.
3. Check if we need to add more nodes.

- TimeComplicity: O(m + n)
- SpaceComplicity: O(m + n)
