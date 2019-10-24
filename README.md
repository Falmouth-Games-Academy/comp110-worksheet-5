# comp110-worksheet-5
Base repository for COMP110 worksheet 5
(a)
The algorithm takes an item from a list, compares it to all the other items and checks to see if they match, does this for all the items.
If there's a item that matches another item, then returns true. If no items match, then exits the loop and returns false.

(b)
The worst case scenario is quadratic, because it would go through n items, n times therefore O(n<sup>2</sup>).

(c)
The algorithm is still correct, because both for loops are looping through the same list size.

(d)
The algorithm will be faster because j is only looking through the loops of i.

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
