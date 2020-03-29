# Task 
Given an integer, n, print its first 10 multiples. Each multiple n X i (where i) should be printed on a new line in the form: n X i = result.

# Code 
```python 
import sys

if __name__ == '__main__':
    n = int(input().strip())
    for i in range(1, 11):
        answer = i*n
        print(str(n) + " x " + str(i) + " = " + str(answer))
```

## OR 

```python 
import sys

if __name__ == '__main__':
    n = int(input().strip())
    for i in range(1, 11):
        print(str(n) + " x " + str(i) + " = " + str(n*i))
```
