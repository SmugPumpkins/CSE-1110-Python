# Lesson 06 - Type Casting

## Overview

This lesson introduces type casting, which is the process of converting a value from one datatype to another in Python.

## `str()`

The `str()` function converts a value into a string.

* `str()`: A built-in function used to convert a value to text.
* `number`: A variable storing a numeric value.
* The result becomes a string version of the original value.

```python id="b7z4km"
# Create a number variable
number = 25

# Convert the number to a string
text_value = str(number)
```

## `int()`

The `int()` function converts a value into an integer.

* `int()`: A built-in function used to convert a value to a whole number.
* `"10"`: A numeric string that can be converted.
* The string must contain only digits to convert successfully.

```python id="m2x8qv"
# Create a string variable
number_text = "10"

# Convert the string to an integer
number = int(number_text)
```

## `float()`

The `float()` function converts a value into a decimal number.

* `float()`: A built-in function used to convert a value to a float.
* `"3.14"`: A string containing a decimal number.
* The string must represent a valid numeric value.

```python id="q9w5lt"
# Create a string variable
decimal_text = "3.14"

# Convert the string to a float
decimal_number = float(decimal_text)
```

## Example - Basic Usage

This example converts values between different datatypes and prints the results.

```python id="y6nc2p"
# Create original variables
age_text = "16"
price_number = 9.99

# Convert string to integer
age_number = int(age_text)

# Convert float to string
price_text = str(price_number)

# Print converted values
print(age_number)
print(price_text)
```

## Example - ValueError From Data That Can't Convert

This example shows what happens when you try to convert invalid data.

```python id="k4v8st"
# Create a string that cannot be converted to an integer
invalid_number = "hello"

# Attempt to convert the string to an integer
# This will cause a ValueError
number = int(invalid_number)

# This line will not run because the program stops at the error
print(number)
```

## Example - User Input to Number for Math

This example converts user input into numbers so it can be used in math operations.

```python id="z8h1rx"
# Ask the user for two numbers
num1 = input("Enter the first number: ")
num2 = input("Enter the second number: ")

# Convert input strings to integers
num1 = int(num1)
num2 = int(num2)

# Add the numbers together
total = num1 + num2

# Print the result
print("The total is:", total)
```
