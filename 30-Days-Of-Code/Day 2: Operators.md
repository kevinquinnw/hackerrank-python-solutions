# Task 
Given the meal price (base cost of a meal), tip percent (the percentage of the meal price being added as tip), and tax percent (the percentage of the meal price being added as tax) for a meal, find and print the meal's total cost.
Note: Be sure to use precise values for your calculations, or you may end up with an incorrectly rounded result!

# Code 
```python
if __name__ == '__main__':
    meal_cost = float(input())
    tip_percent = int(input())
    tax_percent = int(input())
    tip_amount = meal_cost * tip_percent / 100 
    tax_amount = meal_cost * tax_percent / 100
    total_cost = round(meal_cost + tip_amount + tax_amount)

    print(int(total_cost))
```

