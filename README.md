# comp110-worksheet-5
Base repository for COMP110 worksheet 5
(a)  
The algorithm takes an item from a list, compares it to all the other items and checks to see if they match, does this for all the items.
If there's a item that matches another item, then returns true. If no items match, then exits the loop and returns false.

(b)  
The worst case scenario is quadratic, because it would go through n items, n times therefore O(n<sup>2</sup>).

(c)  
The algorithm is still correct, because both for loops are looping through the same list.

(d)   
The algorithm will be faster because j is only looking through the loops of i, this eliminates redundant comparisions throughout the list by only comparing each element ot the ones which follow it.

(e)  
 The time complexity of the algorithm isn't quadratic, because it would be O(n) and not O(n<sup>2</sup>).

(f)  
Python uses Timsort, which was named after Tim Peters, the Python developer who invented it. The Wikipedia page has complexity information:  

Worst case performance  O(nlogn)  
Best case performance   O(n)  
Average case performance    O(nlogn)  
Worst case space complexity O(n)  

Python Software Foundation. Python Language Reference, version 2.7. Available at https://hg.python.org/cpython/file/default/Objects/listobject.c

(g)  
Worst case performance  O(nlogn)  
Best case performance   O(n)  
Average case performance    O(nlogn)  
Worst case space complexity O(n)  

(h)
The algorithm which sorts teh list will be faster if the list is larger, because it's only going to look through a part of the list, if it doesn't find a match it's going to look at another list of the same size, halfing it in the process and looking for a match there and repeat until it returns true or false. This is faster, because if the size of list is doubled, it only needs to half it an extra time, while the other algorithm looks at the whole size of the list for every item in the list. 

(i)
The programmer would always choose "faster" algorithm over the "slower" one in practice. If the list size is extremely small (3 items), then the "slower" algorithm would perform faster than the "faster" algorithm, this might be a reason to go with the less optimal approach for larger size lists. It is also harder to implement the "faster" algorithm, so the "slower" one might be used as a place holder.
