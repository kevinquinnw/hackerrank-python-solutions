# Finding the percentage
You have a record of n students. Each record contains the student's name, and their percent marks in Maths, Physics and Chemistry. The marks can be floating values. The user enters some integer n followed by the names and marks for n students. You are required to save the record in a dictionary data type. The user then enters a student's name. Output the average percentage marks obtained by that student, correct to two decimal places.

## Input Format 
The first line contains the integer n, the number of students. The next n lines contains the name and marks obtained by that student separated by a space. The final line contains the name of a particular student previously listed.

## Constraints 
2<= n <= 10 
0 <= Marks <= 100

## Output Format
Print one line: The average of the marks obtained by the particular student correct to 2 decimal places.

## Sample Input 0
3
Krishna 67 68 69
Arjun 70 98 63
Malika 52 56 60
Malika

## Sample Output 0
56.00

# Code 
```python 
def recScores(listOfStudents):
    line = list(input().split())
    avgScore = sum(map(float, line[1:])) / 3
    name = line[0]
    listOfStudents[name] = avgScore

n = int(input())
listOfStudents = dict()
for i in range(n):
    recScores(listOfStudents)
print('%.2f'% listOfStudents[input()])
```

# Explanation 
Marks for Malika are {52, 56, 60} whose average is {Marks/3} -> 56

## Part A - Setting up

First Line: Defining our function 

Second Line: This line will create our list and split the numbers where need be. 

Third Line: This is used to calculate the average of the marks, and give us back a floating number. 
