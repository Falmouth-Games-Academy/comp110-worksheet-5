# comp110-worksheet-5

(a)

The algorithm is used to check whether any items within a list have the same value, and it returns True if this is the case.

This is achieved by a loop that assigns a value to the variable "i" once every loop. The value of "i" starts at 0, then increases by 1 each loop until it is equal to the number of items in the list minus one.

Each time a value is assigned to "i" the algorithm will begin a nested loop that assigns a value to "j", starting with a value of 0 that increases by 1 each loop until it becomes equal to the number of items in the list minus one. Every time this nested loop assigns a value to "j" it will check whether the value of "i" is currently not equal to the value of "j", and whether the item at the list's index position equal to the current value of "i" has the same value as the item at the list's index position equal to the current value of "j".

If both of these are found to be true then the algorithm returns True.

Once the nested loop has gone through every possible value of "j" it finishes, causing the main loop to assign a new value to "i", which begins the nested loop once again. This continues until the value of "i" is equal to the number of items in the loop minus 1.

If no matching items are found throughout the entirety of the main loop the algorithm returns False.

This is an effective way to check for duplicate items in a list as the algorithm uses the loops to compare the value of every item in the list to the value of every other item in the list.

The values of "i" and "j" have to range between 0 and the length of the list minus 1 as the first item in the list is stored at the index position 0. This means that if "i" or "j" increased to a value exactly equal to the number of items in the list the algorithm would try to check an item at an index position that does not exist on the final loop, causing an error.

(b)

The worst case running time of the algorithm is quadratic as the main loop checks every item in the list each loop, and each time it does so the nested loop itself checks every item in the list. This means that the algorithm must perform a number of checks equal to the number of items in the list once for each item in the list, therefore performing a total number of checks equal to the number of items in the list multiplied by itself.

(c)

The algorithm still works as "i" will still increase until it is equal to n-1.

The nested loop that assigns values to "j" now compares the current value of "i" to the value of every item in the list with a lower index position than the value of "i". As the main loop still iterates through every item in the list any items towards the end of the list are checked against all items before them, so it does not matter that the nested loop does not check the value of items with index positions greater than "i" as any duplicate values will be found during the later checks.

(d)

The algorithm will run approximately twice as fast as the nested loop now only assigns values to "j" that range between 0 and i-1. This means that less of these loops are run throughout the running of the algorithm, allowing it to complete its intended task in approximately half of the time.

(e)

The time complexity of the algorithm is no longer quadratic as it no longer compares the value of every item in the list to that of every other item in the list. As the algorithm only checks part of the list in each nested loop the time complexity is now logarithmic.

(f)

According to the Python Wiki (https://wiki.python.org/moin/TimeComplexity) both the average case and worst case time complexities for the sort() function are O(n log n).

(g)

The time complexity of the algorithm is O(n log n) + O(n) as it performs the sort() function and then performs a for loop that has a linear time complexity.

(h)

The second algorithm is likely to run faster with a larger list as the first algorithm is quadratic and therefore has a runtime based on the number of items in the list squared. This means that as a larger number of list items are added the runtime of the first algorithm will increase greatly, whereas this increase is not as severe when it comes to the second algorithm.

(i)

The first algorithm may be chosen over the second algorithm in cases where the list has very few items, as the second algorithm relies on the sort() function which has a time complexity of O(n log n). This makes the second algorithm slower in cases where n^2 is lower than (n log n).
