# Algorithm
### Input Reading:

Read the number of boys n.
Read the dancing skills of each boy into the vector boys.
Read the number of girls m.
Read the dancing skills of each girl into the vector girls.
### Sorting:

Sort both boys and girls vectors in non-decreasing order of dancing skills.
### Finding Pairs:

Initialize a variable pairs to 0 to keep track of the number of valid pairs.
Initialize two pointers i and j to 0, which will be used to traverse the boys and girls vectors, respectively.
### Pairing Process:

While i is less than the number of boys n and j is less than the number of girls m, do the following:
Check if the absolute difference between the dancing skills of boys[i] and girls[j] is at most one. If so, increment pairs by 1, and move both i and j pointers to the next elements in their respective vectors.
If the dancing skill of the current boy boys[i] is less than the dancing skill of the current girl girls[j], increment i to move to the next boy.
If the dancing skill of the current girl girls[j] is less than the dancing skill of the current boy boys[i], increment j to move to the next girl.
### Output:

Print the value of pairs, which represents the largest possible number of pairs that can be formed with the given conditions.
