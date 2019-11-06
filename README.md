# comp110-worksheet-5
Base repository for COMP110 worksheet 5

#a
Goes through a list and checks for duplicate values

#b
If there are no duplicates both loops will complete, meaning it will have to check each list[j] value against every list[i] value, leading to it checking n^2 values

#c
Since j and i are both working off the same list, in the changed code j contains all previous i values meaning by the time the code ends all values in the list will still be checked against every other value.

#d
Because it only checks each value against each other once, as opposed to twice.

#e
Yes because if there are no duplicates it will still compare both whole loops against each other

#f
python's inbuilt sort method is timsort, with a big O notation of O(nlogn) (cited: Nicolas Auger, Cyril Nicaud, Carine Pivoteau. Merge Strategies: from Merge Sort to TimSort. 2015.
hal-01212839v2f)

#g
O(nlogn) because otherwise you wouldn't've asked the previous question.

#h
O(nlogn) because 5000log5000 < 5000^2

#i
if they are pressed for time and the slower algorithm would be easier to implement
