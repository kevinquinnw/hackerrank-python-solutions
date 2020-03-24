# Find the Runner-Up Score
Given the participants' score sheet for your University Sports Day, you are required to find the runner-up score. You are given  scores. Store them in a list and find the score of the runner-up.

## Input 
5 2 3 6 6 5 

## Output 
5

# Code 
``` python 
n = int(input())
arr = list(map(int, input().split()))
print(max([x for x in arr if x != max(arr)]))
```

# Explanation 
The maximum score is 6, second maximum is 5. Hence we print 5 as the runner-up score. 

First Line: Setting up n, fetch the input. input() will cast the the input as a string.

Second Line: Creating an array. We use a list (that will convert this to a list) and nest a map as that takes two arguments.
    a. method to apply
    b. data to apply to it
    
split() is used to create a Python list out of a string. 

Third Line: Print the highest number that isn't the maximum in the array. 


