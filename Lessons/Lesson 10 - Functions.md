# Lesson 10 - Functions

## Overview

This lesson introduces functions, which allow you to group code into reusable blocks and create input–output behavior in your programs.

## Functions as Reusable Code

Functions allow you to write code once and reuse it multiple times instead of repeating yourself.

* `def`: Keyword used to define a function.
* `greet`: The function name.
* `()`: Parentheses used to define and call functions.
* The function body runs each time the function is called.

```python
# Define a function
def greet():
    print("Hello!")

# Call the function multiple times
greet()
greet()
greet()
```

### Defining the Function Syntax

Functions are defined using the `def` keyword followed by a name and parentheses.

* `def`: Keyword that starts a function definition.
* `say_hello`: The function name.
* `()`: Parentheses required even if there are no parameters.
* Indented code: The block that runs when the function is called.

```python
# Define a simple function
def say_hello():
    print("Hello World")
```

### Calling the Function Syntax

Calling a function runs the code inside it.

* `say_hello`: The function name.
* `()`: Required to call (run) the function.
* Without parentheses, the function will not execute.

```python
# Define the function
def say_hello():
    print("Hello World")

# Call the function
say_hello()
```

## Functions as Input - Output Machines

Functions can accept inputs (parameters) and produce outputs using `return`.

* Parameters: Inputs defined inside the parentheses.
* Arguments: Values passed into the function when calling it.
* `return`: Sends a value back to where the function was called.

```python
# Define a function with input and output
def double(number):
    return number * 2

# Call the function and store the result
result = double(5)

print(result)
```

### Defining a Function with A Parameter

A parameter allows a function to receive data.

* `name`: A parameter inside the function definition.
* `print(f"...")`: Uses the parameter inside the function.
* The function can be reused with different values.

```python
# Define a function with a parameter
def greet(name):
    print(f"Hello {name}!")
```

### Parameters vs Arguments

Parameters are defined in the function. Arguments are the actual values passed in.

* `name`: The parameter.
* `"Alice"`: The argument.
* The argument replaces the parameter when the function runs.

```python
# Define the function with a parameter
def greet(name):
    print(f"Hello {name}!")

# Call the function with an argument
greet("Alice")
```

### Returning a Value with `return`

The `return` keyword sends a value back to where the function was called.

* `return`: Ends the function and sends a value back.
* The returned value can be stored in a variable.
* Code after `return` will not run.

```python
# Define a function that returns a value
def add(a, b):
    return a + b

# Store the returned value
result = add(3, 4)

print(result)
```

## Example - Reusable Code Through Function

This example shows how a function can be reused multiple times.

```python
# Define a reusable function
def greet():
    print("Welcome!")

# Call the function multiple times
greet()
greet()
greet()
```

## Example - Function With Only Inputs

This example uses parameters but does not return a value.

```python
# Define a function with a parameter
def greet(name):
    print(f"Hello {name}!")

# Call the function with different arguments
greet("Alice")
greet("Bob")
```

## Example - Function with Multiple Parameters

This example shows a function that accepts multiple inputs.

```python
# Define a function with two parameters
def add_numbers(num1, num2):
    print(num1 + num2)

# Call the function
add_numbers(5, 3)
```

## Example - Function With Only Return

This example returns a value without printing inside the function.

```python
# Define a function that returns a value
def get_number():
    return 10

# Store and print the returned value
value = get_number()
print(value)
```

## Example - Function with Parameters and Return

This example uses both parameters and `return`.

```python
# Define a function that multiplies two numbers
def multiply(a, b):
    return a * b

# Call the function and store the result
result = multiply(4, 5)

# Print the result
print(result)
```

## Example - Function Definitions Go Above Your Main Code

This example shows proper structure, where functions are defined before being called.

```python
# Define the function first
def greet(name):
    print(f"Hello {name}!")

# Main part of the program
user_name = input("Enter your name: ")
greet(user_name)
```
