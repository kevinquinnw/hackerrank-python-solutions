#Python If-Else

Given an integer, n, perform the following conditional actions:

If n is odd, print Weird
If n is even and in the inclusive range of  to , print Not Weird
If n is even and in the inclusive range of  to , print Weird
If n is even and greater than , print Not Weird
Input Format

A single line containing a positive integer, n .

Constraints
1 <= n <= 100

Output Format
Print Weird if the number is weird; otherwise, print Not Weird.

# Code 

    n = int(input())
    if n % 2 == 1:
        print("Weird")
    elif n % 2 == 0 and 2 <= n <= 5:
        print("Not Weird")
    elif n % 2 == 0 and 6 <= n <=20:
        print("Weird")
    else:
        print("Not Weird")
        
# Explanation 
  
  Line 1: Declaring what n will equal. Asks for an input which is an integer.
  
  Line 2: Use if statement to say if n is odd, print "Weird". We use n % 2 == 1 to check that. 
  This call basically checks the remainder of a number after 2 has been put into it as many times as possible. 
  To understand how this works:
  
  7 % 2 == 1 yields true(or 1), 8 % 2 == 1 yields false(or 0). Use n % 2 == 1 and rely on the compiler to do the work.  
  
  Line 4: Instead of using multiple if's we use elif to see if one if condition satisfies the code. 
  If you only used if conditions your code would go and check all the if conditions.
  
  n % 2 == 0 --> if it's even and in between an inclusive range of 2 to 5, print not weird. 
  We use the and operator to connect the conditions. We use <= operators to say if less than or equal to. 
  
  Line 6: Same as above. But we use 6 to 20 in the inclusive range. 
  
  Line 8: Use else statement to say if all other conditions are unmet, print "Not Weird". 
  
 
        


