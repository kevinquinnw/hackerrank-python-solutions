# Task 
You are given a function f(x) = x^2. You are also given K lists. The i^th list consists of N elements.

You have to pick one element from each list so that the value from the equation below is maximized:

S = (f(x1) + f(x2) + ... + f(xk) %M

X denotes the element picked from the i^th list. Find the maximized value Smax obtained.

% denotes the modulo operator.

##Note 
You need to take exactly one element from each list, not necessarily the largest element. You add the squares of the chosen elements and perform the modulo operation. The maximum value that you can obtain, will be the answer to the problem.

# Code 
```python
import itertools 

(Kevin, Nick) = map(int, input().strip().split(' '))

List = list()
for i in range(Kevin): 
    l = list(map(int, input().strip().split(' ')))
    j = l[0]
    List.append(l[1:])
    assert len(List[i]) == j 

S_max = 0
L_max = None

for l in itertools.product(*List):
    s = sum([x**2 for x in l]) % Nick

    if s > S_max:
        S_max = s
        L_max = l

print(S_max)
```
