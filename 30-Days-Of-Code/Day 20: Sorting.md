# Task 
- Array is sorted in numSwaps swaps.
  - where numSwaps is the number of swaps that took place.
- First Element: firstElement
  - where firstElement is the first element in the sorted array.
- Last Element: lastElement
  - where lastElement is the last element in the sorted array.
# Code 
```python 
#!/bin/python3

import sys

n = int(input().strip())
a = list(map(int, input().strip().split(' ')))
# Write Your Code Here
numSwaps = 0
for i in range(n):
    for j in range(n-1):
        if(a[j] > a[j+1]):
            numSwaps+=1
            a[j], a[j+1] = a[j+1], a[j]
    if(numSwaps is 0):
        break
print("Array is sorted in " + str(numSwaps) + " swaps.")
print("First Element: " + str(a[0]))
print("Last Element: " + str(a[n-1]))
```
