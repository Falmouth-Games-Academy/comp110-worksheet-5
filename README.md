# comp110-worksheet-C
# Answers

(a) Checks each item in the list agaisnt all other items in the list, if the list position is not the same but them item itself is the same, returns true. (checks if an item is duplicated but in different position)

(b) Because both for loops are linear O(n) we multiple the compond algorithms making O(n^2)

(c) Each iteration of i has already been checked against all positions. i.e 1st position is checked against all, now the 2nd position doesn't need to be checked agaisnt 1st position

(d) Each loop of i we have to check one less, at the middle of the loop we are checking vs about half the list, and at the end only checking vs itself makings the j loops quicker and quicker

(e) Because we are doing two things n times still the two linear algorithms still compound to make a quadratic one

(f) Python sort function time complexity worst case - O(n log n) 
[Reference: Python Wiki TimeComplexity](https://wiki.python.org/moin/TimeComplexity)

(g) Time complexity is O(n log n) because we only take the dominant term

(h) The second algorithm using the sort function should run faster. As the amount of elements grow O(n log n) needs a lot less operations compared to O(n^2) [Reference: bigO cheatsheet](http://bigocheatsheet.com/)

(i) Might user the slower function as the sorted list needs to be stored in memory using more memory space than the slower function.

![alt text](https://i.pinimg.com/736x/15/5f/ae/155faed25808c60277b6748aed0e7b25--fan-art-cartoons.jpg "Big O how I see it")
