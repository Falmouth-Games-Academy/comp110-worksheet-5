# comp110-worksheet-5
COMP110 worksheet 5 completed by James Berry

## (a)
Checks _every index_ in a list against _every index_ in the same list,
if it is checking one index against a different index and they are the same,
then it _returns true_ to indicate that _there are duplicate elements_ in the list.

## (b)
The worst case scenario for this is if there are no duplicates in the list so the algorithm checks every index in the list , so for instance index when variable **i** is at **n - 1** and variable **j** is at **n - 1** where **n** is the length of the list. Since the indices of the two variables are expressed in terms of **n**, it means that the time taken will scale linearly as new elements are appended to the list. As both of these are linear searches we can take a product of the linear algorithms as the total time taken for the full algorithm. Linear algorithms can be expressed as **_O_(n)** and since we have two we can get the equation: **n * n** which can be simplified to simply **n^2**
Therefore the worst case running time of the algorithm can be expressed as a quadratic or more specifically **_O_(n^2)**

## (c)
Changing line 4 will change how the algorithm checks the list but not the result of it.
Originally it will run every item in the list by using the variable **i** against the items in the same list by using the variable **j**.
After the change it will run every item in the list using variable **i** against every item that variable **i** has already passed through by using variable **j**. By using this method it will check through all of the elements in the list, but by checking only those that **i** has already been to, ending in **i** reaching the end of the list and checking against **j** which would be one index from the end of the list.

## (d)
The algorithm will take a longer time to run the further into the list it is checking, this is because as **i** increases, so does the amount of indices that **j** will check, this will increase linearly, but will since it starts with such a small amount of indeces to iterate through, the time can be averaged as if it checked half of the list each time, we can infer that it runs in half the time and therefore half of the time

## (e)
The first _for loop_, represented as **i**, has not changed and is still a linear equation. The second _for loop_, represented by **j** however, has been changed; the time taken by **j** has a much lower average time as a constant than before, but it relies on where **i** is in the list and therefore will still increase in time as **n** increases, and is therefore still a linear search. Using the method I showed in part (b), I can assume that the product of the two linear searches is still a quadratic, although it will get exponentially faster than the algorithm in part (b) as **n** increases.

## (f)
The [Python documentation of time complexity for various functions](https://wiki.python.org/moin/TimeComplexity) gives the time complexity of the _sort_ function as **_O_(n _log_ n)

## (g)
First of all, the algorithm calls the sort method which has a notation of **_O_(n _log_ n)**
The second part of the algorithm then has a search based on the length of the list which as previously explained has a notation of **_0_(n)**.
We can therefore assume that the full time complexity would be **(n _log_ n) * (n)**, simplified to **(n^2 _log_ n^2)**. Meaning that the proper notation of the algorithm is **_O_(_log_ n^2)**.

## (h)
I think that the second algorithm will run faster with a larger input list, this is because as a logarithmic function, as larger input lists are used, it will take less and less additional time compared to shorter lists, This will counteract the effect of the exponent, and will make it a lot slower than that of the first algorithm which has only an exponent.
