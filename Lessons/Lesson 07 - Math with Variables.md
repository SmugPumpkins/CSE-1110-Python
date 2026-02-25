# Lesson 07 - Math with Variables

## Overview

This lesson introduces how to modify existing variables using mathematical operations, including both long form and shorthand assignment operators.

## Changing a Variable

You can update a variable by using its current value in a new assignment.

* `var = var + 9`: Long form reassignment using the variable’s current value.
* `var += 9`: Short form (augmented assignment) that does the same thing.
* The variable keeps its name but stores a new updated value.

```python
# Start with a variable
var = 10

# Change the variable using a new assignment
var = var + 5
```

### Adding to a Variable

You can increase a variable’s value using addition.

* `var = var + 9`: Takes the current value of `var` and adds 9.
* `var += 9`: Shorthand that adds 9 to `var`.
* Both lines produce the same result.

```python
# Long form addition
var = 10
var = var + 9

# Short form addition
var = 10
var += 9
```

### Subtracting from a Variable

You can decrease a variable’s value using subtraction.

* `var = var - 9`: Subtracts 9 from the current value.
* `var -= 9`: Shorthand that subtracts 9 from `var`.
* Both lines update the stored value.

```python
# Long form subtraction
var = 20
var = var - 9

# Short form subtraction
var = 20
var -= 9
```

### Multiplying a Variable

You can multiply a variable by a number and store the result back into the same variable.

* `var = var * 9`: Multiplies the current value by 9.
* `var *= 9`: Shorthand for multiplying and reassigning.
* Both lines update the variable’s value.

```python
# Long form multiplication
var = 3
var = var * 9

# Short form multiplication
var = 3
var *= 9
```

### Dividing a Variable

You can divide a variable and store the result back into it.

* `var = var / 9`: Divides the current value by 9.
* `var /= 9`: Shorthand for dividing and reassigning.
* Division using `/` results in a float.

```python
# Long form division
var = 18
var = var / 9

# Short form division
var = 18
var /= 9
```

## Example - Basic Usage

This example demonstrates updating a variable using different math operations.

```python
# Create a starting variable
score = 50

# Add 10 to the score
score += 10

# Subtract 5 from the score
score -= 5

# Multiply the score by 2
score *= 2

# Divide the score by 5
score /= 5

# Print the final result
print(score)
```
