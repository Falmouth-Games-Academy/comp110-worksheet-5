# comp110-worksheet-5
Base repository for COMP110 worksheet 5

# A
This algorithm looks through a list of items and runs each item against every other items to recognise any duplicated items in the list. If there is a duplicate, it will return true.

# B
Because it will have to check n * n = n^2 and if it has to do that many checks, the entire process might be useless if it never finds any duplicates.

# C
This algorithm still works since every item still checks itself with every other item. Instead, this algorithm checks all the items before itself, against itself, checking if it's a duplicate. The algorithm then moves on to the next item, once again checking every item before it on the list, therefore eventually checking every item against each other.

# D
This new algorithm will run twice as fast as the first one because of the way it checks all items against the other items in the list. The first algorithm checks every item against every other item while the new algorithm halves the time it takes since it is only checking every item behind the item it has chosen.

# E
The algorithm is still quadratic because it is still running through two For Loops, which still makes it O(n^2).

# F
Using https://wiki.python.org/moin/TimeComplexity I have found that the time complexity is O(n log n).

# G
The complexity of tha algorithm would be O(n log n) because it uses the sort() function.

# H
I believe the second algorithm will run faster as it's time complexity is O(n log n) which is faster than the first algorithm which had a time complexity of O(n^2).

# I
Programmers might choose the slowest algorithm because it might be more effecient for sorting smaller lists.
