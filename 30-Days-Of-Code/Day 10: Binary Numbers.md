# Task 
Given a base-10 integer, n, convert it to binary (base-2). Then find and print the base-10 integer denoting the maximum number of consecutive 1's in n's binary representation.

# Code 
```python 
if __name__ == '__main__':
    n = int(input())
    consec_ones_count = 0
    one_count = 0

    while n != 0:
        fact = n // 2
        remain = n - 2 * fact
        n = fact
        if remain == 1:
            one_count += 1
            consec_ones_count = max(consec_ones_count, one_count)
        else:
            one_count = 0

    print(consec_ones_count)

```
