# Lesson 05 - Python Math

## Overview

This lesson introduces basic mathematical operations in Python, including addition, subtraction, multiplication, and division.

## Addition

Addition combines two numeric values using the `+` operator.

* `+`: The addition operator.
* `num1` and `num2`: Variables storing numbers.
* The result of `num1 + num2` is a new numeric value.

```python
# Create two number variables
num1 = 5
num2 = 3

# Add the two numbers
result = num1 + num2
```

## Subtraction

Subtraction finds the difference between two numbers using the `-` operator.

* `-`: The subtraction operator.
* The first number: The value being reduced.
* The second number: The value being subtracted.

```python
# Create two number variables
num1 = 10
num2 = 4

# Subtract the second number from the first
result = num1 - num2
```

## Multiplication

Multiplication calculates the product of two numbers using the `*` operator.

* `*`: The multiplication operator.
* Both values must be numeric.
* The result is the product of the two numbers.

```python
# Create two number variables
num1 = 6
num2 = 7

# Multiply the two numbers
result = num1 * num2
```

## Division

Division splits one number by another using the `/` operator.

* `/`: The division operator.
* The first number: The dividend.
* The second number: The divisor.
* Division in Python returns a float (decimal).

```python
# Create two number variables
num1 = 10
num2 = 2

# Divide the first number by the second
result = num1 / num2
```

## Example - Basic Use

This example performs multiple math operations and prints the results.

```python
# Create number variables
a = 8
b = 4

# Perform math operations
sum_result = a + b
difference_result = a - b
product_result = a * b
division_result = a / b

# Print each result
print(sum_result)
print(difference_result)
print(product_result)
print(division_result)
```

## Example - Order of Operations

This example demonstrates how Python follows the order of operations (BEDMAS).

```python
# Create a math expression
result = 2 + 3 * 4

# Print the result
print(result)

# Use parentheses to change the order
new_result = (2 + 3) * 4

# Print the new result
print(new_result)
```
