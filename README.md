# comp110-worksheet-5
Base repository for COMP110 worksheet 5


### a.  
This algorithm uses for loops to go through a list and check for duplicates.   
n is the length of the list, i and j equal each variable in the list and it uses  
an if statement to check if the variable in i and j are not equal to eachother.  
This means if it goes through the list and i and j are not equal to eachother it  
returns true, whereas if they it returns false.  
  
### b.  
The worst case running time of this algorithm is O(n2) is because it involves  
two for loops where one is nested in the other. This means the time complexity is times itself leading  
to the n sqaured. Due to this with two for loops the slowest case of running time will be quadratic   
represented as O(n2) in big O notation.  
   
To double check my awnser I used this archived paper from western science.  
http://www.csd.uwo.ca/courses/CS1027b/notes/AnalysisIntro.pdf  
  
  
### c.  
The algorithm is still correct as it still uses a for loop to check through each list   
and will still return true if each list doesnt have duplicates and still return false if  
they do.    
  
### d.   
The algorithm will run much faster, as when an algorithm is quadratic the time taken to   
run increases rapidly for how much data it has to process. This is because the time complexity  
grows quadratiaclly as n increases. When the change is made to  
line 4 it has to process less data in the loops leading to a much faster runtime.  
  
  
### e.   
I believe the algorithm is still quadratic as it still involves 2 loops with one nested  
inside the other, it is just faster as the for loop on line 4 is more efficent time complexity wise  
meaning it has less time for the quadratic time taken to increase.  
  
### f.  
O(n log n)  
I used stack overflow as a source to find this.  
https://stackoverflow.com/questions/14434490/what-is-the-complexity-of-this-python-sort-method  
  
I also used a python developer paper on Sorting to double check the stack overflow source.  
  
Peters, T. (2019). Sorting. [online] Available at: https://mail.python.org/pipermail/python-dev/2002-July/026837.html [Accessed Nov. 2019].  
  
  
  
### g.  
O(n)  
 The algorithm above is only using one for loop  
 operation making it linear. O(n) represents linear time in   
big-O notation.  
  
### h.  
I think the second linear algothirm will run faster with a large input list.  
This is because with the quadratic algorithm as the list gets larger it becomes  
more and more increasingly slow, as the time complexity grows quadratiaccly as n   
increases. On the otherhand, the second linear algothirm only times itself by 1n  
making it much faster with a larger n.  
  
  
### i.  
Some programmers may choose the "slower" algorithm because it is easier to   
write, read and mantain, whereas the "faster" algorithm may be harder  
to understand and change. Even when a list is long the time difference   
between a "slow" and "fast" algorithm will usually be very small, for   
example less only a few milliseconds.  
  
Another reason the programmer might choose the first algorith is because if  
it is only using a small list the "slower" quadratic algorithm could be faster as it doesn't have   
to use the sort function that the second algorithm does. However, if the list increases  
it would be better to instead use the second linear algorithm as it becomes more time  
efficent when the list is large.  
  
