# comp110-worksheet-5
Base repository for COMP110 worksheet 5



a.)	This procedure takes a list and compares each element within It with all the elements trying to identify duplicates. It does this by taking two temporary variables, firstly it ensures that the two variables are not looking at the exact same piece of data then it checks to see if the values of the two variables are the same. If it finds values that match it returns true to identify that that list has duplicate values.     

b.)	The worst case of running this procedure would be when no duplicate was found in the list, this would mean that every item had been compared against all the other items. The process of comparing all elements within a list is a quadratic complexity. There is nothing in this procedure that exceeds the complexity of this, making the overall complexity of this procedure quadratic.

c.)	Changing line 4 as stated would remove the duplicate tests that occur naturally within the nested for loops. It does this by restricting the second variable to only compare it to earlier items than the first variable. This stops the duplicate testing as for a list such as (0,1,2,3,4) when i was 0 it would be tested against 4, then later when i was 4 it would be tested against 0. By limiting the second variable to being earlier or later then the first it removes this redundant testing.

d.)	As the redundant duplicate tests aren’t run the program will half the amount of work for the computer to do. The average time the computer will take to run the second program will average to roughly half, as it has half the work to do.

e.)	Yes, as the algorithm implemented is still a quadratic one. By halving the amount of work you have altered a multiplier on the equation, however the algorithm itself remains unchanged.  

f.)	  O(n log n)   ( https://wiki.python.org/moin/TimeComplexity ).

g.)	The sorting function will have a logarithmic algorithm (O(n log n)), the comparative will have a constant (O(1)) and the matching mechanism will have a liner (O(n)). The dominant term here is the linear one (O(n)) as it is the worst when n is large making it the most complex equation.

h.)	The most complex equations for these solutions are quadratic for the first and linear for the second. Therefore, when n is large the second program will complete the process faster as quadratic is dominant over linear making the linear solution more efficient.

i.)	A programmer may choose to use the “slower” algorithm is their list is small, this is because the “slower” algorithm will be faster when the list is small. Although quadratic equations are considered slower than linear equations when (n = length of list) is large. When n is small there will be a brief overlap where the quadratic solution is faster. However this is unlikely to make a noticeable difference.       
