# Task
You are given a string. Split the string on a " " (space) delimiter and join using a - hyphen.

# Code 
```python
def split_and_join(line):
    # write your code here
    return "-".join(line.split())
if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)
```

# Keywords 

## split() 
splits a string into a list 
## join ()
a string method which returns a string concatenated with the elements of an iterable.
