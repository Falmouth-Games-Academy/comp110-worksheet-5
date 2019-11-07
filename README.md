# comp110-worksheet-5
Base repository for COMP110 worksheet 5

## (a)

The algorithm looks for numbers that are the same throughout the list. If a duplicate is found in the list, the procedure returns true. If the list
is only made out of different numbers, it returns false.

## (b)

There are 2 nested 'for' loops in the algorithm: the first one iterates 'n' times the second one which also iterates 'n' times for each iteration of the first one. So it is n*n.

## (c)

It is correct because the second loop checks all the numbers before the current iteration of 'i', the iterator of the first loop, so instead of checking all the other numbers on each iteration of the first loop(the first version
of the algorithm), it only checks  the ones before the current 'list[i]' element, so it still check for duplicates correctly.


## (d)

The second version is much more efficient because it halves the number of comparisons, comparing all of the numbers before the current 'list[i]' element, instead of comparing the 'list[i]' element with all the other
elements every iteration.

## (e)

In order to find the answer, I will draw a table of iterations for each loop:

|Value of 'i'| |Number of iterations of the second loop|
|---|---|
|0||0|
|1||1|
|2||2|
|...||...|
|n-2||n-2|
|n-1||n-1|

So the total number of iterations of the inner loop is equal to 'i' so the time complexity is still quadratic.

## (f)

Python's built-in sort method is using Timsort as a sorting algorithm, taking advantage of runs 
of consecutive ordered elements. In the worst case, Timsort/Python's built-in sort takes O(n log n) comparisons
to sort an array of n elements. The best case performance being O(n) and the average case performance being O(n log n).

## (g)

