# List-Comprehensions
Let's learn about list comprehensions! You are given three integers X, Y and Z representing the dimensions of a cuboid along with an integer N. You have to print a list of all possible coordinates given by (i,j,k) on a 3D grid where the sum of i + j + k  is not equal to N. Here, 0 <= i <= X; 0 <= j <= Y; 0<= k <= Z

Input Format
Four integers X, Y , Z and N each on four separate lines, respectively.

Constraints
Print the list in lexicographic increasing order.

Sample Input 0
1
1
1
2

Sample Output 0
[[0, 0, 0], [0, 0, 1], [0, 1, 0], [1, 0, 0], [1, 1, 1]]

# Concept
You have already used lists in previous hacks. List comprehensions are an elegant way to build a list without having to use different for loops to append values one by one. This example might help.

# Code 
``` python 
x, y ,z ,n = [int(input()) for _ in range(4)]
answerList = [[i, j, k] for i in range(x + 1) for j in range(y + 1) for k in range(z + 1) if i + j + k != n]
print(answerList)
```

# Explanation 
1st Line: Asking for range for variables. We use '_' so we don't need to use the iterator or another variable. We use 4 for the range because we want to do our task 4 times. 

2nd Line: Creating our list, we use our coordinates of the cuboid to see what the range will be for our three dimensions. We then wrap it up by saying that this all has to happen if the sum of the three coordinates doesn't equal n. (One of our constraints)

3rd Line: Print 
