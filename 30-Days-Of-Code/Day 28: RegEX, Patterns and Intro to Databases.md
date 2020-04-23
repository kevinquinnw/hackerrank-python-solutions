# Task 
Consider a database table, Emails, which has the attributes First Name and Email ID. Given N rows of data simulating the Emails table, print an alphabetically-ordered list of people whose email address ends in @gmail.com.

# Code 
```python 
#!/bin/python3
import sys 
import re 


N = int(input().strip())
names = []
for a0 in range(N):
    first_name, email = input().strip().split(' ')
    first_name, email = [str(first_name), str(email)]
    match = re.search(r'[\w.-]@gmail.com', email)

    if match: 
        names.append(first_name)

names.sort()
for name in names: 
    print (name)
```
