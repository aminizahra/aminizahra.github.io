---
layout: post
title: "Python for AI, Step 1: Variables and Data Types"
date: 2026-10-02 10:00:00
description: Store values, understand the basic data types, and run your first Python code.
tags: python
step: 1
---

This is the first step of the Python series. By the end you will know how to store information in variables and which basic data types Python gives you.

#### What you will learn

- What a variable is and how to name one
- The four basic data types: `int`, `float`, `str` and `bool`
- How to check a type and convert between types

#### Variables

A variable is a name that points to a value.

```python
age = 25
height = 1.68
name = "Zahra"
is_student = True

print(name, age)
```

#### Basic data types

| Type | Example | Use |
|---|---|---|
| `int` | `25` | whole numbers |
| `float` | `1.68` | decimal numbers |
| `str` | `"Zahra"` | text |
| `bool` | `True` | yes or no |

Check the type of any value with `type()`:

```python
print(type(age))      # <class 'int'>
print(type(height))   # <class 'float'>
```

#### Converting types

```python
price = "120"
total = int(price) * 3
print(total)   # 360
```

#### Practice

1. Create variables for your name, your age and your favourite number.
2. Print a sentence that uses all three.
3. Convert the string `"3.14"` to a `float` and multiply it by 2.

<hr>

**Next step:** Conditions (`if`, `elif`, `else`).

Code and notebooks for this series: [Python-for-AI on GitHub](https://github.com/hobotacademy/Python-for-AI).
