# comp110-worksheet-C
Base repository for COMP110 worksheet C
* (a) The algorithm is testing whether there is 2 or more of the same elements in a list.
* (b) The algorithm worst case is quadratic because it checks each element of i against each element of j n times (from the same list of length n). For every i (n number of times) it goes looping through j n times. O(n * n). The n loop is nested inside another.
* (c) The algorithm still works because j is still comparing to the elements the i loop has gone through already.
* (d) The j for loop is only checking against the elements the i loop has been through already rather than comparing every position in the list in both the i and j loops.
* (e) It is now linear, the j loop is no longer looping n times. There is only one n loop. The computation time will increase proportionally to the list length.
* (f) https://wiki.python.org/moin/TimeComplexity Python's Sort method is O(n log n) in big-O notation.
* (g) The sort function is used in the algorithm and in python the sort function is O(n log n). O( n log n) is dominant over the linear O(n). There are no "Slower" complexity classes in the algorithm.
* (h) The second algorithm uses Sort which is O(n log n) which is the dominant complexity. The first is quadratic, O(n^2) which is slower than O(n log n). The sort function means the second algorithm doesnt need to loop as much as the first algorithm.
* (i) If the list is small or already sorted then the sorting function is an unnecessary step and may take longer.
