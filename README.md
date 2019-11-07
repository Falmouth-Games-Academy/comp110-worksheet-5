# comp110-worksheet-5
Base repository for COMP110 worksheet 5

### A)

The procedure checks for elements equal to each other, where the indexes are not equal (progressive 2 dimensional iteration).

### B)

Checking `list` at indexes `i` & `j` where not equal, requires dual integer decrementation. On each cycle, checking for a return condition or if a loop condition has been met. `n^2` is the count of values to check.

### C)

`j` now only checks from where `i` is currently at, therefore requiring less checks each cycle.

### D)

Checking each index from where `i` left off, reducing the time to complete the task (progressive decremation sequence over list of values).

### E)

Yes, it is still possible to search the entire list (yet it does not reveal what value(s) it has found, so there can be more than one duplicate).

### F)

![Google Math Render of O(N Log N)](https://chart.googleapis.com/chart?cht=tx&chl=O(n%20Log%20n))

- [Python/moin TimeComplexity](https://wiki.python.org/moin/TimeComplexity)
- [Python SVN trunk file](http://svn.python.org/projects/python/trunk/Objects/listsort.txt)

<!-- > **NOTE: `sort` is not is not a function in native python version x, use `<list>.sort()` or `sorted(<list>)`.** -->

### G)

![Google Math Render of O(N^2 Log N)](https://chart.googleapis.com/chart?cht=tx&chl=O(n^2%20Log%20n))

The list is always sorted before compared `O(n Log n)`, then the list is iterated through `O(n)`.

*Other notations are also possible.*

### H)

The algorithm with the notation of `O(n Log n)`, since n^2 is expoential in the terms of quadratics.

### I)

As the list size increases, the number of operations can do so either linearly or exponentially. Therefore, the slower algorithm is a better choice should the list size have a chance of being larger than expected.
