# comp110-worksheet-C

(a) It checks a list for duplicate items, if it finds any then it will return true, otherwise false.

(b) The worst case is quadratic because it loops through the whole list for each element in the list (nested iteration), for the duplicate check. So if the only duplicate item is at the end then it has to have done O(n2) - 1.

(c/d) It will still check every element against each other apart from now it will excude chekcing both ways for example a == b and b == a will now just be checked once so a == b.

(e) It is now no longer quadratic because it now only has to do half the checks it originally did so 0(n2) will now be 0(n2) / 2.

(f) O(n log n) - https://wiki.python.org/moin/TimeComplexity

(g) O(n log n + n) - First the sort takes O(n log n) and then it only has to run through each item in the list once (+n) as any duplicates will be next to each other.

(h) If the list is large, the second algorithm (sorting one) will be faster as it doesn't have to loop as much.

(i) The slower algorithm is easier to understand because it may not be obvious at first how the faster one works with the sort function until you realise duplicates will be next to each other after the sort.
