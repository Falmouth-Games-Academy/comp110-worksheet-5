# Worksheet C
**(a)** Checks if a list has at least two identical items in it  
**(b)** For every item in the list, every item in the list is iterated and checked. If 'every item' consists of n items, this means n * n iterations, or O(n²)  
**(c)** This is valid because when two indices are compared, one will always be smaller than the other. For example, list[3] == list[2] -- or list[3] == list[2]. These two statements are equivalent, so it's legal to clamp one of the indices to be smaller than the other as that will always be the case anyway...  
**(d)** ...Skipping the case where the other value is larger means we are essentially eliminate every one of the unneeded equivalent statements. As each check has one equivalent reversed check, this means half of our total checks are eliminated, resulting in a roughly equivalent cut in computing time.  
**(e)** Yes. In simple terms 0.5n² still has an n². It still stands that if you have to iterate through a particular proportion of the list for each item in the list it's quadratic. **I can't math it out right now, todo.**  
**(f)** According to the Python reference, Python uses the Timsort algorithm. In big O notation: O(n Log n), according to geeksforgeeks.org.  
https://docs.python.org/3/howto/sorting.html  
http://www.geeksforgeeks.org/timsort/  
**(g)** O(n Log n). While the for loop within the function has a complexity of O(n), the most significant factor is the sort function. Big O always illustrates the most significant factor of N.  
**(h)** **???**
**(i)** **???**
