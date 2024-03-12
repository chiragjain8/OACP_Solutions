# ALGORITHM

### Define MOD:
Define a constant MOD which is 10^9 + 7. This will be used to take the modulo of the result to prevent integer overflow.

### CountWays Function:

Initialize a vector dp of size n+1 with all elements initialized to 0. This vector will store the number of ways to obtain each sum.
Set dp[0] to 1, since there is one way to obtain a sum of 0 (by not throwing the dice at all).
Iterate from 1 to n:
For each value of i, iterate from 1 to 6 (since the dice can have outcomes from 1 to 6).
For each outcome j, if i - j is greater than or equal to 0, it means we can obtain the sum i by adding the outcome j to some previous sum. So, update dp[i] by adding dp[i - j] to it.
Finally, return dp[n], which represents the number of ways to obtain the sum n.


### Main Function:

Read the total number of sums from the input file.
Read each sum value from the input file and store them in a list sums.
For each sum in sums:
Call the CountWays function with the current sum value.
Print the result modulo MOD.

