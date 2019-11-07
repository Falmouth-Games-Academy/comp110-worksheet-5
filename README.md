# comp110-worksheet-5
#James Vanstone Comp110 Worksheet 5

##Computational Complexity

An implementation in Python to aide in code understanding.
def HASDUPLICATE(alist):
	n = len(alist)
	for i in range(0, n-1):
		for j in range(0, n-1):
			if (i != j) and (alist[i] == alist[j]):
				return True
	return False

#Question 1. 
(a) State what task this algorithm performs.
- This program is designed to check all the elements in a list to see if there are any repeated variables.

(b) Explain why the worst case running time of the algorithm is quadratic, i.e. O(n²).
- This program is quadratic because it has a nested loop where both loops iterate through all elements of the list. This means that the complexity is O(N²) ↵
	due to the number of operations being N*N.

Now suppose that the for loop on line 4 is changed so that j ranges from 0 to i - 1.
(c) Explain why the algorithm is still correct.
- The algorithm is still correct because each comparison is still being made once, i vs j. The j vs i comparison is being dropped by this change. ↵
	In the previous algorithm, every value in the list was being compared twice.

(d) Explain why the algorithm will run approximately twice as fast.
- Because only half of the operations are taking place, because the j vs i comparison is not happening after the i vs j.

(e) Is the time complexity of the algorithm still quadratic? Explain your answer.
- The time complexity is still quadratic because the number of operations is still within a nested loop. It's simply O(0.5n²) which is still quadraticly scaling because we disregard ↵
	any constant multipliers, resulting in a simplified complexity of O(n²).

(f) With reference to an appropriate source, write down the time complexity of Python’s built-in sort function, in big-O notation.
- The time complexity of python's list.sort() method is O(n log n)[1]

1: procedure HASDUPLICATE(list)
2: let n be the length of list
3: sortedList   SORT(list)
4: for i = 1; 2; : : : ; n - 1 do
5: if list[i - 1] = list[i] then
6: return true
7: end if
8: end for
9: return false
10: end procedure

(g) Thus write down the time complexity of the above algorithm in big-O notation. Explain your answer.
- The time complexity is:
	list.length = O(1) + list.sort = O(n log n) + for loop = O(n) + if = O(1)
	∴ O(2) + O(n log n) + O(n)
	∴ Complexity = ~O(n)

(h) If the size of the input list is large, which of these two algorithms is likely to run faster? Explain your answer.
- The second would run much faster due to it's time complexity being O(n) against the O(n²) of the first. This means that for much larger data sets, it ↵
	would not dramatically increase in number of operations where the first would scale much faster.

(i) Suggest one reason why a programmer might choose the “slower” algorithm over the “faster” one.
- The programmer may not have an efficient sorting algorithm or may have problems writing their own, so the first algorithm would be simpler to implement ↵
	especially where a small data sample is used.

#Bibliography:
[1] "Time Complexity", Jun 2017, url="https://wiki.python.org/moin/TimeComplexity", accessed 7th Nov 2019