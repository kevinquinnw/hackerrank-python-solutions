# Nested Lists
Given the names and grades for each student in a Physics class of  students, store them in a nested list and print the name(s) of any student(s) having the second lowest grade.

Note: If there are multiple students with the same grade, order their names alphabetically and print each name on a new line.

## Input Format
The first line contains an integer, n, the number of students.
The 2n subsequent lines describe each student over 2 lines; the first line contains a student's name, and the second line contains their grade.

## Constraints
There will always be one or more students having the second lowest grade.

## Output Format
Print the name(s) of any student(s) having the second lowest grade in Physics; if there are multiple students, order their names alphabetically and print each one on a new line.

## Sample Input 0
5
Harry
37.21
Berry
37.21
Tina
37.2
Akriti
41
Harsh
39

## Sample Output 0
Berry
Harry

# Code 
```python 
def secondLowestGrade(classList):
    secondLowestRank = sorted(set(_[1] for _ in classList))[1]
    result = sorted([_[0] for _ in classList if _[1] == secondLowestRank])
    return result 

numberOfStudents = int(input())
classList = []
for i in range(numberOfStudents):
    classList.append([str(input()), float(input())])
print ('\n'.join(secondLowestGrade(classList)))
```

# Explanation 

There are 5 students in this class whose names and grades are assembled to build the following list:

python students = [['Harry', 37.21], ['Berry', 37.21], ['Tina', 37.2], ['Akriti', 41], ['Harsh', 39]]

The lowest grade of 37.2 belongs to Tina. The second lowest grade of  belongs to 37.21 both Harry and Berry, so we order their names alphabetically and print each name on a new line.

## Part A - Setting up our list. 

First Line: Defining our function which is going to find the second lowest grade in the class list assigned to each name. 

Second Line: The sorted() function returns a stored list from the items in an iterable It will assort it in either an ascending or descending order. And we use set() parameter to take a single optional parameter. 

Third Line: Setting up result, creating a sorted function for the grades. 

Fourth Line: Return the result.

## Part B - Printing the Students

Fifth Line: Number of Students is what our input value is. 

Sixth Line: Accessing the list we created. 

Seventh Line: append() will add a new item to the end of the list. We use the string(their name), float(grade) for list format. 

Eigth Line: Print the result of the function we created in the first part. 


