# Two Sums

## Whiteboard
![Two Sums whiteboard](https://example.com/images/twoSums.png)


## Algorithm

Steps:

1. Initialize an empty hash map called numMap to store numbers and their indices (index and position).

2. Loop through the array of numbers nums:

* For each number at index i, calculate the complement as complement = target - nums[i].
* Check if the numMap already contains the complement as a key. If it does, you've found a pair of numbers that sum up to the target:

  * Return an array containing the index associated with the complement in numMap (which is the index of the first number in the pair) and the current index i (which is the index of the second number in the pair).
* If the complement is not in the numMap, add the current number to the map along with its index i.

3. If the loop completes without finding a solution (i.e., no pair of numbers sums up to the target), handle this according to your needs (throw an exception, return an indicator, etc.).