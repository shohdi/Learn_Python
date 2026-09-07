# Lecture 3: print(), Variables, and Arithmetic 🐍🧮

**Estimated time:** 15 minutes, including a short exercise  
**Level:** Complete beginner  
**Goal:** Display messages, store values in variables, and calculate results.

**Before class:** Have Python 3 ready. The teacher can demonstrate in a Python editor or start Python by typing `python3` in macOS Terminal. Enter the Python examples at the `>>>` prompt without copying the prompt itself. Type `exit()` to return to Terminal. Installation is separate preparation for this lesson.

## 1. Give your program a voice: print() (2 minutes) 📣

`print()` is a built-in **function**: a named tool that performs a task. Its task is to display the values inside its parentheses. No paper or printer required—your ink budget is safe! 😄

```python
print("Hello, Python!")
print(25)
print("Score:", 25)
```

Output:

```text
Hello, Python!
25
Score: 25
```

Text goes inside matching quotes, either `"hello"` or `'hello'`. Numbers used for calculations do not need quotes. By default, commas separate the displayed values with a space, and each `print()` ends with a new line.

## 2. Variables: names for values (3 minutes) 🏷️

A **variable** is a name that refers to a value so we can use it later. Think of it as a label attached to information.

```python
student_name = "Mona"
age = 20
height = 1.65
print(student_name)
print("Age:", age)
```

Output:

```text
Mona
Age: 20
```

Here, `"Mona"` is text (a **string**, or `str`), `20` is a whole number (an **integer**, or `int`), and `1.65` is a number with a decimal point (a **float**).

The `=` symbol means **assignment**: evaluate the right side and associate its value with the name on the left. It does not ask whether two things are equal.

```python
age = 20
age = age + 1
print(age)
```

Output: `21`. Python reads the old value, adds one, and assigns the result to `age`. Congratulations: a birthday with no cake! 🎂

Use descriptive names such as `student_name` and `total_price`. Names can contain letters, digits, and underscores, but cannot start with a digit or contain spaces. They are case-sensitive: `age` and `Age` are different names. Avoid reserved words such as `class` and names of tools we need, such as `print`.

`print("age")` displays the word `age`; `print(age)` displays the variable's value. Quotes change the meaning!

## 3. Operations: Python the calculator (4 minutes) 🧮

An **operator** is a symbol that performs an operation. An **expression**, such as `3 + 2`, produces a value.

| Operator | Meaning | Example | Result |
| --- | --- | --- | --- |
| `+` | Addition | `7 + 2` | `9` |
| `-` | Subtraction | `7 - 2` | `5` |
| `*` | Multiplication | `7 * 2` | `14` |
| `/` | Division | `7 / 2` | `3.5` |
| `//` | Floor division | `7 // 2` | `3` |
| `%` | Remainder | `7 % 2` | `1` |
| `**` | Power | `2 ** 3` | `8` |

For positive whole numbers, `//` counts complete groups and `%` gives what is left over. Seven cookies shared between two people give three each and one cookie for the teacher. Excellent mathematics. 🍪

More precisely, `//` rounds the quotient down: `-7 // 2` is `-4`. Ordinary `/` division returns a float even for `8 / 2`, which gives `4.0`.

Parentheses control calculation order. For the positive-number examples here, powers come before multiplication/division/remainder, which come before addition/subtraction.

```python
print(2 + 3 * 4)
print((2 + 3) * 4)
```

Output:

```text
14
20
```

Quotes also affect operations:

```python
print(5 + 3)
print("5" + "3")
```

Output:

```text
8
53
```

With numbers, `+` adds. With strings, it joins text.

## 4. Solved examples (3 minutes) ✅

### Example 1: A tiny café receipt ☕

**Task:** Each drink costs 12 riyals. Buy three drinks, apply a 5-riyal discount to the whole order, and display the total.

```python
drink_price = 12
quantity = 3
discount = 5
total = drink_price * quantity - discount
print("Total:", total, "SAR")
```

Output:

```text
Total: 31 SAR
```

**Explanation:** First calculate `12 * 3 = 36`, then subtract `5`. The variable `total` receives `31`.

### Example 2: Minutes and leftover seconds ⏱️

**Task:** Convert 135 seconds into complete minutes and remaining seconds.

```python
total_seconds = 135
minutes = total_seconds // 60
seconds = total_seconds % 60
print("Minutes:", minutes)
print("Seconds:", seconds)
```

Output:

```text
Minutes: 2
Seconds: 15
```

**Explanation:** Two complete groups of 60 fit into 135, leaving 15.

## 5. Unsolved exercises (2 minutes) 🧠

Start exercise 1 in class. Finish the rest as homework; no solutions are included.

1. Create variables for your name and favorite number. Display both with labels using `print()`.
2. A notebook costs 8 riyals. Store its price and a quantity of 4 in variables, calculate the total, and display it.
3. Start with `score = 10`, increase it by 5 using assignment, and display the new score.
4. Predict the results of `print(10 + 2 * 3)`, `print((10 + 2) * 3)`, and `print("10" + "2")` before running them.
5. **Challenge:** You have 23 cookies and boxes that hold 5 each. Calculate the number of full boxes and the leftover cookies using variables.

## Quick recap and common mistakes 🎯 (1 minute)

`print()` displays values, variables give values names, and arithmetic operators calculate new values.

- Use matching straight quotes and closing parentheses.
- Assign a variable before using it; check spelling and capitalization if Python reports `NameError`.
- Use `print("Age:", age)` to display text alongside a number. Joining text and a number with `+` causes `TypeError`.
- Dividing by zero causes `ZeroDivisionError`.

Next: Let the user join the conversation with `input()`, then convert text into numbers using `int()` and `float()`. 🎤
