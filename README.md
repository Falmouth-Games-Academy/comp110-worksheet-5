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
