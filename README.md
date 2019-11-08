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
