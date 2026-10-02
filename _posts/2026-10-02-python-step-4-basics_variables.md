---
layout: post
title: "Python Basics: Variables and Data Types"
date: 2026-10-02
tags: [Python]
step: 4
---

Welcome to our foundational Python series! Before we can train advanced Machine Learning models or build complex Artificial Intelligence systems, we must master the core building blocks of programming. 

In Python, everything revolves around data, and the most fundamental way to interact with data is through **Variables**. In this session, we will explore how Python stores information, the different types of data it handles, and the industry-standard rules for writing clean, readable code.

---

## Learning Objectives for Session 1

By the end of this tutorial, you will be able to:

*   Understand the concept of **variables** in Python and define variables with different data types.
*   Identify basic Python data types, including **integers**, **floats**, **strings**, and **booleans**.
*   Use **casting** to convert between different data types.
*   Apply various Python **operators**, including arithmetic, comparison, and logical operators.
*   Utilize **common string methods** to process and manipulate text.

*(Note: This specific post will focus deeply on Variables, Data Types, and Naming Rules. We will cover casting and operators in upcoming parts of this session!)*

These objectives will help you gain a foundational understanding of Python programming basics and prepare you for more advanced data science topics.

---

## 1. Data Types: `int`, `float`, `string`, `boolean`

Think of a variable as a labeled box in your computer's memory where you can store data. In Python, you do not need to explicitly declare what type of data will go into the box; Python dynamically understands it based on the value you provide.

Here is how we define variables containing the four most common primitive data types:

```python
x = 5
y = 3.14
s = "Hello, Python!"
is_student = True
```

## 2. Assigning Variables with Different Data Types

Let's look at a more practical example. When building a profile for a user, you will naturally use a mix of these data types. The `=` symbol is the **assignment operator**, which assigns the value on the right to the variable name on the left.

```python
name = "Ali"             # String: Used for text (enclosed in quotes)
age = 20                 # Integer (int): Whole numbers
height = 1.75            # Float: Decimal numbers
is_graduated = False     # Boolean (bool): Represents True or False logic
```

## 3. Variable Naming Rules

To ensure your code executes without errors, Python enforces strict rules on how you can name your variables. Furthermore, the developer community relies on conventions to make code readable. 

Here are the absolute rules you must follow:

*   **Start with a Letter or Underscore:** A variable name must begin with a letter or an underscore `_`. It **cannot** start with a number.
*   **Contain Letters, Numbers, and Underscores:** A variable name can only include English letters (A-Z, a-z), numbers (0-9), and underscores `_`. No spaces or special characters (like `-`, `@`, or `!`) are allowed.
*   **Case Sensitivity:** Variable names are case-sensitive. This means `Name` and `name` are treated as two entirely distinct variables in memory.
*   **Avoiding Keywords:** Reserved words in Python (such as `class`, `if`, `while`, `True`, `def`, etc.) have special meanings and cannot be used as variable names.

Let's see these rules in action:

```python
# --- Correct Examples ---
student_name = "Sara"
age = 21
_score = 95

# --- Incorrect Examples (These will cause Syntax Errors) ---
# 1st_student = "Ali"   # Error: Starts with a number
# student-age = 19      # Error: Contains a dash (Python interprets this as subtraction)
# class = "Physics"     # Error: Uses a reserved Python keyword
```

---

## Naming Conventions: How to Write Professional Code

While Python allows you to name your variables in many ways, software engineers follow specific patterns to keep their code organized. Here are the four primary conventions:

### 3.1. `snake_case`
All lowercase letters with words separated by underscores. 
**Usage:** This is the standard convention in Python for naming **variables** and **functions**.

```python
first_name = "Ali"
total_price = 2500
number_of_students = 30
```

### 3.2. `PascalCase`
The first letter of every word is capitalized, with no spaces or underscores.
**Usage:** In Python, this is strictly used for naming **Classes** (Object-Oriented Programming).

```python
FirstName = "Ali"
TotalPrice = 2500
NumberOfStudents = 30
```

### 3.3. `camelCase`
Similar to PascalCase, but the very first letter is lowercase.
**Usage:** Generally *not* used in standard Python code. It is highly common in other languages like JavaScript, Java, or C++.

```python
firstName = "Ali"
totalPrice = 2500
numberOfStudents = 30
```

### 3.4. `UPPER_CASE`
All letters are capitalized, with words separated by underscores.
**Usage:** Used for **Constants**—values that are set once and should never change throughout the execution of the program.

```python
PI = 3.14159
MAX_CONNECTIONS = 100
DEFAULT_TIMEOUT = 3000
```

### Summary of Conventions in Python:
*   `snake_case`: Used for variables and functions.
*   `PascalCase`: Used for classes.
*   `camelCase`: Not standard in Python.
*   `UPPER_CASE`: Used for constant values.

---

## 4. Common Data Types in Variables (Recap)

To solidify what we have learned, here is a final summary of assigning our core data types to variables using proper `snake_case` formatting:

```python
age = 25              # Integer
height = 1.75         # Float
name = "Ali"          # String
is_student = True     # Boolean
```

Mastering these basic assignments and rules is your first major step toward writing robust Python scripts. Practice defining your own variables, and in our next section, we will explore how to manipulate these values using **Operators** and **String Methods**!

## Notebook
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hobotacademy/Python-for-AI/blob/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)

[📄 Download the Python Code/Notebook](https://raw.githubusercontent.com/hobotacademy/Python-for-AI/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)

