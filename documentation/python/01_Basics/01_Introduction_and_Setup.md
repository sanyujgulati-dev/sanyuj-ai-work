# Module 01: Introduction and Setup

## 🎯 Learning Objectives

By the end of this module, you will:
- Understand what Python is and why it's popular
- Install Python on your system
- Set up your development environment
- Run your first Python program
- Understand basic Python syntax

---

## 📖 What is Python?

**Python** is a high-level, interpreted programming language created by **Guido van Rossum** in 1991. It emphasizes code readability and simplicity.

### Why Learn Python?

1. **Beginner-Friendly**: Simple, readable syntax makes it easy to learn
2. **Versatile**: Used in web development, data science, AI, automation, scripting
3. **Large Community**: Millions of developers and extensive documentation
4. **Rich Ecosystem**: Thousands of libraries for various tasks
5. **In-Demand**: One of the most sought-after programming skills
6. **Fast Development**: Write less code to accomplish more

### Python Use Cases

- **Web Development**: Django, Flask, FastAPI
- **Data Science**: Pandas, NumPy, Scikit-learn
- **Machine Learning**: TensorFlow, PyTorch, Keras
- **Automation**: Scripting, testing, scheduling tasks
- **Scientific Computing**: SciPy, Matplotlib
- **Game Development**: Pygame
- **System Administration**: Server management, DevOps

---

## 🛠️ Installation Guide

### Windows

1. Visit [python.org](https://www.python.org/downloads/)
2. Download Python 3.8+ (latest stable version)
3. Run the installer
4. **IMPORTANT**: Check "Add Python to PATH" during installation
5. Click "Install Now"

**Verify Installation:**
```bash
python --version
```

### macOS

**Using Official Installer:**
1. Visit [python.org](https://www.python.org/downloads/)
2. Download macOS installer
3. Follow the installer steps

**Using Homebrew (Recommended):**
```bash
brew install python3
```

**Verify Installation:**
```bash
python3 --version
```

### Linux (Ubuntu/Debian)

```bash
# Update package manager
sudo apt update

# Install Python
sudo apt install python3 python3-pip

# Verify installation
python3 --version
```

### Linux (Fedora/RHEL)

```bash
sudo dnf install python3 python3-pip
python3 --version
```

---

## 📦 Setting Up Development Environment

### Step 1: Choose an IDE/Editor

**Beginner-Friendly Options:**
- **VS Code** (Recommended): Free, lightweight, powerful
  - Install "Python" extension by Microsoft
- **PyCharm Community Edition**: Full-featured IDE, free
- **IDLE**: Comes with Python, basic editor
- **Thonny**: Designed for beginners

**Installation Steps for VS Code:**
1. Download from [code.visualstudio.com](https://code.visualstudio.com/)
2. Install the Python extension
3. Create a folder for your projects

### Step 2: Create a Project Folder

```bash
# Create a folder for learning Python
mkdir python-learning
cd python-learning

# Create a subfolder for each module
mkdir module_01
cd module_01
```

### Step 3: Verify Setup

Create a file named `hello.py`:

```python
print("Hello, Python!")
```

Run it:
```bash
python hello.py
```

Expected output:
```
Hello, Python!
```

---

## 💻 Python Basics

### What is a Program?

A **program** is a set of instructions that tells the computer what to do. Python reads these instructions line by line, from top to bottom.

### Your First Program

```python
# This is a comment - Python ignores this line
print("Welcome to Python!")
print("This is my first program!")
```

**Output:**
```
Welcome to Python!
This is my first program!
```

### Understanding the Code

| Concept | Explanation |
|---------|-------------|
| `#` | Marks a comment (ignored by Python) |
| `print()` | Function that displays text on screen |
| `"text"` | String (text data) enclosed in quotes |
| `()` | Parentheses that contain function arguments |

---

## 🔤 Python Syntax Basics

### Rule 1: Indentation Matters

Python uses indentation (spaces/tabs) to define code blocks:

```python
# Correct indentation
if True:
    print("This is indented")
    print("Still indented")

print("Not indented - outside the if block")
```

### Rule 2: Case Sensitivity

Python distinguishes between uppercase and lowercase:

```python
name = "Alice"
NAME = "Bob"
Name = "Charlie"

# All three variables are different!
print(name)  # Alice
print(NAME)  # Bob
print(Name)  # Charlie
```

### Rule 3: Line Continuation

```python
# Long lines can continue with backslash
message = "This is a very long " \
          "string split across lines"

# Or use parentheses
result = (1 + 2 + 3 +
          4 + 5 + 6)
```

### Rule 4: Multiple Statements

```python
# One statement per line (preferred)
x = 5
y = 10
z = x + y

# Multiple statements on one line (not recommended)
x = 5; y = 10; z = x + y
```

---

## 🐍 Python Execution Models

### 1. Interactive Mode (REPL)

```bash
python
>>> print("Hello")
Hello
>>> x = 5
>>> x + 3
8
>>> exit()
```

Great for testing small code snippets.

### 2. Script Mode

Save code in `.py` file and run:

```bash
python filename.py
```

Used for full programs.

---

## ⚙️ How Python Works

```
Source Code (.py)
       ↓
    Compiler
       ↓
   Bytecode (.pyc)
       ↓
  Python Virtual Machine (PVM)
       ↓
    Output
```

Python is **interpreted**, meaning:
- Code is compiled to bytecode
- Bytecode runs on Python Virtual Machine
- This makes Python portable (runs same on Windows, Mac, Linux)

---

## 📝 Python Naming Conventions (PEP 8)

PEP 8 is Python's style guide. Follow these conventions:

### Variable and Function Names (snake_case)
```python
# Good ✓
first_name = "Alice"
calculate_total = 10

# Avoid ✗
firstName = "Alice"
CalculateTotal = 10
```

### Constants (UPPERCASE)
```python
# Good ✓
MAX_USERS = 100
PI = 3.14159

# Avoid ✗
max_users = 100
```

### Class Names (PascalCase)
```python
# Good ✓
class UserProfile:
    pass

# Avoid ✗
class user_profile:
    pass
```

### Avoid Single Letters (except in loops)
```python
# Good ✓
user_count = 5
for item in items:
    print(item)

# Avoid ✗
uc = 5
for x in items:
    print(x)
```

---

## 🎯 Best Practices

1. **Use Descriptive Names**: `user_age` not `ua`
2. **Keep Code Simple**: Simple is better than complex
3. **Comment When Necessary**: Explain the "why", not the "what"
4. **Follow PEP 8**: Maintains consistency
5. **Test Frequently**: Run code often to catch errors early

---

## ⚠️ Common Mistakes

### Mistake 1: Wrong Indentation
```python
# Wrong ✗
if True:
print("Indented incorrectly")

# Correct ✓
if True:
    print("Properly indented")
```

### Mistake 2: Forgetting Colons
```python
# Wrong ✗
if True
    print("Missing colon")

# Correct ✓
if True:
    print("Has colon")
```

### Mistake 3: Using Reserved Words
```python
# Wrong ✗
class = "Python"  # 'class' is reserved
if = 5            # 'if' is reserved

# Correct ✓
class_name = "Python"
condition = 5
```

---

## 🧪 Practice Exercise

### Exercise 1: Setup and First Program

1. Create a new folder `python_practice`
2. Create file `hello_world.py`
3. Write a program that prints:
   ```
   Hello, World!
   I am learning Python!
   Python is fun!
   ```
4. Run the program

### Exercise 2: Experiment with Comments

```python
# TODO: Create a program that prints your name
# and favorite hobby on separate lines

# Your code here:
print("Your Name")
print("Your Hobby")
```

---

## 📚 Key Takeaways

1. ✅ Python is a beginner-friendly, versatile language
2. ✅ Installation is straightforward on all platforms
3. ✅ Use an IDE like VS Code for better development experience
4. ✅ Python uses indentation to define code blocks
5. ✅ Follow PEP 8 style guide for consistent code
6. ✅ Comments start with `#`
7. ✅ `print()` displays output
8. ✅ Test code frequently in both interactive and script modes

---

## 🔗 Next Steps

Proceed to **[Module 02: Variables and Data Types](./02_Variables_and_Data_Types.md)** to learn how to store and manipulate data.

---

## 📖 Additional Resources

- [Python Official Docs - Introduction](https://docs.python.org/3/tutorial/introduction.html)
- [PEP 8 Style Guide](https://www.python.org/dev/peps/pep-0008/)
- [Real Python - Getting Started](https://realpython.com/python-basics/)

---

**Happy coding! 🐍**
