# comp110-worksheet-C
Base repository for COMP110 worksheet C

a) This algorithm checks if any item in the list has a duplicate by scanning the list through each item, and then for each value scanning the list again and checking if any item that is not of the same index contains the same value.

b) Because of the way that the algorithm scans through the list (which is: scan the list once and for each item in the list scan the whole list again), if the two last items were the same, the algorithm would have to go through the length of the list (n) squared (n^2). Therefore the worst case running time of the algorithm would be quadratic (O(n^2)).

c) if the 'for' loop on line 4 was changed so that 'j' ranges from 0 to i-1, the algorithm would still be correct, because it would check all of the previous items from the current item. So if the duplicate was in front of the item in the list, the algorithm would still find it when it got to the duplicate and started scanning backwards.

d) The algorithm now will run almost twice as fast, because it doesn't have to scan through each item in the list every new item. Instead the number of items will increase with the index of the current item (e.g. if the current item's index is 2, the algorithm will only scan 2 previous items(0, 1) and if the index is the last item of the list(n) then the algorithm will scan through every item in the list except the last). So if we're on the middle item in the list, the algorithm will only scan half of the list leading up to that item instead of scanning every item in the list.

e) The time complexity for the changed algorithm is not quadratic (O(n^2) anymore, because if we add a new item to the list it will not increase the running time by n^2, as we're not scanning each item of the list every iteration. Instead the running time will now be proportional to n, which means the new algorithm's time complexity is linear (O(n)).

f) According to the top answer on https://stackoverflow.com/questions/14434490/what-is-the-complexity-of-this-python-sort-metho and https://wiki.python.org/moin/TimeComplexity the time complexity of the 'sort' function in python in the worst and average case is O(n log n). The answer from the first source refers to a wikipedia article about the sort function in python https://en.wikipedia.org/wiki/Timsort which states that in the worst case the time complexity of the function is O(n log n) and in the best (when the input is already sorted) it's O(n).

g) The time complexity of this algorithm would be O(n log n + n) because we can assume that the time complexity of the sort function used is O(n log n) and the time complexity of the for loop is o(n). Therefore when we add the two together we get O(n log n + n).

h) The second algorithm will be more likely to run faster than the first because O(n log n) < O(n^2).

i) A programmer might choose the "slower" algorithm if the size of the input list is so small that it would actually take more time for the "faster" algorithm to run.
