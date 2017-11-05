# comp110-worksheet-C

(a) It checks a list for duplicate items, if it finds any then it will return true, otherwise false.

(b) The worst case is quadratic because it loops through the whole list for each element in the list, for the duplicate check. So if the only duplicate item is at the end then it has to have done O(n2) - 1.

(c/d) It will still check every element against each other apart from now it will excude chekcing both ways for example a == b and b == a will now just be checked once so a == b.

(e) It is now no longer quadratic because it now only has to do half the checks it originally did so 0(n2) will now be 0(n2) / 2.

(f)
