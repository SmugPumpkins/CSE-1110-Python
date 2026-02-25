# Lesson 11 - Using Multiple Python Files

## Overview

This lesson explains how to organize programs across multiple Python files using imports. You will learn how namespaces work, different import styles, and how to prevent code from running when a file is imported.

## What is a "namespace"

A namespace is a container that holds names like variables and functions and keeps them organized. When you import a file, its contents live inside that file’s namespace unless you specifically import them into your own. This prevents naming conflicts and helps structure larger programs.

---

## Import A Whole File

Importing a whole file allows you to access its functions using dot notation.

* `helpers.py` defines reusable math functions.
* No top-level code runs automatically.
* Functions are available inside the `helpers` namespace.

```python
# helpers.py

# Define basic math functions
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b
```

* `import helpers` imports the entire file.
* `helpers` becomes the namespace.
* Functions are accessed using dot notation.

```python
# main.py

# Import the entire helpers file
import helpers

# Use dot notation to access functions
print(helpers.add(5, 3))
print(helpers.subtract(10, 4))
print(helpers.multiply(2, 6))
```

---

## Import A File With an Alias

You can rename a file during import using `as`.

* `helpers.py` still defines math functions.
* The file contains reusable logic only.
* No code runs automatically when imported.

```python
# helpers.py

def add(a, b):
    return a + b

def divide(a, b):
    return a / b
```

* `import helpers as h` renames the module.
* `h` is now the namespace.
* Dot notation is still required.

```python
# main.py

# Import helpers with an alias
import helpers as h

# Use the alias
print(h.add(8, 2))
print(h.divide(10, 5))
```

---

## Import Some of a File

You can import specific functions from a file.

* `helpers.py` defines multiple math functions.
* Each function is reusable.
* No automatic execution occurs.

```python
# helpers.py

def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

def subtract(a, b):
    return a - b
```

* `from helpers import add, multiply` imports specific functions.
* Imported functions can be called directly.
* No dot notation is needed.

```python
# main.py

# Import specific functions
from helpers import add, multiply

# Call directly
print(add(4, 5))
print(multiply(3, 3))
```

---

## Import All of A File with `*`

You can import everything into your current namespace.

* `helpers.py` defines multiple math functions.
* All functions are available for import.
* No top-level execution occurs.

```python
# helpers.py

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b
```

* `from helpers import *` imports all names.
* Functions are called directly.
* Can cause naming conflicts in large programs.

```python
# main.py

# Import everything from helpers
from helpers import *

print(add(10, 5))
print(subtract(8, 2))
print(multiply(4, 3))
```

---

## Preventing Code From Running

When a file is imported, all top-level code runs unless controlled properly.

* `helpers.py` defines functions.
* Top-level code would run if not protected.
* Use functions or special checks to prevent this.

```python
# helpers.py

def add(a, b):
    return a + b

# Top-level code (would run on import if not controlled)
print("Helpers file loaded")
```

* Importing this file runs top-level code.
* Demonstrates why protection is needed.
* Shows behavior when importing.

```python
# main.py

import helpers

# The print statement in helpers.py runs automatically
```

---

### By Containing it In Functions

Placing code inside functions prevents it from running automatically.

* Executable code is placed inside a function.
* Nothing runs unless explicitly called.
* Keeps the module clean when imported.

```python
# helpers.py

def add(a, b):
    return a + b

def run_demo():
    print(add(2, 3))
```

* Importing does not execute `run_demo()`.
* You must call the function manually.
* Demonstrates controlled execution.

```python
# main.py

import helpers

# Nothing runs automatically
helpers.run_demo()
```

---

### Using `if __name__ == "__main__:"`

This condition prevents code from running when imported.

* `__name__` is a built-in variable.
* The block runs only when the file is executed directly.
* Prevents execution during import.

```python
# helpers.py

def add(a, b):
    return a + b

if __name__ == "__main__":
    print(add(2, 3))
```

* Importing this file does not run the block.
* Code only runs if helpers.py is executed directly.
* Demonstrates safe structure.

```python
# main.py

import helpers

# The guarded code does NOT run
print(helpers.add(5, 5))
```

---

## Example - Basic Use

This example shows standard import usage.

* `helpers.py` defines math functions.
* Contains reusable logic only.
* No automatic execution.

```python
# helpers.py

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b
```

* `main.py` imports the file.
* Uses dot notation.
* Prints results.

```python
# main.py

import helpers

print(helpers.add(3, 7))
print(helpers.subtract(10, 6))
```

---

## Example - Importing an Alias

This example shows alias usage.

* Defines reusable functions.
* No automatic execution.
* Ready for import.

```python
# helpers.py

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b
```

* Uses alias `h`.
* Access via alias namespace.
* Demonstrates cleaner naming.

```python
# main.py

import helpers as h

print(h.multiply(4, 5))
print(h.divide(20, 4))
```

---

## Example - Importing Some of a File

This example imports only needed functions.

* Multiple math functions exist.
* Only specific ones are imported.
* No top-level execution.

```python
# helpers.py

def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b
```

* Imports selected functions.
* No dot notation required.
* Direct usage.

```python
# main.py

from helpers import add, divide

print(add(1, 9))
print(divide(8, 2))
```

---

## Example - Importing with `*`

Imports everything from the file.

* Defines several functions.
* All are available for import.
* No execution on import.

```python
# helpers.py

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b
```

* Imports all functions.
* Direct usage.
* Can cause conflicts in large projects.

```python
# main.py

from helpers import *

print(add(2, 2))
print(subtract(5, 3))
print(multiply(3, 4))
```

---

## Example - Importing Multiple Files

This example shows importing helpers plus another module.

* Defines math functions.
* Reusable module.
* No automatic execution.

```python
# helpers.py

def add(a, b):
    return a + b
```

* Imports helpers and built-in math.
* Uses both modules.
* Demonstrates multiple namespaces.

```python
# main.py

import helpers
import math

print(helpers.add(4, 6))
print(math.sqrt(16))
```

---

## Example - Prevent Code From Running By Putting it in Functions

Executable code is placed in a function.

* Defines math functions.
* Demo code is inside a function.
* Does not run automatically.

```python
# helpers.py

def add(a, b):
    return a + b

def demo():
    print(add(10, 5))
```

* Must call demo manually.
* Import does not trigger execution.
* Controlled behavior.

```python
# main.py

import helpers

helpers.demo()
```

---

## Example - Prevent Code From Running By Putting it in `if __name__ == "__main__:"`

Uses the special name check.

* Defines functions.
* Guards execution with condition.
* Safe for importing.

```python
# helpers.py

def multiply(a, b):
    return a * b

if __name__ == "__main__":
    print(multiply(3, 3))
```

* Import does not run guarded code.
* Only runs when helpers.py executed directly.
* Demonstrates best practice.

```python
# main.py

import helpers

print(helpers.multiply(5, 5))
```

---

## Example - Using a `main()` Function and Calling it in `if __name__ == "__main__:"`

Best practice structure for larger programs.

* Defines math functions.
* Uses a `main()` function.
* Calls `main()` only when run directly.

```python
# helpers.py

def add(a, b):
    return a + b

def main():
    print(add(7, 8))

if __name__ == "__main__":
    main()
```

* Import does not execute `main()`.
* Functions must be called explicitly.
* Clean and scalable structure.

```python
# main.py

import helpers

print(helpers.add(1, 2))
```
