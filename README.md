# Implement selection sort


## Constraints
* Is a naive solution sufficient (ie not stable, not based on a heap)?
    * Yes
* Are duplicates allowed?
    * Yes
* Can we assume the input is valid?
    * No
* Can we assume this fits memory?
    * Yes


We can do this recursively or iteratively. Iteratively will be more efficient as it doesn't require the extra space overhead with the recursive calls.

* For each element
    * Check every element to the right to find the min
    * If min < current element, swap

Selection sort might be a good option if moving elements is more expensive than comparing them, as it requires at most n-1 swaps.

The finding of a minimum element can be done with a min heap, which would change the worst-case run time to O(n log(n)) and increase the space to O(n). This is called a heap sort.