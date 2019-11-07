# comp110-worksheet-5
Base repository for COMP110 worksheet 5

a)
	Checks the whole list for duplicate.
	if the i and j position arent the same but the value in the list is than it will return true.

b)
	For every extra element in the list it will quadruple the running time.
	The reason being that every element has to be cross checked with each other.

c)
	It will still check every element in the list for doubles.
	Instead of using n as an outside limiter it will immediatly use i as the end point.
	Which makes it faster on execution.

d)
	Instead of running to seperate counters it will only need to run 


e)	
	It is still quadratic, since you still check every entry with each other.

f)
	Python uses Timsort by default which is O(n log n)
	source: https://en.wikipedia.org/wiki/Timsort
	
g)
	O(log n). this is the best case where you find the duplicate on the first time it goes through the list
	O(n log n) would be the average and worst case if you have to go through multiple iterations.

h)
	Quadratic, first one, is slower with longer lists since it has to go through all the options before it ends.
	the second one would be better since you have less iterations regardless of how long it takes.

i)
	Depending on the length of the list size the "slower" one is better for longer lists.
	where as the "faster" one takes longer the more items you put into a list.
