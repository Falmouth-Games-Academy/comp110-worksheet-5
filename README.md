# comp110-worksheet-5
COMP110 worksheet 5 completed by James Berry

## (a)
Checks _every index_ in a list against _every index_ in the same list,
if it is checking one index against a different index and they are the same,
then it _returns true_ to indicate that _there are duplicate elements_ in the list.

## (b)
The worst case scenario for this is if there are no duplicates in the list so the algorithm checks every index in the list , so for instance index when variable **i** is at **n - 1**and variable **j** is at **n - 1** where **n** is the length of the list. As both of these are linear searches we can take the product of both as the computation time
So the product of **n - 1** * **n - 1** would be **n^2 - 2n + 1**, when dealing with computation time,
you take the largest value, which in this case would be **n^2**. 

Therefore the worst case running time of the algorithm can be expressed as a quadratic or more specifically **_O_(n^2)**
