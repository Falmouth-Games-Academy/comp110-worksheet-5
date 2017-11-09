# comp110-worksheet-C
Base repository for COMP110 worksheet C
```
1: procedure HASDUPLICATE(list)
2: 	let n be the length of list
3: 		for i = 0, 1, . . . , n − 1 do
4: 			for j = 0, 1, . . . , n − 1 do
5: 				if i != j and list[i] = list[j] then
6: 					return true
7: 				end if
8: 			end for
9: 		end for
10: 	return false
11: end procedure

```
## a State what task this algorithm performs
For each element in array i compare to each element in array j. If 2 elements are not in the same position in the list and they hold the same value then there is a duplicate, else there is not.
## b Explain why the worst case running time of the algorithm is quadratic, i.e.O(n^2).
The search mamkes use of 2 liniar searches resulting in a quadratic search. This is due to the combination of nested loops resulting in the worst case being O(n^x) where x is the number of nested loops in this case 2. 

Now suppose that the for loop on line 4 is changed so that j ranges from 0 to i − 1
## c Explain why the algorithm is still correct.
As the elements have to be in the same position to count as a duplicate there is no need to check any positions in array j after the position that the element holds in list i as it will always return as false.
## d  Explain why the algorithm will run approximately twice as fast.
The algorithm is only checking up till the element number of the element in list i in list j. As such it only check the first element on the first itteration and will work up to all of the elements in the final itteration, this will average out to 50% run time or twice as fast.
## e Is the time complexity of the algorithm still quadratic? Explain your answer.
Yes there are still 2 nested search algorithms and as such it will always be quadratic even though it is made much faster by the change.
Now consider the following algorithm, which performs the same task as the
first:
```
procedure HASDUPLICATE(list)
	let n be the length of list
	sortedList ← SORT(list)
		for i = 1, 2, . . . , n − 1 do
			if list[i − 1] = list[i] then
				return true
			end if
		end for
	return false
end procedure
```
## f With reference to an appropriate source, write down the time complexity of Python’s built-in sort function, in big-O notation
The sort function in python makes use of the syntax ```Sort()``` the details of which can be found in the python documentation here [https://docs.python.org/2/howto/sorting.html] and according to the python wiki [https://wiki.python.org/moin/TimeComplexity] the time complexity can be called as O(n log n).
## g Thus write down the time complexity of the above algorithm in big-O notation. Explain your answer
The algorithm above has to sections to it, the sort which makes use of the python inbuilt sort function gives this section the time complexity of O(n log n). The second section is a liniar search which has a time complexity of o(n). Due to the nature of "big O notation" it only looks at the most significant factor and in the case of the algorithm above this is the logarithmic sort, due to this the time complexity is defined as O(n log n). 
## h If the size of the input list is large, which of these two algorithms is likely to run faster? Explain your answer.
The second algorithm will be faster with larger sets of data due to the sorting of the data and the ability to merely check the element prior to the current element rather than having to check multiple elements. The only time it would be faster to use the first algorithm with small sets of data where the sorting of the data is redundent and simply creates an amount of inefficiency. 
## i Suggest one reason why a programmer might choose the “slower” algorithm over the “faster” one.
Faster search algorithms are usually more complex to code and also often require prior sorting of what is being searched. A novice level programmer may struggle with this as they are much harder to code and there is often much more code or more complicated syntax involved in there more efficient searches that a novice programmer would not have the knowlege to use and/or understand.