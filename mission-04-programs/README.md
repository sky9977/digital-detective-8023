# Mission 4 — How programs run

## 1. Mission title

Mission 4 — How programs run

## 2. Task / objective

Run a simple Python program and compare how compilers and interpreters translate or execute programs.

## 3. Work completed

### Task 4.1 — Create and run a Python program

Created `hello.py` containing:

```python
print("Hello from Python")
```

Ran it using `python3 hello.py`. Terminal output:

```text
Hello from Python
```

### Task 4.2 — Compare compiler and interpreter

| Point | Compiler | Interpreter |
|---|---|---|
| When translation or execution happens | Translates the complete source program before execution | Reads and executes instructions while the program runs |
| Typical output | Machine code or a compiled executable | Immediate program output or runtime error |
| One example | C or C++ compiler implementations | Python interpreter implementations |
| One advantage | Compiled programs can execute quickly after compilation | Code can be changed and tested quickly without a separate compilation step |

In three or four sentences: A compiler translates source code into another form before the program runs, while an interpreter executes source instructions at runtime. A compiler commonly produces a separate executable or intermediate form, whereas an interpreter directly carries out instructions and reports problems as execution reaches them. Python implementations are commonly described as interpreted, although they can compile source to bytecode as part of their execution process. Real implementations can combine compilation and interpretation rather than following only one strict approach.

## 4. Commands / tools used

- Text editor — created `hello.py`.
- `python3 hello.py` — ran the Python program.
- Python 3 — interpreted the program and produced the displayed message.

## 5. My understanding

Python source code can be executed with the Python 3 interpreter. A compiler prepares code for later execution, while an interpreter executes instructions in sequence at runtime. The distinction describes typical behavior, but real language implementations may use both methods.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- `hello.py`
- Recorded Terminal output: `Hello from Python`

## 9. Commit details

- Commit message: `Compare compilers and interpreters`
- Status: Committed and pushed successfully to `main`.
