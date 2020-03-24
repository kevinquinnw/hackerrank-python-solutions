# Arithmetic Operators 

Task
Read two integers from STDIN and print three lines where:

1. The first line contains the sum of the two numbers.
2. The second line contains the difference of the two numbers (first - second).
3. The third line contains the product of the two numbers.

Input Format

The first line contains the first integer, a. The second line contains the second integer, b.

Constraints

1<= a <= 10^10
1<= b <= 10^10

Output Format

Print the three lines as explained above.

Sample Input 

3, 2

Sample Output 

5, 1, 6

# Code 

  a, b = int(input()), int(input())
  print = ((a + b), (a - b), (a * b), sep ='\n')


# Explanation 

1st Line: Setting up the function. 

2nd Line: Printing the three values. The separator parameter known as 'sep' between the arguments to print() function is space by default.

This can be modified and can be made to any character, integer, or string per our choice. It is found only in Python 3.X or later.
