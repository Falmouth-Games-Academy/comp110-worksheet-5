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

## g Thus write down the time complexity of the above algorithm in big-O notation. Explain your answer

## h If the size of the input list is large, which of these two algorithms is likely to run faster? Explain your answer.

## i Suggest one reason why a programmer might choose the “slower” algorithm over the “faster” one.