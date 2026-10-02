---
layout: post
title: "Python Basics: Postscript – Python Memory Management and Immutability"
date: 2026-10-02
tags: [Python]
step: 7
---

Welcome back! In our previous sessions, we successfully learned how to define variables, assign different data types, and explicitly cast them. We treated variables like simple "boxes" holding our data. 

However, to write highly optimized code for Artificial Intelligence and Machine Learning—where you will process millions of data points—you must understand what is actually happening under the hood. How does Python store this data? What happens to data we no longer need?

In this special postscript session, we will dive into **Python Memory Management**, the `id()` function, Immutability, and Garbage Collection.

---

## The Reality of Variables in Python

In many older programming languages (like C), a variable is a specific designated space in memory. In Python, **variables are just name tags (references)** pointing to objects in the computer's memory. The data itself is the object.

Let's explore this step-by-step using Python's built-in `id()` function, which returns the exact memory address of an object.

### 1. Object Creation and Variable Referencing

When you assign a value to a variable, Python first creates the object in memory and then attaches the variable name to it as a reference.

```python
# 1. Object Creation and Value Assignment
# The value 10 is created as an integer object in memory. 
# The variable 'x' is created and points to that object's memory address.
x = 10  

# 2. Variable Referencing
# Here, 'y' does NOT create a new object. It simply points to the 
# exact same object (10) that 'x' is pointing to.
y = x  

# Checking the memory address of the object using the id() function
print(f"Address of x: {id(x)}")  # e.g., Output: 140717769671752
print(f"Address of y: {id(y)}")  # e.g., Output: 140717769671752
```
*Notice that both `x` and `y` output the exact same memory address. They are two different name tags attached to the same piece of data.*

---

### 2. Reassignment and Garbage Collection

What happens if we change the value of `x`? Because `x` is just a reference, it simply stops pointing to `10` and starts pointing to a newly created object. 

When an object in memory has zero variables pointing to it, Python's automated **Garbage Collector (GC)** steps in and deletes the object to free up your computer's RAM.

```python
# 3. Reassignment and Garbage Collection
x = 20  
# Now, 'x' points to a newly created object with the value 20.
# If 'y' was not still pointing to 10, the object '10' would be 
# cleared from memory by the Garbage Collector.

print(f"New address of x: {id(x)}")  # e.g., Output: 140717769672072
```

---

### 3. Understanding Immutability

In Python, primitive data types like `int`, `float`, `str`, and `bool` are **Immutable** (unchangeable). 

This is a critical concept: *You cannot alter the actual object in memory once it is created.* When you try to modify a number or a string, Python actually creates a brand-new object in memory and points the variable to the new one.

```python
# 4. Immutable Data Types in Action

# Integer Example
num = 42
print(f"Address of num: {id(num)}")  # Output: 140717769672776

# We mathematically add 1 to num. 
# Because integers are immutable, Python creates a new object (43).
num += 1  
print(f"New address of num after change: {id(num)}")  # Output: 140717769672808
# The address has changed!

# String Example
text = "Hello"
print(f"Address of text: {id(text)}")  # Initial address of the string

# Appending text creates a new string object in memory
text += " World"  
print(f"New address of text after change: {id(text)}")  # New address generated
```

---

### 4. Memory Optimization (Integer Caching)

Python is highly optimized for performance. To save memory and execution time, the CPython implementation pre-loads and caches small, frequently used integers (specifically from `-5` to `256`).

If you assign two different variables to the same small integer within this range, Python will not create two separate objects. It will point both variables to the cached object.

```python
# 5. Memory Optimization for Small Integers (Interning)
a = 256
b = 256

# Because 256 falls within the optimized range (-5 to 256), 
# both 'a' and 'b' point to the exact same pre-existing object in memory.
print(f"Do a and b point to the same memory address? {id(a) == id(b)}")  
# Output: True
```
*(Note: If you were to do this with large numbers, like `a = 1000` and `b = 1000` in standard execution environments, they would generate different memory addresses because they fall outside the cached range!)*

---

## Conclusion

Understanding memory references, immutability, and garbage collection separates average programmers from excellent software engineers. When you begin passing enormous datasets into machine learning algorithms, knowing how to manage variable references prevents memory leaks and fatal system crashes.

Now that we understand how data lives in our computer's memory, we are ready to manipulate it. In our next official session, we will explore **Python Operators** (Arithmetic, Logical, and Comparison). Stay tuned!

---

## Notebook
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hobotacademy/Python-for-AI/blob/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)

[📄 View or Download the Python Notebook](https://github.com/hobotacademy/Python-for-AI/blob/main/01_Py_Basics/01_Py_Basics-ASH.ipynb)