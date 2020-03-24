# Write a Function 
We add a Leap Day on February 29, almost every four years. The leap day is an extra, or intercalary day and we add it to the shortest month of the year, February.
In the Gregorian calendar three criteria must be taken into account to identify leap years:

The year can be evenly divided by 4, is a leap year, unless:
The year can be evenly divided by 100, it is NOT a leap year, unless:
The year is also evenly divisible by 400. Then it is a leap year.
This means that in the Gregorian calendar, the years 2000 and 2400 are leap years, while 1800, 1900, 2100, 2200, 2300 and 2500 are NOT leap years.Source

Task
You are given the year, and you have to write a function to check if the year is leap or not.
Note that you have to complete the function and remaining code is given as template.

Input Format
Read y, the year that needs to be checked.

Constraints
1900 <= y <= 10^5

Output Format
Output is taken care of by the template. Your function must return a boolean value (True/False)

Sample Input 0
1990

Sample Output 0
False

# Code
``` python 

def is_leap(y):
    return y % 4 == 0 and (y % 100 != 0 or y % 400 ==)

year = int(input())
print(is_leap(year))

```

# Explanation 
1st Line: Defining what y (year) will be. 

== Equal-to Operator 
!= Not Equal-to Operator

2nd Line: Return y if divides by 4 with no remainder.  Use 'and' to add other conditions. Return y if doesn't divide by 100 with no remainder or return y if y divides by 400 with no remainder. 

3rd Line: Setting up year equation 

4th Line: print output. function(component) to check. 

1990 is not a multiple of 4 hence it is not a leap year. 
