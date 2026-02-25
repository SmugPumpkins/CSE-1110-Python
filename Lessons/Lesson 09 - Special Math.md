# Lesson 09 - Special Math

## Overview

This lesson introduces special math operators in Python, including exponents, floor division, and modulo division.

## Exponents `**`

The exponent operator raises a number to a power.

* `**`: The exponent operator.
* `base ** exponent`: Raises the base number to a power.
* `2 ** 3`: Means 2 × 2 × 2.

```python
# Raise a number to a power
result = 2 ** 3

print(result)
```

## Floor Division `//`

Floor division divides two numbers and rounds the result down to the nearest whole number.

* `//`: The floor division operator.
* `7 // 2`: Divides 7 by 2 and removes the decimal.
* Always rounds down to the nearest whole number.

```python
# Perform floor division
result = 7 // 2

print(result)
```

## Modulo Division (Getting the Remainder) `%`

The modulo operator returns the remainder after division.

* `%`: The modulo operator.
* `7 % 2`: Divides 7 by 2 and returns the remainder.
* Useful for checking even or odd numbers.

```python
# Get the remainder of a division
result = 7 % 2

print(result)
```

## Example - Basic Usage

This example demonstrates all three special math operators.

```python
# Perform special math operations
power_result = 3 ** 2
floor_result = 9 // 4
remainder_result = 9 % 4

# Print the results
print(power_result)
print(floor_result)
print(remainder_result)
```

## Example - When You Might Need Floor Division

This example shows how floor division can determine how many full groups can be made.

```python
# Total number of students
students = 23

# Number of students per group
group_size = 5

# Determine how many full groups can be formed
full_groups = students // group_size

# Print the result
print(f"Number of full groups: {full_groups}")
```

## Example - When You Might Need Modulo Division

This example uses modulo to check whether a number is even or odd.

```python
# Get a number from the user
number = int(input("Enter a number: "))

# Check if the number is even or odd
if number % 2 == 0:
    print("The number is even.")
else:
    print("The number is odd.")
```
