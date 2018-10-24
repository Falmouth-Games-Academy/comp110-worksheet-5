# comp110-worksheet-C
Base repository for COMP110 worksheet C

(a): The 'HasDuplicate(list)' function goes compares every member of a list to every member of the same list (including, rather inefficiently, comparing the same member against itself). 
If i and j are the same, it also asks if it is the same space in the list. If it isn't, the list contains a duplicate entry and we return true.

(b): The running time of the algorithm is quadratic ( O(n^2) ) because, since the algorithm is comparing each element of the list (including the same element), it is going through the the list exactly n^2 times.

(c) The algorithm isn't correct. If a for loop runs from 0 to -1, it will crash. If i = 0, then i-1 will be -1, resulting in a crash. If we assume I'm incorrect and the algorith won't crash, then this new pair of for-loops should avoid comparing each element to itself and comparing two elements more than once.

(d) The new algorithm will only compare two different elements once. 
When i = 0, it doesn't run the j loop.
When i = 1, it compares it to 0.
When i = 2, it compares it to 0 and 1.
When i = 3, it compares it to 0, 1 and 2. This repeats indefinitely and efficiently prevents duplicate comparisons and self-comparisons.

(e) The new algorithm complexity is not quadratic, because it is no longer doing n^2 operations. 

This appears to be the second-fastest method of searching for duplicates in an unsorted list, the fastest being O(n) using a 'tally chart'-like hashing system, like storing each entry in an array and stopping (returning true) when a new entry already exists.

(f) Now we have sorted our list, 
