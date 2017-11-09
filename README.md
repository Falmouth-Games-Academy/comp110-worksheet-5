# comp110-worksheet-C
<<<<<<< HEAD
Base repository for COMP110 worksheet C (Arturs Zingis)


**Algorithm:**

	procedure HASDUPLICATE(list)
	let n be the length of list
	for i = 0, 1,..., n - 1 do
	for j = 0, 1,..., n - 1 do
	if i =/ j and list[i] = list[j] then
	return true
	end if
	end for
	end for
	return false
	end procedure


A) O(n). This algorithm sets two lists with i/j and for every item in the list, it takes away 1 from the length of the list and then checking if both lists are equal and if they are then return true and if not, return false. 

B) It would be the worst case scenario because we would have go through the list n times and with each iteration, you would have to go through the first loop. Which would take double the time.

**Algorithm 2**

	procedure HASDUPLICATE(list)
	let n be the length of list
	for i = 0, 1,..., n - 1 do
	for j = 0,..., i - 1 do
	if i =/ j and list[i] = list[j] then
	return true
	end if
	end for
	end for
	return false
	end procedure

c) This loop will carry out the same operation but instead of referring to the number of lists in the (j), it will link back to the first (i) list. The result of the (i) list -1 will determine (j).

d) The second algorithm will perform better because the function depends on the loop within the list (i) as well as the number of operations is halved as the number of elements is less. This algorithm is O(1).

e) This algorithm is no longer quadratic because it doesn't take another number for the length of the list but instead uses the first list - 1 to figure out what the value is which reduces the operation time as there is a lack of elements.
 

**Algorithm 3**

	procedure HASDUPLICATE(list)
	let n be the length of list
	sortedList <- SORT(list)
	for i = 1, 2,..., n - 1 do
	if list[i - 1] = list[i] then
	return true
	end if
	end for
	return false
	end procedure

f) O(n log n)

From: [https://wiki.python.org/moin/TimeComplexity](https://wiki.python.org/moin/TimeComplexity "Reference")

g) Using binary search to find largest/smallest number in the tree and the basic concept of this is to reduce the problem size with each iteration. As the number of elements increases, the operation time increases. The time complexity is bad.

h) If the input list is large, then the O(n log n) would be the fastest as a with a large list, this sort will try break down the problem with each iteration but with O(n), it is more linear and require more steps to perform the sort.

i) The slower algorithm may perform less elements but in a faster time rather than more elements in a slower time.
=======
Base repository for COMP110 worksheet C
>>>>>>> 57a794b904cdc6f40c6ec71149247b3637e6d0e5
