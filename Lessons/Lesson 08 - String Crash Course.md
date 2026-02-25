# Lesson 08 - String Crash Course

## Overview

This lesson introduces essential string operations in Python, including combining strings, formatting output, and modifying string content.

## String Concatenation

String concatenation combines multiple strings using the `+` operator.

* `"Hello"`: A string literal.
* `+`: The concatenation operator for strings.
* `" "`: A string containing a space.
* `"World"`: Another string literal.
* All parts must be strings.

```python
# Combine multiple strings into one
message = "Hello" + " " + "World"

print(message)
```

## Strings With Commas

You can print multiple strings separated by commas inside `print()`.

* `print()`: Built-in function used to display output.
* Commas `,`: Separate multiple values.
* Python automatically adds a space between comma-separated values.

```python
# Print multiple strings separated by commas
print("Hello", "World")
```

## Formatted Strings (f strings)

Formatted strings (f strings) allow you to insert variables directly into a string and are the best and cleanest way to format strings.

* `f" "`: The `f` before the quotes creates a formatted string.
* `{name}`: Curly braces insert the variable’s value.
* Variables inside `{}` are replaced with their stored values.

```python
# Create variables
name = "Alice"
age = 16

# Use an f string to insert variables
message = f"My name is {name} and I am {age} years old."

print(message)
```

## Trim Whitespace

The `.strip()` method removes whitespace from the beginning and end of a string.

* `.strip()`: A string method that removes leading and trailing spaces.
* Does not change the original string unless reassigned.
* Useful for cleaning user input.

```python
# Create a string with extra spaces
text = "   Hello World   "

# Remove whitespace from both ends
clean_text = text.strip()

print(clean_text)
```

## Lowercase

The `.lower()` method converts all characters in a string to lowercase.

* `.lower()`: A string method that returns a lowercase version.
* Does not modify the original string unless reassigned.
* Useful for standardizing user input.

```python
# Create a string with uppercase letters
text = "HELLO WORLD"

# Convert the string to lowercase
lower_text = text.lower()

print(lower_text)
```

## Example - Basic Usage of Formatted Strings

This example demonstrates using f strings to create clean and readable output.

```python
# Create variables
first_name = "John"
last_name = "Smith"

# Combine variables using an f string
full_name = f"{first_name} {last_name}"

# Print the result
print(full_name)
```

## Example - Trimming Whitespace

This example removes extra spaces from user input.

```python
# Ask the user for their name
name = input("Enter your name: ")

# Remove extra spaces
clean_name = name.strip()

# Print the cleaned name
print(f"Hello {clean_name}!")
```

## Example - Lowercase

This example converts user input to lowercase.

```python
# Ask the user for their favorite color
color = input("Enter your favorite color: ")

# Convert to lowercase
color = color.lower()

# Print the result
print(f"Your favorite color is {color}.")
```

## Example - Putting it All Together

This example trims whitespace, converts input to lowercase, and uses an f string.

```python
# Ask the user for their name
name = input("Enter your name: ")

# Clean the input
name = name.strip().lower()

# Create a formatted message
message = f"Welcome, {name}!"

# Print the final message
print(message)
```
