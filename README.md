# comp110-worksheet-C
Base repository for COMP110 worksheet C  

#### A)  
Procedure HasDuplicate(list) goes through all the elements of the list and compares it to all the other elements of the same list (skipping over the element it is checking) if it finds a match it returns True if it get to the end of the list without a match it returns False  
#### B)  
The worse case scenario is quadratic because if there is no match it has to go through all the list elements again each time 'i' increases.  
#### C)  
The algorithm is still correct because it tests the list[i] against elements up to 'i-1' all the elements after 'i-1' will be tested as 'i' increases.  
#### D)  
The Algorithm is approximately twice as fast because it checks an element against another only once, it will also never test it against itself so the 'i != j' could be removed from the if statement. so for example if i == 0; j = i-1 == -1 so it just skips over it as i increases by 1. When i == 1; j = 0; so the second element is test against the first element, i == 2; j = 1 so the third is tested by the first and seconded element and so on...  
#### E)  
No! it would be O(n*2) as it only tests any element against another only once.  
#### F)  
https://wiki.python.org/moin/TimeComplexity  
O(n log n)  
#### G)  
O((n log n) + (n-1)) but i think it would be expressed as O(n log n) because 'n' is so small compared to 'n log n' which is the main time complexity there’s no need to add 'n-1' to it.  
#### H)  
The second would be faster for larger lists. for larger list it is faster to do a binary sort first then test the previous element against the next as once there sorted if there the same they will be next to each other. where as if its not sorted you would have to test all elements of the list against all the other elements of list each time i increases.  
But if its the same algorithm used as (C, D, E) that would be faster than both. (i think)  
#### I)  
A programmer might choose the "slower" algorithm because it is easier to read and maintain  
