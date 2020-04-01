# Task 
Given an array, A, of N integers, print A's elements in reverse order as a single line of space-separated numbers.

# Code 
```python 
import sys



if __name__ == '__main__':
    n = int(input().strip())

    arr = [int(arr_data) for arr_data in input().strip().split(' ')]

    arr.reverse()

    arr_string = ' '.join(str(e) for e in arr)

    print(arr_string)
```
