# Algorithm
### Input Handling:
The program takes two inputs from the user: a sorted integer array (nums) and an integer n.

### Algorithm Overview:

Initialize variables range to represent the current covered range (initially 0), res to count the number of patches added, and i as the index to traverse nums (initially 0).
The loop continues until range covers the entire range of numbers up to n.
Looping and Patching:

If i is within the bounds of nums and the current element in nums (nums[i]) can extend the current range (nums[i] <= range + 1), update range by adding nums[i] to it and increment i.
If the current element in nums cannot extend the current range, add a patch (increment res) and extend the range by adding range + 1 to it.
### Output:
After the loop, res contains the minimum number of patches required to cover the range of numbers [1, n] inclusive.
