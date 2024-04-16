# Algorithm

### Input:
Take the size of the grid n as input.
### Input Grid:
Input the elements of the nxn grid, where 0 represents white squares and 1 represents black squares.
Count Subgrids:
Initialize count to 0.
Iterate through each cell (i, j) in the grid:
If the cell (i, j) is black (grid[i][j] == 1), iterate through all cells (k, l) below and to the right of (i, j):
If all four corners of the subgrid defined by (i, j) and (k, l) are black (grid[i][j], grid[i][l], grid[k][j], grid[k][l] are all 1), increment count.
### Output:
Print the value of count as the number of subgrids with all black corners.


This algorithm checks each cell of the grid. If a black cell is found, it looks for all possible subgrids with that cell as the top-left corner and counts those where all four corners are black.





