# comp110-worksheet-5
## A
The algorithm checks a list for duplicates, returning true if there is a duplicate, otherwise returning false.

## B
In the worst case scenario there will be no duplicates, meaning every entry in the list will have to be checked. As the algorithm uses two nested for loops each with n iterations the total number of times the loops will run will be n * n = n^2

## C
The algorithm is still correct as every entry is checked against all previous entries, with the final entry being checked against all other entries in the list. This eliminates entries being checked twice, for example in the previos algorithm when i = 1, entry 1 would be checked against entries 0, 2, ... , n-1. At i = 2 entry two would then be checked against entry 1 again, even though this is redundent.

## D
With the new algorithm on average only half of the list is being tested against, whereas in the previous loop the entire list was being tested against each iteration.

## E
The equation for calculating the new complexity would be i_max * j_max, where i_max = n and j_max = i_max - 1 = n - 1. Therefore the time complexity is n * (n -1) = n^2 - n. As when calculating time complexity we take only the value with the largest power, the time complexity is still n^2.

## F
The time complexity of the python sort functin is O(n log(n)). (Sourced from the official python wiki - https://wiki.python.org/moin/TimeComplexity)

## G
The time complexity of the algorithm would be n log(n) + n. However, because n log(n) is slower than n we can ignore the n when writig in big-O notation, meaning the time complexity is still O(n log(n)).

## H
The second one is likely to run the fastest as linearithmic time complexity O(n log(n)) is faster than quadratic time complexity O(n^2) for large lists.

## I
For n < 100 quadratic time complexity is actually faster than linearithmic time complexity
