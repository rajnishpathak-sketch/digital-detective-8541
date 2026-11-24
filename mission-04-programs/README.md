# Mission 4: How Programs Run

## Objective

To understand how programs are executed by computers, learn how to run a simple Python program using Terminal, and compare compilers and interpreters.

---

## Task 4.1: Create and Run a Python Program

### Program Created

File name: `hello.py`

```python
print("Hello from Python")
```

### Commands Used

```bash
cd mission-04-programs
touch hello.py
python3 hello.py
```

### Expected Output

```text
Hello from Python
```

### What I Learned

- A Python program can be written and saved in a `.py` file.
- Terminal can be used to execute Python programs.
- The `python3` command runs a Python program.
- The `print()` function displays a message in the Terminal.
- A program must be saved before running it so that the latest changes are executed.

### Tools Used

- Python 3
- Visual Studio Code
- macOS Terminal

---

## Task 4.2: Compare Compiler and Interpreter

A compiler and an interpreter are two approaches used to translate and execute programming languages.

### Comparison Table

| Point | Compiler | Interpreter |
|---|---|---|
| When translation / execution happens | Translates the program before execution | Translates and executes instructions during runtime |
| Typical output | Often produces machine code or an executable file | Usually executes the program without producing a separate executable |
| One example | C compiler (GCC) | Python interpreter |
| One advantage | Compiled programs generally execute faster | Easier to test and debug code during development |

### Difference Between Compiler and Interpreter

A compiler translates the source code into machine code or another lower-level form before the program is executed. An interpreter executes the program at runtime by translating and processing instructions. Compiled programs generally offer faster execution, while interpreted approaches make testing and development convenient. Both approaches are used to execute programs written in different programming languages.

---

## Overall Learning

Through this mission, I learned how to create a basic Python program and execute it using Terminal. I also understood the difference between a compiler and an interpreter, including when translation takes place and how both approaches execute programs.

## Difficulties Faced

- Understanding the difference between compilation and interpretation.
- Learning how to execute a Python file from the Terminal.

## Conclusion

This mission helped me understand the basic process of program execution. I learned how to create and run a Python program and gained an understanding of how compilers and interpreters work.

