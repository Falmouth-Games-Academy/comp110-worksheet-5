# comp110-worksheet-5
COMP110 worksheet 5 completed by James Berry

## (a)
Checks _every index_ in a list against _every index_ in the same list,
if it is checking one index against a different index and they are the same,
then it _returns true_ to indicate that _there are duplicate elements_ in the list.

## (b)
The worst case scenario for this is if there are no duplicates in the list so the algorithm checks every index in the list , so for instance index when variable **i** is at **n - 1** and variable **j** is at **n - 1** where **n** is the length of the list. As both of these are linear searches we can take the product of both as the computation time
So the product of **(n - 1)** * **(n - 1)** would be **n^2 - 2n + 1**, when dealing with computation time,
you take the largest value, which in this case would be **n^2**. 

Therefore the worst case running time of the algorithm can be expressed as a quadratic or more specifically **_O_(n^2)**

## (c)
Changing line 4 will change how the algorithm checks the list but not the result of it.
Originally it will run every item in the list by using the variable **i** against the items in the same list by using the variable **j**.
After the change it will run every item in the list using variable **i** against every item that variable **i** has already passed through by using variable **j**. By using this method it will check through all of the elements in the list, but by checking only those that **i** has already been to, ending in **i** reaching the end of the list and checking against **j** which would be one index from the end of the list.

## (d)
The algorithm will take a longer time to run the further into the list it is checking, this is because as **i** increases, so does the amount of indices that **j** will check, this will increase linearly, but will since it starts with such a small amount of indeces to iterate through, the time can be averaged as if it checked half of the list each time, we can infer that it runs in half the time and therefore half of the time
