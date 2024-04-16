# Algorithm

### Input:
Take the number of elements n as input.
### Input Elements:
Input n integers into the vector nums.
Calculate Hamming Distance:
Initialize ans to 0.
Iterate from i = 0 to i = 30 (31 bits for integers).
For each i, count the number of elements in nums where the i-th bit is set (cnt1).
Add cnt1 * (n - cnt1) to ans, where n is the size of nums.
### Output:
Print the calculated ans as the total Hamming distance.


This algorithm calculates the Hamming distance between all pairs of integers in the input array nums. The Hamming distance between two integers is the number of positions at which the corresponding bits are different in the binary representation of the integers.





