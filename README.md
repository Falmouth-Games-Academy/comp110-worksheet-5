# comp110-worksheet-5

## Answers

### A
This algorithm checks through a list for any duplicates. If there are any duplicates found within the list, it will return True. If not, then it returns False.

### B
The worse possible case for the algorithm is there not being a single duplicate within the list. This means that every item within the list will have to be checked. Now with the algorithm using nested `For` loops, the list will have to be checked the amount of iterations of `n`. Meaning that the amount of times the loop will run would be n * n = n^2.

### C
This new algorithm is still correct as it checks the list against all other previous items within the list. And with this new algorithm, the very last item in the list would be checked against every other item within the list. This new algorithm still compares every item in the list, making it fit for its purpose.

### D
This new algorithm runs roughly twice as fast, due to loop only using half the amount of iterations the original algorithm was completing.

### E
The algorithm was originally n^2 but it now has changed to n(n - 1) / 2. This can be adjusted to (n^2 - n) / 2, which can still be changed to O(n^2). Meaning that the algorithm is still quadratic.

### F
The time complexity for Python's sort function is:
```python
O(n log(n))
```
Source: [Python Wiki: Time Complexity](https://wiki.python.org/moin/TimeComplexity)

### G

### H

### I
