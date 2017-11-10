# comp110-worksheet-C
Base repository for COMP110 worksheet C

1: procedure HASDUPLICATE(list)

2: let n be the length of list

3: for i = 0, 1, . . . , n − 1 do

4: for j = 0, 1, . . . , n − 1 do

5: if i 6= j and list[i] = list[j] then

6: return true

7: end if

8: end for

9: end for

10: return false

11: end procedure

A) State what task this algorithm performs.
This aglgorithm is a duplicate check on a list of figures , it starts with two sets of lists i and j for each sets of figures , the aglorithm takes 1 for the length of the list to check if both lists are running equal to each other if both are equal then it will return true if both lists are not equal it will return false.  
