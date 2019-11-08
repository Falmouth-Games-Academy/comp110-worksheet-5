# comp110-worksheet-5
Base repository for COMP110 worksheet 5


a) The algorithm compares each element of the list with every other one. If it finds two equal elements in different positions of the list, it returns TRUE. If it doesn't detect any duplicate values, the algorithm returns FALSE.

b) The procedure HasDuplicate is a compound algorithm because of its nested loops. For each run of the loop of line 3 (O(n)) it goes through the loop on line 4 n times (O(n)). Because of this, we get an algorithm which has quadratic time (O(n^2)).

c) It's still correct because the algorithm will still end up comparing every value of the list with each other, thus achieving its goal.

d) With the first iteration of the algorithm, it would compare every single element of the list with every other one. However, since every individual element was always compared to every other one, every comparison would eventually end up being repeated. As an example, if i was 5, the algorithm would compare all other elements of the list with list(5). In the next loop, with i being 6, it would compare every element with list(6), including list(5), a comparison which had just been performed in the previous run of the loop. In the new iteration of the algorithm, it would only compare an element of the list with all the elements before it, making the earlier runs of the loop significantly faster, and they would get progressively slower as the algorithm kept running. However, the only time it would take roughly as long as a run of the algorithm's previous iteration would be if it reached the point where i = n-1, as only then would i be compared to every single other element of the list (except itself).

e) 

f) O(n log n) https://wiki.python.org/moin/TimeComplexity

g) 

h) The second one, as it only does one comparison per value of i, as opposed to the first one which does multiple.

i) The programmer might want to be looking for what the first duplicate value is in the list's original form. The second algorithm sorts it, thus making this impossible.
