# Algorithm
### Input Handling: 
The program takes two inputs from the user: the non-negative integer number (num) and the number of digits to remove (k).

### Stack-based Approach:

The algorithm uses a stack to keep track of digits in a non-decreasing order.
It iterates through each digit in the input number.
For each digit, it compares it with the top of the stack (if the stack is not empty) to ensure that the digits in the stack are in non-decreasing order. If the current digit is smaller than the top of the stack, it removes the top of the stack and decrements k until the condition is satisfied.
After processing all digits, the algorithm removes any remaining digits from the stack to ensure that exactly k digits are removed.
Constructing the Result:

After processing all digits and removing k digits, the algorithm constructs the resulting number by popping digits from the stack and appending them to the result string.
Since digits are popped from the stack in reverse order (due to the stack's LIFO nature), the result string is initially in reverse order.
The algorithm then removes leading zeros from the result string to ensure that the result is a valid non-zero number.
### Output: 
The program outputs the smallest possible integer obtained after removing k digits from the input number.

This algorithm ensures that the resulting number is the smallest possible integer by strategically removing digits while maintaining the non-decreasing order.





