# Task 
You are given two classes, Person and Student, where Person is the base class and Student is the derived class. Completed code for Person and a declaration for Student are provided for you in the editor. Observe that Student inherits all the properties of Person.

## Complete the Student class by writing the following:

### A Student class constructor, which has  parameters:
1. A string, firstName.
2. A string, lastName.
3. An integer, id.
4. An integer array (or vector) of test scores, scores.
5. A char calculate() method that calculates a Student object's average and returns the grade character representative of their calculated average:

## Grading Scale
|Letter |  Average(a)   |
| ----- |:-------------:|
| O     | 90<= a <= 100 |
| E     | 80<= a <= 90 |
| A     | 70<= a <= 80 | 
| P     | 55<= a <= 70 |
| D     | 40<= a <= 55 | 
| T     |  a < 40 | 

# Code 
```python 
class Person:
	def __init__(self, firstName, lastName, idNumber):
		self.firstName = firstName
		self.lastName = lastName
		self.idNumber = idNumber
	def printPerson(self):
		print("Name:", self.lastName + ",", self.firstName)
		print("ID:", self.idNumber)

class Student(Person):
    def __init__(self, firstName, lastName, idNumber, scores):
        super().__init__(firstName, lastName, idNumber)
        self.scores = scores

    def calculate(self):
        avg = 0.0
        for score in self.scores:
            avg += score

        avg = avg/len(self.scores)
        if avg < 40:
            return 'T'
        elif avg < 55:
            return 'D'
        elif avg < 70:
            return 'P'
        elif avg < 80:
            return 'A'
        elif avg < 90:
            return 'E'
        else:
            return 'O'

line = input().split()
firstName = line[0]
lastName = line[1]
idNum = line[2]
numScores = int(input()) # not needed for Python
scores = list( map(int, input().split()) )
s = Student(firstName, lastName, idNum, scores)
s.printPerson()
print("Grade:", s.calculate())
```
