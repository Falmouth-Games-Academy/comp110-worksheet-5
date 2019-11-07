# comp110-worksheet-5
Base repository for COMP110 worksheet 5

A) The algorithm checks the elements in a list against a second list with both lists being the same size. If an element from List [i] in one position doesn't match the element from List [j] in the same position. Then the algorithm will return true, indicating that the Lists are not the same. If the opposite occurs, where every element in the lists are the same. Then the algorithm will return false, indicating that the lists are the same.

B) Using this algorithm, the worst case scenario of returning a True or False value would be quadratic because it is possible that every element in the list is the same, apart from the very last element. The algorithm would check the elements, in n<sup>th</sup> order, until there is a difference. For example, if there were 20 elements and the first 19 in each list were the same and the only different element in each list was the 20th. Then the algorthim would check 20 times, which is coincidentally the length of the list. This is a Quadratic Time complexity. The time of the search being equal to how many elements are in the list that have to be searched before a result is found. Quadratic Time complexity is also known as O(n<sup>2</sup>) time complexity.

C) The Algorithm is still correct as the function and what the code does remains the same, the way that it completes it is different. The first for loop remains the same and compares every element in the [i] list against the [j] list as normal. However the second for loop now doesn't compare that chosen element against everything in its list, which it was doiung before. It now only checks up to the value which [i] represents. So if i = 1, then the first element from the [i] list is being checked against the second list. Before the change, the second loop would check that element against every element up to n - 1 (The whole list). After the change, the second loop would only check that element up to the element position that is equal to what i - 1 is. In this case, that would be element position 0. Meaning that it only checks the element up to the first element in the second loop. Making it quicker because it will do less checks. 

D) The algorithm only does one comparison with each element instead of two comparisons, which will half the time.

E) Yes, because the outer loop would have to go to n regardless. The inner loop cycle depends on i, which in turn can still reach the value n. So both the outer and inner loop, in the worst case scenario, would still have to reach the value of n. Because of this, the time complexity notation is still quadratic, notated as O(n<sup>2</sup>).

F) The Time Complexity notation of python's built-in sort function is O(n Log n). [Source] https://wiki.python.org/moin/TimeComplexity

G) The algorithm goes through a list, comparing one element with the next one in the list. Going until it finds a duplicate in the list. Because of this the time complexity would be n + n log n which is notated as O(n) and known as linear time complexity. 

H) When the two time complexities, O(n<sup>2</sup>) and O(n), are compared with one another on graphs. The linear time complexity appears to raise a lot quicker than quadratic time complexity. So O(n) would run quicker, meaning that the second algorithm may run quicker.

I) A programmer may choose the "slower" algorithm over the faster one if they have a shorter list. The algorithm is actually quicker with fewer elements despite getting slower over time.
