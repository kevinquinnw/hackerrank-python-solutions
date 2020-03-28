# Task 
This tool computes the cartesian product of input iterables. It is equivalent to nested for-loops.
- For example, product(A, B) returns the same as ((x,y) for x in A for y in B).
# Code 
```python 
from itertools import product
# Enter your code here. Read input from STDIN. Print output to STDOUT


a = list(map(int, input().split()))
b = list(map(int, input().split()))
print(*list(product(a,b)))
```
