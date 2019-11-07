# comp110-worksheet-5
Base repository for COMP110 worksheet 5

(a)

this algorithm compares each item of the i and j lists and checks if their values are the same. After comparing two values, it will either keep comparing the next two until the list is finished, where it will return false and end the loop, or if the algorithm detects if two values are the same, it will return true and end the loop.

(b)
Because a for loop is being run within a for loop, this creates a nested loop and therefore a quadratic running time.

(c)
This algorithm would still be functional, as n represents the same length for i and j. Because i and j have the same total length,  i can be used to represent the length of j.


(d)
Doing this would allow the program to only have to calculate the value of one list. Processing the length of both lists would only need to be done once by i, and j can simply reference the result.


(e)
Yes, it would be as the j loop is still present, while highly simplified. This still means that there is a for loop being run based on a for loop, being a nested loop - meeting the criteria of a quadratic time complexity.

(f)
The time complexity of python's sort function is O(n log n) [1]


(g)


O(n) - As this represents the addition of each value in the list until n is reached, being the most complex item in the list, and therefor the most impactful to the time complexity.


(h)

The second algorithm would run faster, as there are only 2 embedded loops, rather than the first algortithm's 3.

(i)

The slower algorithm might take longer, but could use less space in the system's memory, while the faster program may use more.

References:
[1] Via Wikipedia - on https://wiki.python.org/moin/TimeComplexity