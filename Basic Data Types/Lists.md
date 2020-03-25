# Task 
Initialize your list and read in the value of  followed by  lines of commands where each command will be of the  types listed above. Iterate through each command in order and perform the corresponding operation on your list.

## Input Format
The first line contains an integer, , denoting the number of commands.
Each line  of the  subsequent lines contains one of the commands described above.

## Constraints
The elements added to the list must be integers.

## Output Format
For each command of type print, print the list on a new line.

## Sample Input 0
12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print

## Sample Output 0
[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]

``` python
def handle(result):
    inpu = input().split()
    command = inpu[0]
    values = inpu[1:]
    if command == 'print':
        print(result)
    else:
        execute = 'result.' + command + "(" + ",".join(values) + ")"
        eval(execute)

    
result =[]
for i in range (int(input())):
    handle(result)
```
# Explanation
