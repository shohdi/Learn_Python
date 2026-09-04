# Lecture 1: Files, Folders, and the macOS Terminal 🗂️

**Estimated time:** 15 minutes  
**Level:** Complete beginner  
**Goal:** Understand files and folders, open Terminal, move around the computer, and create and copy items safely.

## 1. Meet the computer's filing cabinet (3 minutes) 🗄️

A **file** is a named piece of stored information. A photo, a song, a Python program, and a text document are all files.

Examples:

- `cat.jpg` — an image file
- `shopping_list.txt` — a text file
- `hello.py` — a Python file

The part after the final dot is called the **file extension**. It helps us and the computer recognize the file's type. Renaming `cat.jpg` to `cat.py` does not turn the cat into a programmer. Sadly. 🐈‍⬛

A **folder** (also called a **directory**) is a container that organizes files and other folders. For example:

```text
Documents/
└── PythonCourse/
    ├── notes.txt
    └── exercises/
```

A **path** is the address of a file or folder. For example:

```text
/Users/sara/Documents/PythonCourse/notes.txt
```

The `/` separates the folders in the address.

## 2. What is Terminal? (3 minutes) 💻

The **Terminal** is an application that lets us control the computer by typing commands instead of clicking icons. It is like texting your Mac, except your Mac is extremely literal and never understands sarcasm. 😄

To open it on a Mac:

1. Press `Command (⌘) + Space`.
2. Type `Terminal`.
3. Press `Return`.

You will see a line waiting for a command. This is called the **command prompt**.

Try these safe commands:

```bash
pwd
ls
```

- `pwd` means **print working directory**. It shows your current location.
- `ls` means **list**. It shows what is inside the current folder.

Useful navigation commands:

```bash
cd Documents
cd ..
cd ~
```

- `cd Documents` enters the `Documents` folder.
- `cd ..` goes up to the parent folder.
- `cd ~` returns to your home folder.

> **Tip:** Terminal commands and names are case-sensitive. `Documents` and `documents` may not mean the same thing.

## 3. Creating files and folders (3 minutes) ✨

Create a folder with `mkdir` (**make directory**):

```bash
mkdir python_course
```

Create an empty file with `touch`:

```bash
touch notes.txt
```

Names containing spaces need quotation marks:

```bash
mkdir "Python Course"
touch "day one.txt"
```

You can check your work with:

```bash
ls
```

## 4. Copying files and folders (2 minutes) 🐑

Copy a file using `cp` (**copy**):

```bash
cp notes.txt notes_backup.txt
```

Copy a file into another folder:

```bash
cp notes.txt python_course/
```

Copy an entire folder using `cp -R` (**recursive copy**):

```bash
cp -R python_course python_course_backup
```

The `-R` tells Terminal to copy the folder and everything inside it. A folder has children, grandchildren, and occasionally 4,000 mysterious screenshots. 📸

> **Safety note:** A copy command can replace an existing file with the same destination name. Use `ls` to inspect the destination first.

## 5. Solved examples (4 minutes) ✅

### Example 1: Build a course folder

**Task:** Go to the home folder, create `python_course`, enter it, and create `notes.txt`.

```bash
cd ~
mkdir python_course
cd python_course
touch notes.txt
ls
```

Expected final output includes:

```text
notes.txt
```

### Example 2: Create a backup

**Task:** Copy `notes.txt` and name the copy `notes_backup.txt`.

```bash
cp notes.txt notes_backup.txt
ls
```

Expected result:

```text
notes.txt  notes_backup.txt
```

### Example 3: Copy a whole project folder

Assume `python_course` is inside `Documents`.

```bash
cd ~/Documents
cp -R python_course python_course_backup
ls
```

Now `Documents` contains both folders. The original remains unchanged.

## Unsolved exercises 🧠

Do not peek at imaginary answers—the exercises are intentionally unsolved!

1. Open Terminal and display your current location.
2. Go to your `Documents` folder and list its contents.
3. Create a folder named `coding_practice`.
4. Enter that folder and create two files: `ideas.txt` and `commands.txt`.
5. Copy `ideas.txt` to a new file named `ideas_backup.txt`.
6. Return to `Documents` and copy the entire `coding_practice` folder to `coding_practice_backup`.
7. **Challenge:** Create a folder named `My Python Work` using quotation marks, then create `lesson one.txt` inside it.

## Quick recap 🎯

- A **file** stores information.
- A **folder/directory** organizes files and folders.
- A **path** is an item's address.
- Terminal accepts typed commands.
- `pwd`, `ls`, and `cd` help us navigate.
- `mkdir` and `touch` create folders and files.
- `cp` copies a file; `cp -R` copies a folder.

Next: What programming languages are, how their main types differ, and why Python is so popular. 🐍
