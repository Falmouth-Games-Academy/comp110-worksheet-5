# comp110-worksheet-5
Base repository for COMP110 worksheet 5


A)

The algorithm goes through the list and increases the index in the list incremently checking if two numbers in two seperate positions are the same, if so it will exit the procedure. However it also has a fail safe to stop the program from detecting the numbers as duplicates when they are in the same index in the list. 

B)

This algorithm loops through the j loop n-1 number of times, as does the i loop. However because the j loop is nested in the i loop thaat means that the equation for time would be (n-1)(n-1) which expanded would be n^2 - 2n + 1. When we try to find out how long the a program will take we always use the slowest time complexity which in this case is n^2.

C)

the algorithm is still correct because of the fact that orginally n was used as a variable for the length of the list this is still true in the case of the i loop. However when we use i - 1 for the j loop then that means that j is only checking the items in the list that are before the postion that i is in. This means that j is not checking the whole list everytime i checks 1 item, which makes the procedure able to be executed faster.

D)

The implemention of the i - 1 into the j loop means that it will run approximately twice as fast because j has to do half as many checks on the list.

E)

Yes the time complexity is still quadratic because of the fact that in a worst case scenario i and j both have to go through the whole list. In a worst case scenario n - 1 and i - 1 are exactly the same, which means that the formula for the time complexity is still (n-1)(n-1) which is still expanded and simplified to O(n^2). 

F)

O(n log n)      https://wiki.python.org/moin/TimeComplexity

G)

The time complexity of the algorithm is O(n log n), this is because the formula for the whole algorithm is (n-1)+(n log n), the -1 can be canceled out first as it is the fastest, followed by the n in the n-1 statement. This leaves us with our slowest and our final result for the time complexity which is O(n log n). 

H)

The second algorithm would run faster because the big-O notation for the second algorithm is faster, this is because it has a lower time complexity.

I)

A programmer would be likely to choose a "slower" algorithm if the list was over 100 as the O(n log n) time complexity is only faster if the list is over 100 whereas if the list is below that limit then the O(n^2) is faster.
