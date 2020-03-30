# Task 
Given a string, S, of length N that is indexed from 0 to N-1, print its even-indexed and odd-indexed characters as 2 space-separated strings on a single line.
# Code 
```python 
# Enter your code here. Read input from STDIN. Print output to STDOUT

N = int(input())

for i in range(0, N):
    S = input()

    for j in range(0, len(S)):
        if j % 2 == 0: 
            print(S[j], end = '')

    print(" ", end = '')

    for j in range(0, len(S)):
        if j % 2 != 0:
            print(S[j], end = '')
    

    print ("")
```
