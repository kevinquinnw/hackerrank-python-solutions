# Task 
You are given an integer, N. Your task is to print an alphabet rangoli of size N. (Rangoli is a form of Indian folk art based on creation of patterns.)

# Code 
```python 
def print_rangoli(size):
    alpha = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u',
             'v', 'w', 'x', 'y', 'z', '1']
    letter = alpha[size]
    if alpha[size - 1] == "a":
        print("a")
    else:
        # middle part
        first_part = ""
        for i in alpha:
            if i == letter:
                break
            else:
                first_part = first_part + "-" + i
        second_part = first_part.replace("-a-", "")
        first_part = first_part[::-1]
        parts = first_part + second_part
        # haut part
        lengthh = (len(parts) - 1) // 2
        haut_part = parts[0:1]
        first_lengthh = 4
        second_lengthh = len(parts) - 1
        for i in range(1, size):
            print(haut_part.center(len(parts), "-"))
            haut_part = parts[0:first_lengthh] + parts[second_lengthh:len(parts)]
            first_lengthh += 2
            second_lengthh -= 2

        print(parts)

        # bottom part
        if alpha[size - 1] == "b":
            for i in range(1, size):
                parts = parts.replace(parts[(len(first_part) - 2):(len(first_part) + 2)], "")
                parts = ("-" * 2) + parts + ("-")
                print(parts)
        else:
            for i in range(1, size):
                parts = parts.replace(parts[(len(first_part) - 2):(len(first_part) + 2)], "")
                parts = ("-" * 2) + parts + ("-" * 2)
                print(parts)

```
