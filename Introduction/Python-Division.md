# Python-Division
Read two integers and print two lines. The first line should contain integer division,  a// b. The second line should contain float division, a / b .

You don't need to perform any rounding or formatting operations.

Input Format

The first line contains the first integer, a. The second line contains the second integer, b.

Output Format

Print the two lines as described above.

Sample Input 
4, 3 

Sample Output 
1, 1.333333333333


# Code 
``` python
a, b = int(input()), int(input())
print((a//b), (a/b), sep='\n')
```

# Explanation
1st Line: Setting up a and b 
2nd Line: a // b means it will round the final answer resulting in an integer (a number w/ no decimal). a / b means the it will result in a floating number. Floating division is performed if either operand (or both) is floating-point.

