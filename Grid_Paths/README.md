# Algorithm

### Read Input:

Accept the size of the grid, denoted by n.
Read the grid, represented by a 2D vector of characters, where '.' indicates an empty cell and '*' denotes a trap.

### Initialize Dynamic Programming Table:

Create a 2D vector dp of size n x n to store the number of paths to reach each cell.
Set dp[0][0] to 1, as there's only one way to reach the upper-left cell.

### Fill the First Row and Column:

Traverse the first row and column of the grid:
If the current cell is not a trap, set dp[i][j] to the value of the cell on its left (if moving right) or above it (if moving down).
If the current cell is a trap, break the loop as no further paths are possible beyond that trap.

### Fill the Rest of the Grid:

Begin traversing the grid from the second row and column:
For each cell (i, j):
If the current cell is not a trap:
Calculate the number of paths to reach cell (i, j) as the sum of paths to reach the cell above it (i-1, j) and the cell to the left of it (i, j-1).
Store this sum in dp[i][j], taking modulo 10^9 + 7.
If the current cell is a trap, set dp[i][j] to 0, as it's not possible to reach a trap.

### Output Result:

Output dp[n-1][n-1], representing the number of paths to reach the lower-right cell while avoiding traps.
