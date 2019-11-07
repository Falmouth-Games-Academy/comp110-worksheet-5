# comp110-worksheet-5
Base repository for COMP110 worksheet 5
## (a)
This algorithm will check every index in i and j against each other, if they are the same then it will return true therefore revealing that there is a duplicate in one of the lists.

## (b)
the worst case scenario for this algorithm is if there is no duplicates in the lists, this is because it would have to run through both lists completely. Alone these searches would be O(n), however, when there are no duplicates then it would end up being O(n²). It ends up being quadratic because the two linear algorithms would be multiplyed together, which can then be simplified to O(n²).

## (c)
It will still work however the method will just be slightly different. Because i and j are the same length anyway then it will still run for the same length of time, but if one list is a different size then it would be missing some from j.

## (d)
The progam will be running twice as fast because it's checking segments of the lists, this will increase the chances of a duplicate being found.

## (e)
Yes it would still be quadratic, this is because thej loop is still there just simplified now. This means that it will still be n * n hence the simplification to O(n²).

## (f)
The time complexity for pythons sort function is: O(n log n) [1](https://en.wikipedia.org/wiki/Timsort).

## (g)
O(n) It should be linear as the algorithm is sorting the list but then still checking them from start to end.

## (h)
The second algorithm should run faster as it's a linear whereas the first is quadratic.

## (i)
The programmer may not know how to set up the more complex faster algorithm.
