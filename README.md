# comp110-worksheet-5

###a)  
The algorithm takes a list and iterates through it comparing different items in the list checking for duplicates.  
If there are two items which are the same at different indices then there is a duplicate so the program returns 'true'.  
If there are no duplicates the program returns 'false'.  

###b)  
There are 2 nested for loops. The outer loop executes n times and the inner loop executes m times for each n.  
Therefore the time complexity is n * m or O(n^2).

###c)  
n is the length of the whole list so using i-1 instead stops the algorithm from doing the same checks several times.  

###d)  
It has about half the comparisons to make so takes about half the time.  

###e)  
The algorithm is faster but it is still quadratic because it take about half the time not square root the time which  
would make it linear.

###f)  
Python's sort function has a time complexity of O(n log n). As found from [python time complexities](https://wiki.python.org/moin/TimeComplexity)  

###g)  
O(n log n)is a greater time complexity than O(n) so the time complexity stays as O(n log n).  

###h)  
For larger inputs O(n log n) is faster than O(n^2) so the second algorithm will run faster than the first.  

###i)  
If the programmer knows that the lists that their program will be sorting are going to be small then they may choose  
the slower one because it is actually quicker for smaller inputs.