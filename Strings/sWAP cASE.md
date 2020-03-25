# Task 
You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.

## Sample Input 0
HackerRank.com presents "Pythonist 2".

## Sample Output 0
hACKERrANK.COM PRESENTS "pYTHONIST 2".

# Code 
```python 
def swap_case(s):
    return s.swapcase()

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```

# Key Terms 

## swapcase()
This method returns the string where all uppercase characters are converted to lowercase, and lowercase characters are converted to uppercase
