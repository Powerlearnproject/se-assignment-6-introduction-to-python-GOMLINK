### Python Basics

**What is Python?**

Python is a high-level, interpreted programming language known for its readability and simplicity. Created by Guido van Rossum and first released in 1991, it emphasizes code readability with its notable use of significant whitespace.

**Key Features of Python:**
1. **Easy to Learn and Use:** Python's syntax is straightforward, making it a great language for beginners.
2. **Interpreted Language:** Python executes code line by line, which simplifies debugging.
3. **Dynamically Typed:** No need to declare the type of variable, making code more flexible.
4. **Extensive Standard Library:** Python comes with a wide range of libraries and modules that simplify many common tasks.
5. **Community Support:** A large and active community contributes to a wealth of resources, libraries, and frameworks.

**Use Cases:**
- **Web Development:** Using frameworks like Django and Flask.
- **Data Science:** Libraries such as Pandas, NumPy, and Matplotlib.
- **Automation:** Scripts to automate repetitive tasks.
- **Machine Learning:** Libraries like TensorFlow and scikit-learn.
- **Game Development:** Using Pygame.

### Installing Python

**Steps to Install Python:**

**Windows:**
1. Download the Python installer from the [official website](https://www.python.org/downloads/).
2. Run the installer and ensure the "Add Python to PATH" option is checked.
3. Follow the prompts to complete the installation.

**macOS:**
1. Install Homebrew if not already installed: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Use Homebrew to install Python: `brew install python`

**Linux:**
1. Update your package list: `sudo apt update`
2. Install Python: `sudo apt install python3`

**Verify Installation:**
Open a terminal or command prompt and type:
```sh
python --version
```
or
```sh
python3 --version
```

**Set Up a Virtual Environment:**
1. Install `virtualenv` (if not already installed):
    ```sh
    pip install virtualenv
    ```
2. Create a virtual environment:
    ```sh
    virtualenv venv
    ```
3. Activate the virtual environment:
   - Windows:
     ```sh
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```sh
     source venv/bin/activate
     ```

### Python Syntax and Semantics

**Simple Python Program:**
```python
print("Hello, World!")
```

**Explanation:**
- `print`: A built-in function that outputs text to the console.
- `"Hello, World!"`: A string literal enclosed in double quotes.

### Data Types and Variables

**Basic Data Types:**
1. **Integer (`int`)**: Whole numbers, e.g., `42`
2. **Float (`float`)**: Decimal numbers, e.g., `3.14`
3. **String (`str`)**: Sequence of characters, e.g., `"Hello"`
4. **Boolean (`bool`)**: `True` or `False`

**Example Script:**
```python
# Integer
age = 25
print(age)

# Float
pi = 3.14
print(pi)

# String
name = "Alice"
print(name)

# Boolean
is_student = True
print(is_student)
```

### Control Structures

**Conditional Statements:**
```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")
```

**For Loop:**
```python
for i in range(5):
    print(i)
```

### Functions in Python

**Functions:**
Functions are blocks of reusable code that perform a specific task. They help in modularizing and organizing code.

**Example Function:**
```python
def add(a, b):
    return a + b

# Calling the function
result = add(3, 5)
print(result)  # Output: 8
```

### Lists and Dictionaries

**Lists:**
Ordered collections of items.
```python
numbers = [1, 2, 3, 4, 5]
print(numbers)

# Accessing elements
print(numbers[0])

# Adding an element
numbers.append(6)
print(numbers)
```

**Dictionaries:**
Unordered collections of key-value pairs.
```python
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
print(person)

# Accessing values
print(person["name"])

# Adding a key-value pair
person["email"] = "alice@example.com"
print(person)
```

### Exception Handling

**Exception Handling:**
Managing errors during runtime to prevent the program from crashing.
```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
finally:
    print("Execution completed.")
```

### Modules and Packages

**Modules and Packages:**
Modules are files containing Python code. Packages are directories containing multiple modules.

**Importing a Module:**
```python
import math

# Using a function from the math module
print(math.sqrt(16))
```

### File I/O

**Reading from a File:**
```python
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
```

**Writing to a File:**
```python
lines = ["First line", "Second line", "Third line"]

with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")
```

These examples cover the basic aspects of Python and provide a foundation for further exploration and learning.
