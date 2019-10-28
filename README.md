# comp110-worksheet-5
James A's Worksheet 5 Solutions,

## a

This algorithm will check if the set is equal to another

## b

It has to check for every element, the other list. Using the identity, given that checking it once would be O(n), then this algorithm would be O(n\cdot n) = O(n^2)

## c

Let the two sets be A and B. Due to the fact that if the cardinality of A is greater than B, for A to equal B, then only the cardinality of A numbers need to be run through, which is i.

## d

Only half of the numbers are being run through. For the first run, consider the two sequences of numbers left out in the second version.

B = i - 1, i - 2, i - 3, i - 4, ... , 4, 3, 2, 1

B_l = 1, 2, 3, 4, ... , i - 4, i - 3, i - 2, i - 1 

It should be obvious that these are equal.

## e

It should be quadratic, its just that the list grows slightly slower than before.

### f

O(n\cdot log n) [SOURCE](https://www.ics.uci.edu/~pattis/ICS-33/lectures/complexitypython.txt)

### g

Compound complexities: O (n \cdot nlogn) = O(n^2 \cdot logn)

### h

For sufficiently large n, we should take n^2logn, i.e. n > 10. So choose O(n^2\cdot logn)

### i

Because they have a small set


























