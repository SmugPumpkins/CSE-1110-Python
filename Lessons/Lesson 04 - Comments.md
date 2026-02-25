# Lesson 04 - Comments

## Overview

This lesson introduces comments in Python, which are used to explain code and make programs easier to understand without affecting how they run.

## Single Line Comments

Single line comments begin with the `#` symbol and continue to the end of the line.

* `#`: The symbol that starts a comment.
* Anything after `#`: Ignored by Python.
* Used to explain what a line of code does.

```python
# This is a single line comment
print("Hello World")  # This comment explains the print statement
```

## Multi Line Comments

Python does not have a special multi-line comment symbol, but triple quotes are often used to write comments that span multiple lines.

* `"""` or `'''`: Triple quotes used to write multi-line strings.
* Text inside triple quotes: Not executed when not assigned to a variable.
* Often used for longer explanations.

```python
"""
This is a multi-line comment.
It can span multiple lines.
Python will ignore it if it is not assigned to a variable.
"""
print("Hello World")
```

## Example - Basic Use

This example demonstrates using comments to explain different parts of a simple program.

```python
# This program greets the user

# Ask the user for their name
name = input("Enter your name: ")

# Print a greeting using the name provided
print("Hello", name)
```
