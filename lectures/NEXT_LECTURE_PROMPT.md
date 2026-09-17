# Prompt for the Next Course-Writing Session 📝

Copy and send this prompt when it is time to prepare the next lecture:

> Continue building the beginner Python course in this repository. Read the existing lectures to preserve the established structure, tone, and numbering, and avoid repeating material. Lectures 1 and 2 covered macOS files/folders/Terminal commands and an introduction to programming languages/Python. Lecture 3 covered `print()`, variables, assignment and reassignment, naming rules, a brief introduction to `str`/`int`/`float`, arithmetic operators (`+`, `-`, `*`, `/`, `//`, `%`, `**`), parentheses, and text versus numeric addition. It included café-receipt and time-conversion examples.
>
> The user chose practical Python topics for Lecture 3 instead of the previously proposed installation lesson. Installation and running `.py` files have not been taught in a dedicated lecture; Lecture 3 assumes Python 3 is ready and briefly explains starting/exiting the interpreter. Do not assume setup was taught or insert an installation lecture unless requested.
>
> The user chose conditions and `if` statements for Lecture 4. Lecture 4 covered comparison operators, Boolean values (`True`/`False`), `if`/`elif`/`else`, colons and indentation, first-match behavior versus separate `if` statements, and boundary values. Its solved examples covered conditional café discounts and even/odd checks. It also explained entering conditional blocks in the interpreter. `input()`, numeric conversion, and logical operators (`and`, `or`, `not`) have not been taught.
>
> Unless the user requests a different topic, create Lecture 5 in `lectures/lecture_05_en.md` and `lectures/lecture_05_ar.md`, covering `input()`, its string result, conversion with `int()` and `float()`, and a small interactive calculator using previously taught conditions where useful. Explain invalid numeric input briefly without introducing exception handling yet. Make each version about 15 minutes, beginner-friendly, accurate, funny, and include emojis. Include topic descriptions, solved examples with expected output, unsolved exercises, a timing breakdown totaling 15 minutes, common mistakes, and a recap. Count a short practice task in the timing and label longer exercises as homework. Use natural Arabic and copyable Python 3 code. Update this prompt afterward; a suggested next topic is combining conditions with `and`, `or`, and `not`.

## Course conventions to preserve

- One topic-sized lecture should take approximately 15 minutes.
- Maintain separate English and Arabic files.
- Every lecture must contain explanations, solved examples, and unsolved exercises.
- Use clear headings, short sections, copyable code blocks, gentle humor, and emojis.
- Explain new technical vocabulary the first time it appears.
- Prefer Python 3 and the `python3` command on macOS.
- Never include destructive Terminal commands in beginner exercises.
