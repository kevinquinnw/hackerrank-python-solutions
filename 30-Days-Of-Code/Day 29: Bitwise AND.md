# Task 
Given set S ={1,2,3,...,N}. Find two integers, A and b (where A < B), from set S such that the value of A & B is the maximum possible and also less than a given integer, K. In this case, & represents the bitwise AND operator.

# Code 
```python
#!/bin/python3
import sys 


t = int(input().strip())
for a0 in range(t):
    n, k = input().strip().split(' ')
    n, k = [int(n), int(k)]
    print(k-1 if ((k-1) | k) <= n else k-2)
```
