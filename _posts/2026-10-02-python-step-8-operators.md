---
layout: post
title: "Python Basics: Operators (Arithmetic, Comparison, and Logical)"
date: 2026-10-02
tags: [Python]
step: 8
---

Welcome back to our Python foundational series! In our previous sessions, we successfully learned how to define variables, assign various data types, cast data, and understand how Python manages memory under the hood. 

However, simply storing data is not enough. To build algorithms, process datasets, or train machine learning models, we need to manipulate this data and evaluate conditions. This is where **Operators** come into play.

In this session, we will explore the three most essential categories of Python operators: Arithmetic, Comparison, and Logical operators.

---

## 1. Arithmetic Operators

Arithmetic operators are used to perform common mathematical operations. In data science, you will use these constantly to calculate statistics, normalize data, or adjust weights in a neural network.

Python provides a comprehensive set of mathematical operators:

| Operator | Description | Example | Example Result |
| :---: | :--- | :--- | :--- |
| `+` | **Addition** | `x + y` | If x=3 and y=2, the result is 5 |
| `-` | **Subtraction** | `x - y` | If x=5 and y=3, the result is 2 |
| `*` | **Multiplication** | `x * y` | If x=4 and y=3, the result is 12 |
| `/` | **Division** | `x / y` | If x=10 and y=2, the result is 5.0 (always returns a float) |
| `**` | **Exponentiation** | `x ** y` | If x=2 and y=3, the result is 8 (2 to the power of 3) |
| `%` | **Modulus** | `x % y` | If x=5 and y=2, the result is 1 (returns the remainder) |
| `//` | **Floor Division** | `x // y` | If x=10 and y=3, the result is 3 (rounds down to nearest whole number) |

### Code Example: Arithmetic in Action

```python
# Example of using arithmetic operators
x = 10
y = 3

print("Addition:", x + y)            # Output: 13
print("Subtraction:", x - y)         # Output: 7
print("Multiplication:", x * y)      # Output: 30
print("Division:", x / y)            # Output: 3.3333333333333335
print("Exponentiation:", x ** y)     # Output: 1000
print("Modulus (remainder):", x % y) # Output: 1
print("Floor Division:", x // y)     # Output: 3
```

---

## 2. Comparison Operators

Comparison operators are used to compare two values. Instead of returning a number, they evaluate the mathematical relationship and return a Boolean value (`True` or `False`). 

These operators form the backbone of "Control Flow" (like `if` statements), allowing your program to make decisions based on the data it receives.

| Operator | Description | Example | Result of Example |
| :---: | :--- | :--- | :--- |
| `==` | **Equal to** | `x == y` | If `x=5` and `y=5`, the result is `True`. |
| `!=` | **Not equal to** | `x != y` | If `x=5` and `y=3`, the result is `True`. |
| `>` | **Greater than** | `x > y` | If `x=10` and `y=2`, the result is `True`. |
| `<` | **Less than** | `x < y` | If `x=2` and `y=5`, the result is `True`. |
| `>=` | **Greater than or equal** | `x >= y` | If `x=5` and `y=5`, the result is `True`. |
| `<=` | **Less than or equal** | `x <= y` | If `x=3` and `y=5`, the result is `True`. |

### Code Example: Comparing Values

```python
# Example of using comparison operators
x = 5
y = 10

print("x is equal to y:", x == y)                  # Output: False
print("x is not equal to y:", x != y)              # Output: True
print("x is greater than y:", x > y)               # Output: False
print("x is less than y:", x < y)                  # Output: True
print("x is greater than or equal to y:", x >= y)  # Output: False
print("x is less than or equal to y:", x <= y)     # Output: True
```

---

## 3. Logical Operators

Sometimes, evaluating a single condition is not enough. You may need to check if *multiple* conditions are true simultaneously, or if at least *one* of several conditions is met. 

Logical operators are used to combine multiple conditional statements. They also return a Boolean value (`True` or `False`).

| Operator | Description | Example | Result of Example |
| :---: | :--- | :--- | :--- |
| `and` | Returns `True` if **both** conditions are `True` | `(x > 0) and (x < 10)` | If `x=5`, the result is `True`. |
| `or` | Returns `True` if **at least one** condition is `True` | `(x > 0) or (x < 10)` | If `x=-5`, the result is `True`. |
| `not` | Returns the **opposite** Boolean value | `not(x > 0)` | If `x=5`, the result is `False`. |

### Code Example: Combining Logic

```python
# Example of using logical operators
x = 5
y = 15

# and operator: Both sides must be True
print("x is greater than 0 and less than 10:", (x > 0) and (x < 10))  
# Output: True

# or operator: Only one side needs to be True
print("x is greater than 0 or y is less than 10:", (x > 0) or (y < 10))  
# Output: True

# not operator: Inverts the Boolean result
print("x is not greater than 0:", not(x > 0))  
# Output: False
```

---

## Conclusion

Understanding operators is like learning the grammar of a language; they allow you to take basic vocabulary (variables) and construct meaningful sentences (logic and mathematics). 

Whether you are calculating the error rate of a machine learning model using arithmetic, or filtering a dataset using logical and comparison operators, these tools will be present in nearly every script you write.

In our next session, we will explore **String Methods** and learn how to manipulate text data powerfully and efficiently. Keep practicing, and happy coding!

---

## Notebook
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hobotacademy/Python-for-AI/blob/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)

[📄 View or Download the Python Notebook](https://github.com/hobotacademy/Python-for-AI/blob/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)