# Worksheet C
**(a)** Checks if a list has at least two identical items in it  
**(b)** For every item in the list, every item in the list is iterated and checked. If 'every item' consists of n items, this means n * n iterations, or O(n²)  
**(c)** This is valid because when two indices are compared, one is always smaller than the other. For example, list[3] == list[2] -- or list[2] == list[3]. These two statements are equivalent, so it's legal to omit the latter case by clamping the inner index *j* to values smaller than the outer *i*, i.e. for j < i.  
**(d)** Skipping the case where the other value is larger means we essentially eliminate every one of the equivalent statements. As each check has one equivalent reversed check, this means half of our total checks are eliminated, resulting in a roughly equivalent cut in computing time.  
**(e)** Yes. While half of the total checks are eliminated, a halving of the number of checks is just a linear division of an ultimately quadratic number. In simple terms, 0.5n² still has the quadratic square of n, just halved.  
**(f)** According to the Python reference, Python uses the Timsort algorithm. In big O notation: O(n Log n), according to geeksforgeeks.org.  
https://docs.python.org/3/howto/sorting.html  
http://www.geeksforgeeks.org/timsort/  
**(g)** O(n Log n). While the for loop within the function has a complexity of O(n), the most significant factor is the sort function. Big O always illustrates the most significant factor of N.  
**(h)** The second one, as the time penalty with respect to the data size is at worst n multiplied by log N. With large sets of data this is a lower time penalty than the former's quadratic n², as the increment of log N decreases over time while n increments constantly, hence in scenarios where n is high, n² > n Log N.  
**(i)** The programmer may be working with smaller sets of data, wherein the cost of sorting the list might be higher due to a) extra overhead b) more memory/cache R/W which can be slow and c) he had no idea he could do it and they won't replace his precious code unless you donate £5 in coffee and £3 in Dr Pepper. These costs are expensive as there are other time-intensive processes to run and other generally-intensive programmers to feed.  
