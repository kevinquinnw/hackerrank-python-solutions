# Task 
You are given a string s.
Your task is to find out if the string s contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

# Code 
``` python
if __name__ == '__main__':
    s = input()
    print(any([char.isalnum() for char in s]))
    print(any([char.isalpha() for char in s]))
    print(any([char.isdigit() for char in s]))
    print(any([char.islower() for char in s]))
    print(any([char.isupper() for char in s]))
```

# Keywords

## isalnum()
The isalnum() method returns True if all characters in the string are alphanumeric (either alphabets or numbers). If not, it returns False.

## isalpha()
The isalpha() method returns True if all characters in the string are alphabets. If not, it returns False.

## isdigit()
The isdigit() method returns True if all characters in a string are digits. If not, it returns False.

## islower()
The islower() method returns True if all alphabets in a string are lowercase alphabets. If the string contains at least one uppercase alphabet, it returns False.

## isupper()
The string isupper() method returns whether or not all characters in a string are uppercased or not.
