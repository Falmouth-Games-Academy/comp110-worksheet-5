# comp110-worksheet-5
Base repository for COMP110 worksheet 5

##A)

The algorithm cycles through the entire list to check if there are any duplicates. It does this by cycling through each item of the list with j for each instance of i which also is an item of the list. It then checks to see if i and j are the same element of the list and if they aren't and the two items are the same then it returns true and ends the algorithm;

##B)

The worst case for this algorithm would be running through all possibilities and not finding any duplicates. In that case the list has to run through itself for every element. For example if the list was 10 items long then it would be running through all 10 items 10 times(10^2).

##C)

The algorithm would still run correctly after this change as it would only be checking values it hasn't checked before whereas with the previous algorithm it checked every element against itself. The reason this works is because both i and j are working off the same list so for example i[2] and j[3] is the same as i[3] and j[2]. This means that by only checking j as far as i has gone then you only check original values.

##D)

The algorithm would run twice as fast as its checking roughly half the values. For example with the old algorithm a list of 10 it would be chcking 10 x 10 values which is 100 however with the new algorithm it only checks 10 + 9 ... + 1 which works out to 55.

##E)

The time complexity is still quadratic as it is still using nested for loops which increase the value of j overtime expenentially increaseing the overall time to complete as the list gets longer.

##F)

[O(n log n)](https://wiki.python.org/moin/TimeComplexity)

##G)



##H)



##I)
