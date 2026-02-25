# Lesson 03 - User Input

## Overview

This lesson introduces how to collect input from a user using the `input()` function and store that input in variables.

## Syntax

The `input()` function pauses the program and waits for the user to type something.

* `input()`: A built-in Python function used to collect user input.
* `"Enter your name: "`: A prompt shown to the user.
* Parentheses `()`: Required to call the function.
* The function always returns a string.

```python
# Prompt the user for input
input("Enter your name: ")
```

### Optional - `print()` then `input()`

You can display a message first using `print()`, then call `input()` on the next line.

* `print()`: Displays a message in the console.
* `input()`: Waits for the user to type something.
* This separates the message from the input line.

```python
# Display a message first
print("Enter your name:")

# Then collect user input
input()
```

## Storing Input to a Variable

To use the input later, store it in a variable.

* `name`: The variable that stores the input.
* `=`: The assignment operator.
* `input()`: Collects the user's input.
* The stored value is always a string.

```python
# Store user input in a variable
name = input("Enter your name: ")
```

## Example - Basic Use

This example asks the user for their name and then prints a greeting.

```python
# Ask the user for their name and store it
name = input("Enter your name: ")

# Print a greeting using the stored value
print("Hello", name)
```

## Example - Print Type Of an Input Variable (always a string)

This example shows that input is always stored as a string.

```python
# Ask the user for their age
age = input("Enter your age: ")

# Print the value entered
print(age)

# Print the datatype of the input
print(type(age))
```
