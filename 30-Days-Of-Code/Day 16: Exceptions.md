# Task 
Read a string, S, and print its integer value; if S cannot be converted to an integer, print Bad String.

# Code 
```python 
#!/bin/python3

import sys


S = input().strip()
try:
    t = int(S)
    print(S)
except BaseException as error:
    print('Bad String')
```
