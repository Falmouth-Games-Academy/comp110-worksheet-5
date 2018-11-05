# comp110-worksheet-C
Base repository for COMP110 worksheet C
(a) The algorithm checks through the list to see if it has duplicate entries in it. If it has, it returns true, if not it returns false.
(b) The algorithm is in quadratic time (O(n^2)) because the function checks item i in the list, then j increments through all posible positions in the list to check for duplicates. This means that for each item in the list you are checking the entire list.
(c) Because it is still checking every item in the list and seeing if it is duplicated, but is checking more efficiently.
(d) The algorithm runs faster because j is only iterating up to i - 1. Which means that at the start it is checking less items. 
(e) Yes, the algorithm is still quadratic (O(n^2)) because it is still a linear search within a linear search.
(f) Using the information presented in [1] We see that pythons Sort function uses a hybrid algorith called Timsort which merges Insertion sort and Merge sort. While Insertion sort has quadratic time complexity (O(n^2)) Merge sort has the larger time complexity of O(n log(n)) which means that it runs in logarithmic time.
(g) While the algorithm is might appear to be running in linear time, O(n), the sort function is still part of the algorithm which means that the time complexity is still in logarithmic time O(n log(n)) 
(h) The second algorithm will run faster with a larger list because logarithmic time complexity runs faster than quadratic time complexity.
(i) You might chose to run the slower algorithm because it is able to run through unsorted lists.
[1]https://www.geeksforgeeks.org/timsort/
