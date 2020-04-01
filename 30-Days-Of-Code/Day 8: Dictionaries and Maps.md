# Task 
Given n names and phone numbers, assemble a phone book that maps friends' names to their respective phone numbers. You will then be given an unknown number of names to query your phone book for. For each name queried, print the associated entry from your phone book on a new line in the form name=phoneNumber; if an entry for name is not found, print Not found instead.
# Code 
```python 
phonebook = {}
num = int(input())
for i in range(0, num):
    data = str(input()).split(" ")
    name = data[0]
    phone = int(data[1])
    phonebook[name] = phone

for i in range(0, num): 
    name = input()
    if name in phonebook:
        print(name + "=" + str(phonebook[name]))
    else:
        print("Not found")
```

This code gave me a runtime error, and I did not get maximum points. Below is my other solution, that got max points.

```python
def getphonebook(n):
    phonebook = {}
    for x in range(n):
        line = input().strip().split(' ')
        name = line[0]
        number = line[1]
        phonebook[name]=number
    return phonebook

if __name__ == '__main__':
    numberofentries = int(input())
    phonebook = getphonebook(numberofentries)

    while True:
        try:
            name = input()
            if name in phonebook.keys():
                print(name,'=',phonebook[name],sep='')
            else:
                print('Not found')
        except EOFError as eof:
            break
```
