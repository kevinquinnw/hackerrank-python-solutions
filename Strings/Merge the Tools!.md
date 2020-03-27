# Task 
Given s and k, print n/k lines where each line i denotes string u.
# Code 
```python 
from collections import OrderedDict

def merge_the_tools(string, k):
    # your code goes here
    for i in range(0, len(string), k):
        print(''.join(OrderedDict.fromkeys(string[i:i +k])))

```
