# Lecture 4: Conditions and if Statements 🐍🚦

**Estimated time:** 15 minutes, including a short exercise  
**Level:** Complete beginner  
**Goal:** Compare values and choose what a program does using `if`, `else`, and `elif`.

**Before class:** Have Python 3 ready in a Python editor. We use variables, `print()`, and arithmetic from Lecture 3. Run each code block separately and change its starting values to explore different results.

**Using Terminal?** Start Python with `python3`. When entering a conditional statement, Python shows `...` for continuation lines. Do not copy the prompts. Indent the body, keep any `elif` and `else` attached to the same statement, and enter a blank line after the whole statement to execute it. Then enter any following unindented instruction. Type `exit()` to leave Python.

## 1. Conditions and comparisons (3 minutes) ❓

A **condition** is an expression a program checks to decide what to do. Our comparisons produce a **Boolean** value (type `bool`): `True` or `False`.

“Is the temperature at least 30?” is a question Python can answer. “Is the weather nice?” needs more detail! ☀️

| Operator | Meaning | Example | Result |
| --- | --- | --- | --- |
| `==` | Equal to | `5 == 5` | `True` |
| `!=` | Not equal to | `5 != 5` | `False` |
| `>` | Greater than | `7 > 5` | `True` |
| `<` | Less than | `7 < 5` | `False` |
| `>=` | Greater than or equal to | `5 >= 5` | `True` |
| `<=` | Less than or equal to | `6 <= 5` | `False` |

```python
temperature = 30
is_hot = temperature >= 30
print(is_hot)
print(temperature < 30)
print("tea" == "Tea")
```

Output:

```text
True
False
False
```

`=` assigns a value; `==` compares values. Text comparisons are case-sensitive. Write `True` and `False` with capital first letters and no quotes: `"False"` is text, not a Boolean.

## 2. if: act when a condition is true (3 minutes) 🚦

An **`if` statement** runs a group of instructions only when its condition is true.

```python
temperature = 32
if temperature >= 30:
    print("It is hot!")
    print("Bring some water.")
print("Weather check complete.")
```

Output:

```text
It is hot!
Bring some water.
Weather check complete.
```

The colon (`:`) introduces a **block**, a group of instructions belonging together. **Indentation**, the spaces at the start of a line, tells Python which instructions belong to that block. Use four spaces for each indented line here.

Both indented messages belong to `if`. The final `print()` lines up with `if`, so it runs after the check whether the condition was true or false. Change `temperature` to `25` and the only output is `Weather check complete.`

Spaces now have a job. They are no longer just decorating the page! 😄

## 3. else and elif: choose a path (3 minutes) 🛤️

**`else`** provides an alternative when the `if` condition is false. It has a colon but no condition of its own.

```python
score = 45
if score >= 50:
    print("Pass")
else:
    print("Keep practicing")
```

Output:

```text
Keep practicing
```

Exactly one of these two blocks runs. A score of exactly `50` takes the `if` path because `>=` includes equality.

**`elif`**, short for “else if,” checks another condition if the earlier conditions were false.

```python
score = 85
if score >= 90:
    print("Excellent")
elif score >= 50:
    print("Pass")
else:
    print("Keep practicing")
```

Output:

```text
Pass
```

Python checks from top to bottom and runs only the **first matching block** in this chain. If nothing matches, it runs `else`. You can have several `elif` blocks; `else` is optional and goes last. Align `if`, `elif`, and `else` with each other.

Order matters: check `>= 90` before `>= 50`, or `95` would match the lower threshold first. Separate `if` statements are independent checks, so more than one of their blocks can run.

## 4. Solved examples (3 minutes) ✅

### Example 1: A café discount ☕

**Task:** Give a 5-riyal discount on orders of at least 30 riyals. Otherwise, keep the original total. Display the final price.

```python
total = 36
if total >= 30:
    total = total - 5
print("Total:", total, "SAR")
```

Output:

```text
Total: 31 SAR
```

**Explanation:** `36 >= 30` is true, so Python subtracts 5. The final `print()` runs after the check. Starting at `30` gives `25 SAR`; starting at `29` gives `29 SAR`. No `else` is needed because there is no extra action when the condition is false.

### Example 2: Even or odd? 🔢

**Task:** Decide whether a whole number is even or odd.

```python
number = 7
if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

Output:

```text
Odd
```

**Explanation:** `%` gives the remainder, as we learned in Lecture 3. Dividing 7 by 2 leaves 1, so the comparison with 0 is false. Try `8` and `0`: both give `Even`.

## 5. Unsolved exercises (2 minutes) 🧠

Do exercise 1 in class. Exercises 2–5 are homework; no solutions are included.

1. Set `battery = 15`. Use `if`/`else` to display `Charge now` when the battery is below 20, or `Battery OK` otherwise. Try `15`, `20`, and `80`.
2. Set `number` to a number of your choice. Use `if`/`elif`/`else` to display `Positive`, `Negative`, or `Zero`. Try one value from each group.
3. Delivery costs 10 riyals on orders below 100 riyals and is free otherwise. Store an order total, calculate delivery, and display the final total. Try `99`, `100`, and `101`.
4. Use the score example in section 3. Predict the output for `49`, `50`, `89`, and `90` before running it. Explain why condition order matters.
5. **Challenge:** Store `drink = "tea"`. Display one message for `"tea"`, another for `"coffee"`, and a fallback message for any other value. What happens with `"Tea"`?

## Quick recap and common mistakes (1 minute) 🎯

Comparisons produce `True` or `False`. Use `if` for a conditional action, `elif` for another check, and `else` for the remaining case.

- Compare with `==`, not `=`.
- Put `:` after every `if`, `elif`, and `else` header.
- Indent blocks consistently with four spaces; avoid mixing tabs and spaces.
- Write `elif`, not `else if`, and do not add a condition after `else`.
- Test the exact boundary: `>` excludes equality; `>=` includes it.
- Compare numbers with numbers. `"20" == 20` is false; `"20" > 10` causes `TypeError` because it tries to order text and a number.

**Timing:** 3 + 3 + 3 + 3 + 2 + 1 = 15 minutes.

Next: Get values with `input()`, convert text with `int()` and `float()`, and use those values in decisions. 🎤
