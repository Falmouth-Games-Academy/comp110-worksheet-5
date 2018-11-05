# comp110-worksheet-C
Base repository for COMP110 worksheet C

# Paul Rauca's submission for worksheet C

## Answers for questions (a) - (i)

### (a)
	The presented algorithm performs an array-wide check for any duplicate elements and upon 
	finding one it returns 'true' and 'false' otherwise
	
### (b)
	The worst case running time of the algorithm would obviously be in the scenario in which
	all the elements are checked against each other. Since there are 2 for loops that iterate
	through the entire list EACH, that would come up as n iterations for the first loop, and
	for EACH iteration of the first one, an entire n-element loop is performed. That leaves 
	us with n x n elements iterated through, coming up to a total of n^2 steps =>
	=> Complexity of O(n^2)
### (c)
	* Question: having verified the code in Python, the syntax is still correct, however in the case of 
	C-based languages simply changing the range of j would cause errors (if i is 0, then j would go 
	from 0 to -1 with an implicit step of 1)
	* That said, the algorithm is still correct because now it simply checks
	all the elements before the one we are currently at (j <= i - 1).
	This means that even we are not checking all the elements with each
	other, instead we are doing the minimum amount of checks, checking each
	element with the others only ONCE
	* example: if there are 3 elements, the first one will not be checked with any,
	the second one will be checked with the first one and the last one
	will be checked with the other 2. If we turn that around, the first element
	was checked with the other 2, the second one with the other 2 etc.
### (d)	
	Because instead of iterating through n x n elements, for each element (of position i)
	we iterate through i elements.
	Thus, the total running time would be:
	(0 + 1 + ... + n - 1) = [n * (n - 1)]/2 ~ (n^2)/2
### (e)
	In accordance with the principles of complexity, the complexity 
	of O((n * n - 1)/2) can be reduced to O((n * n)/2) and even further to O(n^2).
	Therefore, yes, the complexity is still quadratic
### (f)
	According to the Python Wiki (https://wiki.python.org/moin/TimeComplexity), the
	built-in sort() function uses Timsort, an algorithm that has an average 
	time complexity of O(n logn)
### (g)
	The given algorithm can be broken down into: sorting the given list using Python's 
	built-in sort() (O(n logn)) function and iterating through the newly formed list (O(n)). Therefore, the
	time complexity of the algorithm is O(2n logn), which can be further simplified to
	O(n logn)
### (h)
	The 2 time complexities can be safely reduced to n * n and, respectively, n * log(n). For instance, if one were
	to calculate the limit of n^2/n*log(n) (http://www.wolframalpha.com/input/?i=lim+n+log(n)+%2F+n%5E2),
	it would result in 0, which means that n^2 will grow faster, making it less efficient in favour of n*log(n),
	if n is high enough (as in our case).
### (i)
	As previously stated, O(n*log(n)) is prefferable, but only when n is high enough. Therefore, 
	one may want to use the 'less efficient' method either for the sake of performance when 
	n is low enough, or for  the sake of code simplicity
	
