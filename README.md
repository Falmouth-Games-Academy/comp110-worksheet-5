# comp110-worksheet-5
Base repository for COMP110 worksheet 5

### A
This alogorithm checks through a list to see if there is a duplicate item in the list, it checks each item against the others, excluding itself.

### B
The worse case for this algorith is quadratic because if there is no duplicates in the list, it will have to run for each item in the list. In line 4 the for loop will iterate for each item in the list meaning that the algorithm will have to run O(n) * O(n) or O(n²).

### C
The algorithm is correct as it is still checking each element in the list against eachother, with the final item being checked against all other items in the list.

### D
It will run faster as on average, only half of the amount of iterations will be needed to complete the algorithm.

### E
It is still quadratic as it is still going thorough two loops, meaning that it is still being compared twice resulting in the same O(n) * O(n) or O(n²). 

### F
https://wiki.python.org/moin/TimeComplexity The Python Wiki shows that, O(n log n) is the time complexity of the built-in sort function

### G
The time complexity would be n log(n) + n; however, because n log(n) is slower than n, we can ignore the n when writing in big-O notation, meaning the time complexity is still O(n log n).

### H
The second algorith will run faster as O(n log n) will run the algorithm in less opererations than the O(n²) of the first algorithm. This is because the first algorithm's operations wll increse with the elements of the list.

### I
One reason could be that Quadratic time complexity is often faster than linearithmic time complexity when dealing with shorter lists.
