Read an integer N.

Without using any string methods, try to print the following:
123...N

Note that "..." represents the values in between.

Input Format
The first line contains an integer .

Output Format
Output the answer as explained in the task.

Sample Input 0
3

Sample Output 0
123

# Code 
``` python 
for i in range(1, int(input()) + 1):
    print( i, end='')
```

# Explanation 
1st Line: Getting numbers 1, 2, 3. So 1, 1+1(2), 2+1(3).

2nd Line: Print i, instead of creating a new line between our numbers, we use the end parameter to print without a newline. You could use an '@' sign and it would become 1@2@3
