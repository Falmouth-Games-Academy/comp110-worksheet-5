### comp110-worksheet-5
Base repository for COMP110 worksheet 5


### Question A

The algorithm compares the two lists; it compares all the items and sees if they match. If it finds any matches then it returns "True", if not then it returns "False" and exits the for loop.


### Question B

Running through quadratic would be the worst case because it would take longer compared to other complexities. Using the bubble sort method, doubling the items in the list would actually quadruple the time it takes hence O(n<sup>2</sup>). Not only that but going through all the items in the list is mandatory unlike with a binary search.


### Question C

Both for loops are still going through the same list. for i goes from 0 to n - 1. n is the length.


### Question D

Again both for loops are connected. J is going through the loop of i and therefore the algorithm will run twice as fast as it only needs to check the length of one loop


### Question E

The time complexity is not Quadratic. I believe that it is now linear O(n) because the J for loop now feeds into the I for loop which makes the algorithmn twice as fast. It moreso fits linear now because linear is known for being "faster" than quadratic. Because both for loops are now essentially the same; It has a time complexity of "comparing" the length of n to one set of items - O(n)


### Question F

Sources:<br>
The Python Wiki and Wikipedia<br>
https://wiki.python.org/moin/HowTo/Sorting<br>
https://en.wikipedia.org/wiki/Timsort<br>
Python has a Timsort algorithm created by Tim Peters. The Big O notation is as follows:<br>
Worst case performance = O(nlogn)<br>
Best case performance = O(n)<br>
Average case performance = O(nlogn)<br>
Worst case space complexity = O(n)<br>


### Question G

For the algorithm above<br><p>Best case performance: O(n<sup>2</sup>)<br>
I believe Quadratic complexity would be the fastest because they are both the same list with a difference of minus 1, therefore if you were to use a bubble sort method, it wouldn't have to rerreange the items in numerical or alphabetical order for both loops.<br><p>
Worst case performance: O(n)<br>It would be a waste to search through all the items in loops that are almost identical<br><p>
Average case performance:<br>
Worst case space complexity:


### Question H

The second algorithm would run faster because the two loops are similar. Both algorithms use Quadratic time complexity which means that doubling the lists would make the time it takes to search quadruple but for the second algorithm, the similarity would make it a faster performance than the first.


### Question I

Having a "slower" algorithm could potentially be easier to debug. You may be able to notice errors easier


