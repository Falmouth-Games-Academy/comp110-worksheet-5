# comp110-worksheet-5
Base repository for COMP110 worksheet 5

(a)	The algorithm takes every element in a list one by one and compares it to every other element in the list to find any duplicates. The algorithm finishes as soon as it finds a duplicate item or if it doesn’t find a single duplicate.

(b)	If the list has no duplicates, the algorithm will have to check every element against every other element. Checking just one element against all of the rest is a simple linear search with a time complexity of O(n) but since we are checking n number of elements, the total running time of the program would be n * O(n) which has a time complexity of O(n<sup>2</sup>).

(c)	This version of the algorithm skips comparisons between the ith and any element after it. Any skipped comparisons during the first few iterations are addressed in the later iterations of the for loop. For example: if i = 3, the 4<sup>th</sup> ((i + 1)<sup>th</sup>) element gets compared to the 1<sup>st</sup>, 2<sup>nd</sup> and 3<sup>rd</sup> element and then the next iteration begins, skipping the comparisons between the 4<sup>th</sup> and 5<sup>th</sup> to n<sup>th</sup> elements but during the next iteration (i = 4) the 5<sup>th</sup> element does get compared to the 4<sup>th</sup> and so on to the n<sup>th</sup> (i = n), therefore filling in any skips created in early iterations of the loop.

(d)	With the original algorithm some comparisons are redundant (the 1<sup>st</sup> element gets compared to the 2<sup>nd</sup> and later the 2<sup>nd</sup> element is compared to the 1<sup>st</sup>). The updated algorithm removes all of the redundant cases. In the original, the amount of comparisons was n<sup>2</sup> while in the updated version the amount of comparisons is the sum of all numbers from 1 to n which averages out to be roughly half of n<sup>2</sup>.

(e)	Even though the new total running time of the program is roughly 0.5 * n<sup>2</sup> it is still noted as O(n<sup>2</sup>) time complexity.

(f)	Python’s sort function uses an algorithm called “Timsort” (mentioned here: https://python-textbok.readthedocs.io/en/1.0/Sorting_and_Searching_Algorithms.html) which has a time complexity of O(n log n) (mentioned here as sort(): https://wiki.python.org/moin/TimeComplexity and here as “Timsort”: https://en.wikipedia.org/wiki/Timsort#Analysis)

(g)	Since the for loop only checks every element against it’s neighbour element once, it’s time complexity is O(n), so the running time of the whole program would be n + n log n the dominant term of which is O(n) so the whole algorithm has a time complexity of O(n).

(h)	When graphed O(n<sup>2</sup>) grows much faster than O(n log n) as n increases so with a large list, the second algorithm is more likely to be faster.

(i)	If the sequence of elements in the list is important to the program, sorting is no longer an option and the programmer might use the slower algorithm instead.
