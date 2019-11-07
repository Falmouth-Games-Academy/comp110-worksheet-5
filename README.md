# comp110-worksheet-5

a.) Checks for duplicate elements in a list

b.) If there are no duplicate elements, the algorithm has to check the entire list for each element in the list, I.e.: n times by n

c.) The algorithm would simply not check previous values of i, but would still function as intended

d.) The algorithm won't waste time rechecking previous values, so the algorithm is completed nearly twice as fast

e.) The time complexity of the algorithm is still quadratic, because the maximum running time is now (n^2)/2 which is still quadratic

f.) O(nlogn) (https://stackoverflow.com/questions/14434490/what-is-the-complexity-of-this-python-sort-method)

g.) O(n) becasue after the list has been sorted the algorithm only needs to go through the list once to check for any duplicate elements next to each other

h.) The second is more likely to run faster the larger the list is - if you ignore the time taken to sort the list - as the list has only needs to be checked through once, guaranteeing that a duplicate will be found in that check if there is one, while the first algorithm may not find a possilbe duplicate on it's first pass

i.) The time taken to sort the list in the second program might mean that it's more benefiial to use the first program instead
