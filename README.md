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

(f) I'm unsure whether referencing Wikipedia is a cardinal sin or not, but (with reference to the Wikipedia page on Timsort (which is the sorting algorithm used in Python's built in sorting functions)[https://en.wikipedia.org/wiki/Timsort#Analysis], it has a worst case complexity of O(n log n), with a best case (when the input is already sorted) of O(n).

(g) If we include Python's sort into this equation, it would remain O(n log n) as the difference made by line 4's 'for loop' is small enough to be ignored when writing our big O formula. 
Otherwise, if we exclude the sort from this equation, the complexity of line 4 would be at most O(n), linear.

(h) The second function will run faster with larger lists because the first function suffers with scalability - with large lists its runtime grows massively, whereas the second function has a very stable runtime as the size of n grows.

(i) The reason "slower" and "faster" are written in quotations is because one is not **always** faster than the other. It is a question of scalability, and scalability vs simplicity is the reason a programmer might choose one over the other - because the "slower" one may be faster/the same and much simpler to implement when we needn't take scalability into account.
