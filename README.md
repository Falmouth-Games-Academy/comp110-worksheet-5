# comp110-worksheet-C
Base repository for COMP110 worksheet C

#### (a)
The algorithm performs a search of the list to find if there are any duplicate items

#### (b)
The worst possible running time is O(n^2) because the program might have to run to full length linear searches to find a duplicate ( the duplicate items are the last 2 items)

#### \(c\)
The algorithm is still correct, as the second loop only scans the values prior to the item selected by the first loop.

#### (d)
The algorithm will run about twice as fast, as it is removing a lot of extra searches. It doesnt search every value against every value, it only searches previous values against each value - which cuts out a lot of extra searches at the start of the list

#### (e)
The time complexity is still quadratic, as it is still one linear search within another linear search.

#### (f)
The sort function in python uses a Timsort, which has an an average and worstcase time complexity of O(n log(n)) - https://en.wikipedia.org/wiki/Timsort 

#### (g)
The complexity of the algorithm uses both a linear search and a TimSort. The total complexity of this is O(n log(n)) + O(n), which results to a overall complexity of O(n log(n))

#### (h)
The first algorithm has a complexity of O(n^2) and the second has a complexity of O(n log(n)). O(n^2) is a higher complexity so the new algorithm with the sort can be expected to run faster

#### (i)
If new items where to be added to the list, the first (slower) algorithm could easily pick up where it left off and continue checking for duplicates. If you wanted to add items for the second algorithm, the whole sort would have to be done again. In this situation, while the time complexities remain the same, the slower alogithm would have less worse case iterations to run (if it continues where it left off) then the faster sort, where it has to do everything again.
