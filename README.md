# comp110-worksheet-5
Base repository for COMP110 worksheet 5

(a). The algorithm is just iterating through the two lists looking for duplicate elements between the lists.  

(b). Explain why the worst case running time of the algorithm is quadratic, i.e. O(n^2).

(n - 1) x (n - 1) = (n - 1)^2

n^2 - n - n + 1 

n^2 - 2n + 1 

n^2

(c). The algorithm is still checking each of the items in the list but it is just improved because it doesn't check all of the upcoming elements.  

(d). The algorithm runs approximately twice as fast because the average amounts of times that it runs is half the length of the list.

(e). The algorithm is still quadratic because: 

(n - 1) x (i - 1) = ni - n - i + 1 

n^2 -2n + 1 

n^2 

(f). Python's sort functions time complexity is O(n log n).

https://wiki.python.org/moin/TimeComplexity

(g). n log(n) + n



(h). If the size of the list is large, than the quicker algorithm will be O(n log n), as the O(n^2) grows in number of operations much more quickly because its multiplying the lists length by the list length every time it is run. Whereas O(n log n) has a less aggressive increase than the quadratics.

(i). A programmer may choose to use the "slower" algorithm if they have a smaller list, as the O(n^2) is actually faster than O(n log n) with elements n < 100. 
