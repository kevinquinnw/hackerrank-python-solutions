# Task 
Given an integer, n, and n space-separated integers as input, create a tuple, t, of those n integers. Then compute and print the result of hash(t).
Note: hash(t) is one of the functions in the __builtins__ module, so it need not be imported.

## Input Format
The first line contains an integer, , denoting the number of elements in the tuple.
The second line contains  space-separated integers describing the elements in tuple .

## Output Format
Print the result of hash(t).

## Sample Input 0
2
1 2

## Sample Output 0
3713081631934410656

```python 
n = int(input())
print(hash(tuple(map(int, input().split()))))
```

## hash()
Hash values are just integers which are used to compare dictionary keys during a dictionary lookup quickly.

## tuple() 
Tuples are sequences, just like lists. The differences between tuples and lists are, the tuples cannot be changed unlike lists and tuples use parentheses, whereas lists use square brackets.
