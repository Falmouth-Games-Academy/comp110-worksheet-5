# comp110-worksheet-C
Base repository for COMP110 worksheet C - Aidan Crossan

**a)** The algorithm performs a search to see if there are duplicate items in the same list (e.g. to see if there are more than two people in a list who have the name 'Garry' for instance).

**b)** The least efficient way of cycling through the list is to check each of the items in the list in pairs to see whether they match or not. This would be quadratic complexity O(n^2).

**c)** i-1 will still be similar to n-1, it just means that the j loop will be one behind the i loop. 

**d)** The two loops ran twice in the original version meaning it had to go through one list and then run it again to see if there was any overlap.

**e)** The time complexity is still quadratic as the task the algorithm performs is still the same. It's roughly twice as fast because it cuts down the number of searches by about a quarter.

**f)** [The Python documentation site mentions that Python uses Timsort under the 'Sort Stability and Complex Sorts' section.](https://docs.python.org/3/howto/sorting.html)

O(n log(n)) - Timsort

**g)** O(n log(n)) with the worst outcome being O(n). Timsort works by cutting down its sets of data (dividing it of sorts) into sets of similar sized data. This is similar to binary search which operates in a similar manner. It would be incredibly efficient for lists with a fewer items and would become increasingly less efficient once more items are added in.

**h)** The second algorithm would be faster as it works out duplicates without having to go through two loops simultaneously.

**i)** The slower algorithm may require less code to write and it allows for a bit more flexibility as there is only one 'for loop'.