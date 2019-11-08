# comp110-worksheet-5
## A)
Checks every index in the list against a different index in the same list and returns true if two elements are the same and false if they are different.

## B)
The worst case scenario appears when there are no duplicates within the list causeing the alogithm to got through every element with in the list and return false. Since the algorithms are linear and therefore represented as O(n) and there are two of them we can multiply them together O(n) * O(n) to get O(n^2) which is a quadratic formula.

## C)
The code will still be correct because instead of going through the entire list it will only check the elements that i has already passed through by using j. So when i gets to the end of the list j will be one of the end of the list.

## D)
The code it going through less elements as when the index of i gets to say 8 j will be at i - 1 and therfore be 7 overall reducing the ammount of time that is taken up by not checking previously checked elements

## E)
Technicly speaking this should still be a quadratic as it is still 2 for loops with one indented within the other meaning it should still be n^2

## F)
The time complexity of pythons sort function is O(n log n) [StackOverflow](https://stackoverflow.com/questions/14434490/what-is-the-complexity-of-this-python-sort-method)

## G)
When we are dealing with time complexity we only need to care about the most dominant one in this case it would be O(n)

## H)
As long as the list is large enough i believe that the second algorithm would be faster as its liniar. Whilst the first algorithm will take longer on larger list cause as the number of items increases the time taken with n^2. So if there were 100 items the second algorithm would take 100^2 seconds/miliseconds to complete

## I)
They may choose the "slower" one when using a smaller list as a quadratic would be faster for smaller lists.
