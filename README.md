# comp110-worksheet-C
Base repository for COMP110 worksheet C

a) The algorithm checks if there are duplicate values in a list, returning true if there are.  

b) If there are no duplicates, the algorithm will have to iterate the entire length of the list for each item in the list, resulting in the number of passes being (length of list ^ 2).   

c) The function now checks for duplicates before the current item in the list, rather than checking the whole list. However, when the last item in the list is reached, every item before it will be checked, therefore any duplicates will still be found.  

d) As only the items before the current item are checked, there are approximatly half the number of comparisons to make.  

e) No, as the second loop no longer has to iterate through all values. I believe it would be O(n log n).  


f) https://wiki.python.org/moin/TimeComplexity Python sort function time complexity is O (n log n)  

g) Time complexity = O(n log n) as the algorithm still has to sort the list first.  

h) The second function will run faster as it has a time complexity of O(n log n) compared to O(N^2)  

i) If the list is small the greater time complexity of the slower algorithm may not be an issue.  

