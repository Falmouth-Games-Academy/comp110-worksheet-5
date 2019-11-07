# comp110-worksheet-5
Base repository for COMP110 worksheet 5

a) This algorithm uses the length of list – 1 for i and j and then asks if i is not equal to j and list[i] is equal to list[j] then True is returned otherwise False is returned. So essentially it asks if two items in the same list are the same then true is returned. If they aren’t the same then we get False.

b) Because i and j are both equal to 0 to n-1, so the algorithm takes n^2 operations. Which means that if the size of the list is doubled then the time taken to go through this algorithm will quadruple meaning that it is quadratic.

c) The algorithm is still correct because i is equal to 0 to n – 1 anyway. 

d) It will run twice as fast because we’re incrementing j at the same time as i rather than incrementing them separately. 

e) Yes, because the algorithm still takes n^2 operations. 

f) 0(log n) 
(https://stackoverflow.com/questions/14434490/what-is-the-complexity-of-this-python-sort-method)

g) 0(n), I think that it’s linear because the list is sorted before being searched, which means that the list will be searched linearly. 

h) The first algorithm because the list doesn’t have to be sorted first to search. And if the input list is large then sorting the list will increase the amount of time taken. 

i) A programmer might choose to use the slower algorithm over the faster one because the list will be sorted and then the list can be used more efficiently in other areas of the program. 
