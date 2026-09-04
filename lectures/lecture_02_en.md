# Lecture 2: Programming Languages and Python 🐍

**Estimated time:** 15 minutes  
**Level:** Complete beginner  
**Goal:** Understand programming languages, recognize common ways to classify them, and discover what Python is.

## 1. What is a programming language? (4 minutes) 🗣️

A computer is fast, obedient, and impressively bad at guessing what we mean. A **programming language** is a structured language used to give a computer instructions.

A **program** is a sequence of those instructions. For example, a program might tell the computer to:

1. Ask for a user's name.
2. Store the answer.
3. Display a greeting.

Computers ultimately execute **machine code**, made of binary instructions represented using `0` and `1`. Humans usually write code in friendlier languages, and special software translates it into instructions the computer can execute.

Programming languages have:

- **Syntax:** the rules for writing valid code—like grammar.
- **Semantics:** what the code means.
- **Vocabulary:** keywords and symbols with special jobs.

If syntax is grammar, a syntax error is the computer saying, “I know every word, but this sentence has three hats and no trousers.” 🎩

## 2. Types of programming languages (5 minutes) 🧩

Languages can be grouped in several ways. These groups overlap; they are not rival sports teams.

### Low-level and high-level

- **Low-level languages** are close to the computer's hardware. Machine code and Assembly are examples. They offer detailed control but are harder for people to read and write.
- **High-level languages** are closer to human reasoning and hide many hardware details. Python, JavaScript, Java, and C# are examples.

### Compiled and interpreted

- A **compiled language** is commonly translated into machine code before the program runs. C and Rust are common examples.
- An **interpreted language** is commonly executed through another program called an interpreter. Python and JavaScript are common examples.

Real implementations can mix these approaches. For example, Python commonly compiles source code to bytecode and then executes it using the Python virtual machine. So these labels are helpful introductions, not unbreakable laws carved into a keyboard. ⌨️

### Programming paradigms

A **paradigm** is a style of organizing programs:

- **Procedural:** organize work as steps and reusable procedures.
- **Object-oriented:** organize code around objects that contain data and behavior.
- **Functional:** build programs mainly by combining functions and limiting changing state.

Many modern languages support more than one paradigm. Python supports all three.

## 3. What is Python? (3 minutes) 🐍

**Python** is a high-level, general-purpose programming language created by Guido van Rossum and first released in 1991. Its name was inspired by the comedy group *Monty Python*, not by the snake—but the snake has clearly won the logo competition. 🐍🏆

Python is popular because it emphasizes readable code and can be used for many tasks, including:

- Web development
- Automation and scripting
- Data analysis and visualization
- Artificial intelligence and machine learning
- Scientific computing
- Education and quick prototypes

A tiny Python program looks like this:

```python
print("Hello, world!")
```

`print()` asks Python to display something on the screen. The text inside quotation marks is called a **string**.

## 4. Solved examples (3 minutes) ✅

### Example 1: Identify the language level

**Question:** Python hides most processor and memory details and lets us use readable commands. Is it low-level or high-level?

**Solution:** It is a **high-level language** because its code is designed to be easier for humans to understand and abstracts many hardware details.

### Example 2: Read a simple program

```python
name = "Mona"
print("Hello", name)
```

**Solution:**

1. The first line stores the text `Mona` under the name `name`.
2. The second line displays a greeting.
3. The output is:

```text
Hello Mona
```

### Example 3: Match a tool to a task

**Question:** You need to rename 500 files automatically. Could Python help?

**Solution:** Yes. Automation is a common use of Python. The program can repeat the renaming instructions while you perform the critical engineering duty of drinking coffee. ☕

## Unsolved exercises 🧠

1. Explain “programming language” in one sentence, using your own words.
2. What is the difference between syntax and semantics?
3. Classify Python as low-level or high-level, and explain why.
4. Name two compiled languages and two commonly interpreted languages mentioned in this lecture.
5. List three jobs for which Python can be used.
6. Predict what this code displays:

   ```python
   course = "Python"
   print("I am learning", course)
   ```

7. **Challenge:** Think of a boring task you repeat on a computer. Describe how a program might automate it; no code is required.

## Quick recap 🎯

- A programming language lets humans express instructions for computers.
- Languages may be described by their level, execution method, and paradigm.
- Classifications can overlap.
- Python is a readable, high-level, general-purpose language.
- Python is widely used in automation, web development, data work, AI, and education.

Next: Install/check Python on macOS, meet the Python interpreter, and run our first real program. 🚀
