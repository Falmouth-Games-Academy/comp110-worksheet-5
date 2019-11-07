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
