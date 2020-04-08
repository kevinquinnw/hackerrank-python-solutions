# Task 
Complete the Difference class by writing the following:

- A class constructor that takes an array of integers as a parameter and saves it to the elements instance variable.
- A computeDifference method that finds the maximum absolute difference between any 2 numbers in N and stores it in the maximumDifference instance variable.

# Code 
```python 
class Difference:
    def __init__(self, a):
        self.__elements = a

    # Add your code here
    def computeDifference(self):
        lengthElem = len(self.__elements)
        max = 0
        for i in range(lengthElem):
            for j in range(lengthElem):
                value = abs(self.__elements[i] - self.__elements[j])
                if (max < value):
                    max = value
        self.maximumDifference = max    

# End of Difference class

_ = input()
a = [int(e) for e in input().split(' ')]

d = Difference(a)
d.computeDifference()

print(d.maximumDifference)
```
