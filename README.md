# comp110-worksheet-5
Base repository for COMP110 worksheet 5

(a) The algorithm checks for duplicates from 0 to the input n.

(b) This is the worst case because if the algorithm was quadratic, the time required to search would double.
The input is n, the outer loop will carry out its task and the inner loop will also carry out its task, making it n^2.

(c) The algorithm is still correct because the first .

(d) It would run twice as fast as it does not need to check every number as it has a limit of i.
It would only count up to i, which basically means it halves the amount of items to look at.

(e) Yes the algorithm is still quadratic as it works with the O(n^2) notation.
This algorithm still doubles the list of objects in the list.

You can work out how the algorithm is still quadratic by using an equation and removing the coefficient.

Return True, is a simple line of code so it would take one step to complete. so this line is O(1), as it will always take one step, it is a constant.

The return false is the same so there is another O(1). Another constant*

So far we have O(1) + O(1), which will give us O(1). but the algorithm isnt a constant its a quadratic, so here is how we figure it out.

There are 2 for loops, and 2 lists. This means that because 1 of the for loops are inside the other for loop, there is an array within an array, otherwise known as a 2d array.
This is an easy outline as to why the algorithm is still quadratic, we can say there are 2 axis as an example.
I will make an example of a 2d array here:

	2d array = [[1, 2, 3, 4]
				[5, 6, 7, 8]
				[9, 10, 11, 12]
				[13, 14, 15, 16]]
				
Here you can see my 2d array. Now because we already have O(1) + O(1) in our equation, we can find another part by looking at how many for loops there are in our algorithm.
There are 2 for loops, this means that whatever big O notation is inside the second for loop will be multiplied by n^2.

So now we have O(1) + n^2 * O(1) + O(1), this is our equation now and we can find out how this is a quadratic time complex.
Lets say that T3 = O(1) + n^2 * O(1) + O(1), we can get rid of the 3 constants easily because we know that 2 O(1)'s is still O(1), and its the same with 3 or any number of constants.
Now lets say c3 is our expression for the 2 O(1)'s and c4 is the expression for the O(1) multiplied by n^2.
Now we have T3 = c3 + n^2 * c4 and we get rid of the coefficient, which are the c's, and we're left with n^2.
The n^2 is what goes in the brackets in O(n^2).

(f) The time complexity is O(nlogn) with reference to: (https://en.wikipedia.org/wiki/Time_complexity#Quasilinear_time)

(g) So first off, we see that we have a new line of code 'sort(list)'
this just sorts the list out in order to make it easier for the computer to find the user's desired item.
Now, n is our input, and there is a list which has our values in. the sort function will sort the list into sub-lists with a limit on the number of items each sub-list contains in proportion to the input.
Now, since this sounds like a linear time complexity algorithm, it isnt because of the sub-lists, so if the input increases, the amount of numbers increases and the amount of sub-lists increases.
So this is a gradual increase in time as there are more items added to the input.
What the algorithm will do, is sort the sub-lists into pairs, sorting them, and then sorting the pairs into another list until a full list is remade.

As an example, n is the input, so n * i. i is the list. log n = i, so this is n * log n. The big O time complexity is linearithmic. O(n log n)
														   2						 2
														   
(h) The second algorithm will run faster since n^2 will double the input, meaning it will double the time depending on how big the input is.

(i) They may choose the slower algorithm simply because they could use a programming language that does not have sort functions.