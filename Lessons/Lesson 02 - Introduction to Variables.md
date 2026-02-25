# Lesson 02 - Introduction to Variables

## Overview

This lesson introduces variables, common Python data types, and how to store, access, and modify values in a program.

## Datatypes

Datatypes define the kind of value a variable stores, such as text, numbers, or true/false values.

* `str`, `int`, `float`, `bool`: Built-in Python data types.
* The datatype determines what kind of data the variable can hold.
* Different datatypes behave differently when used in operations.

```python
# Examples of different datatypes
text_value = "Hello"
whole_number = 10
decimal_number = 3.14
boolean_value = True
```

### Strings (`str`)

A string stores text and must be enclosed in quotation marks.

* `"Hello"`: Text wrapped in quotes.
* `str`: The datatype name for strings.
* Quotes `""` or `''`: Required to define a string.

```python
# Create a string variable
message = "Hello World"
```

### Numbers

Numbers store numeric values and can be whole numbers or decimals.

* `int`: Whole numbers without decimals.
* `float`: Numbers with decimal points.
* Numbers are written without quotation marks.

```python
# Create number variables
whole_number = 5
decimal_number = 2.5
```

#### Integers (`int`)

Integers are whole numbers without decimal points.

* `10`: A whole number.
* No quotes: Indicates it is a number, not text.
* Can be positive or negative.

```python
# Create an integer variable
age = 16
```

#### Decimals (`float`)

Floats are numbers that contain decimal points.

* `3.14`: A decimal number.
* Decimal point `.`: Makes it a float.
* Used for more precise numeric values.

```python
# Create a float variable
price = 9.99
```

### Booleans (`bool`)

Booleans store either `True` or `False`.

* `True`: Represents a true condition.
* `False`: Represents a false condition.
* No quotes: They are special keywords.

```python
# Create boolean variables
is_student = True
has_passed = False
```

## Initializing a Variable

Initializing a variable means creating it and giving it a value.

* `=`: The assignment operator.
* `score`: The variable name.
* `100`: The value being stored.

```python
# Initialize a variable
score = 100
```

## Accessing a Variable

Accessing a variable means using its stored value.

* `score`: The variable name.
* `print(score)`: Displays the stored value.
* No quotes around `score`: Refers to the variable, not text.

```python
# Access and display a variable's value
score = 100
print(score)
```

## Changing a Variable

You can change a variable by assigning it a new value.

* `score = 100`: Original value.
* `score = 90`: New value replaces the old one.
* The most recent assignment is the value stored.

```python
# Change the value of a variable
score = 100
score = 90
print(score)
```

## Example - Basic Use

This example creates a variable and prints its value to the console.

```python
# Create a variable and assign a value
name = "Alice"

# Print the value stored in the variable
print(name)
```

## Example - Print a Variable's Type

This example uses the `type()` function to display the datatype of a variable.

```python
# Create variables with different datatypes
name = "Alice"
age = 15

# Print the type of each variable
print(type(name))
print(type(age))
```

## Example - Assigning a Variable with an Expression

This example assigns a variable the result of a mathematical expression.

```python
# Assign a variable using an expression
length = 5
width = 3

# Calculate the area
area = length * width

# Print the result
print(area)
```

## Example - Printing Variable Values

This example prints multiple variable values in a single statement.

```python
# Create variables
first_name = "Alice"
last_name = "Smith"

# Print both variables
print(first_name, last_name)
```

## Example - Adding 2 Variables Together

This example adds two number variables and prints the result.

```python
# Create two number variables
num1 = 10
num2 = 5

# Add the two variables together
total = num1 + num2

# Print the result
print(total)
```
