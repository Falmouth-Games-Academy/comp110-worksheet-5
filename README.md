# comp110-worksheet-5
Base repository for COMP110 worksheet 5
by *Adrian Tofan*.

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
|---|---|---|
|0| |0|
|1| |1|
|2| |2|
|...| |...|
|n-2| |n-2|
|n-1| |n-1|

So the total number of iterations of the inner loop is equal to 'i' so the time complexity is still quadratic.

## (f)

Python's built-in sort method is using Timsort as a sorting algorithm, taking advantage of runs 
of consecutive ordered elements. In the worst case, Timsort/Python's built-in sort takes O(n log n) comparisons
to sort an array of n elements. The best case performance being O(n) and the average case performance being O(n log n).

[Reference link 1](https://en.wikipedia.org/wiki/Timsort)
[Reference link 2](https://stackoverflow.com/questions/25813774/complexity-of-python-sort-method)

## (g)

It is O(n log n), as n log n(the complexity of the built-in sort method) + n = n log n time complexity; n log n > n.

## (h)

The second algorithm would be faster than the first one, as the Timsort algorithm is supposed to work with larger inputs. The first one would work better for shorter lists.
The second algorithm's worst case time complexity is O(n log n), while the first algorithm's worst case is O(n*n). 

## (i)

The programmer's choice would depend on the size of the data they are working with. Taking exercise h) as an example, the first algorithm would be considered slower than the second one when working with
larger inputs, but it would be more efficient on shorter lists.
