# comp110-worksheet-5
Base repository for COMP110 worksheet 5


A) Checks if any list elements are duplicated
B) The outer loop counts from 0 to n, and for every loop, the inner loop also counts from 0 to n, making the total time n * n or n^2
C) In the first algorithm, every pair of elements is checked twice, but the second algorithm cuts out one of the checks for each pair of numbers
D) Since half of the checks have been eliminated, the algorithm only needs to perform half the amount of comparisons, roughly halving the execution time
E) The worst case has changed from n^2 to n(n-1)/2, which expands to (n^2 - n)/2, which is still O(n^2), so the time is still quadratic
F) Python list sorts are in O(n log(n)) (https://wiki.python.org/moin/TimeComplexity)
G) n log n + n = O(n log n), since n log n > n
H) Algorithm 2 will run faster, since n log n is faster than n^2 if the list is large enough
I) The language may not have an n log n sorting function for lists/arrays
