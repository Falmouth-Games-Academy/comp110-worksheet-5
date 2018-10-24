a) Checks if a list contains a duplicate.

b) Because if the list contains no duplicates, it will have to run through the second again for every additional element.

c) Because the second duplicate item's iteration will  always catch the fact that it matched the first.

d) Because on average, it will only go through just under two-thirds of the iterations (1+2+3...+n instead of n^2).

e) Yes. It's closer to triangular time, but as big O notation is always an upper bound it would still be O(n^2)
