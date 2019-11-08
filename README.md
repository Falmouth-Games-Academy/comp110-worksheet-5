# comp110-worksheet-5
Base repository for COMP110 worksheet 5
a) This algorithm performs 2 seperate loops of the same list one within the other, then compares them to see if any entries which are the same. If the i and j compared are the same value and is not the i and j of the same value (eg i = 2 and j = 2), the algorithm returns true, otherwise if after performing the entire algorithm without finding a single duplicate, the algorithm returns false. a potential improvement can be if there are multiple duplicates we can create a list for all the duplicates we do find.

b) This is because the algorithm performs n loops n times which mathematically means n^2 (n squared) and as a time complexity O(n^2)

c) Say for instance n=5. variable i will go from 0 - 4 and j, 0 - 4. i and j being the same will be irrelevant as i and j of the same number are going to be the same value. Therefore if j was changed to 0 - (i - 1), in our case this becomes 0 - 3 and the last check will be i = 4 and j = 3 allowing the algorithm to still perform the same task correctly.

d) Lets say n=5 again. variable i will go from 0 - 4 and j, 0 - 3. 

e) The time complexity is still quadratic because if it has become twice as fast the time complexity has gone from O(n^2) (n squared) to O((n^2)/2) (n squared divided by 2), even if any non 0 constant was put onto this it should still be quadratic.

f) https://en.wikipedia.org/wiki/Timsort (analysis header)
Timsort's sort function has a worst time complexity of O(nlog(n)) and best of O(n)

g) Worst case O(nlog(n)) + O(n) or O(n + nlog(n)) and Best case O(2n). This is because the algorithm first needs to sort the list which takes time which will at worst be O(nlog(n), then it will need to check for duplicates however it only needs to go through the list only once so that will be O(n).

h) The second algorithm will be faster because the list only has to be sorted once and also only has to be iterated once comparing each i value with the one before it which massively saves time (and timsort already saves time on its own)

i) Assuming we use the improved version of the first algorithm (the first one without the improvement is still worse) it actually happens to be better only up to and including n=2 (if my answer to g is right). If we had many lists that happened to be of 2 length, using the sort involved algorithm will be more time consuming as it first has to sort and then find duplicates, however, because timsort does its job so well, anything n=3 or over (I found n=3 to be 4.43 compared to the first algorithm being 4.5).
