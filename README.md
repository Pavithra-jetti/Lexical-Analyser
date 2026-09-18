# Lexical Analyzer in C

## Overview

This project is a **Lexical Analyzer for the C programming language, developed in C**. It reads a C source file character by character and classifies its content into tokens such as keywords, identifiers, operators, literals, and symbols — printing each token along with its line number.

The project demonstrates the practical use of **file handling, character-level parsing, arrays, and string manipulation** in C, and models the tokenizing phase of a compiler.

## Features

* Identifies preprocessor directives (e.g. `#include`)
* Skips single-line (`//`) and multi-line (`/* */`) comments
* Recognizes character literals (`'a'`) and string literals (`"text"`)
* Detects numeric constants
* Classifies identifiers, data-type keywords, and non-data keywords separately
* Recognizes operators and symbols
* Tracks and reports mismatched round `()` and curly `{}` braces
* Reports the line number for every token detected
* Color-coded console output for readability

## Technologies Used

* **Programming Language:** C
* **Compiler:** GCC
* **Platform:** Linux / Windows
* **Concepts:** File Handling, Character-by-Character Parsing, Arrays, String Handling, Compiler Design Basics
* **Libraries:** `stdio.h`, `stdlib.h`, `string.h`, `ctype.h`

## Project Structure

```text
Lexical-Analyzer-in-C/
│
├── main.c
├── function.c
├── header.h
├── sample.c
├── README.md
└── .gitignore
```

### File Description

| File         | Description                                                             |
| ------------ | ----------------------------------------------------------------------- |
| `main.c`     | Core lexer logic; reads the source file and classifies each token       |
| `function.c` | Helper functions for identifying keywords, operators, and symbols       |
| `header.h`   | Keyword/operator/symbol tables, color macros, and function declarations |
| `sample.c`   | Sample C source file used as input to test the lexical analyzer         |
| `README.md`  | Project documentation                                                   |
| `.gitignore` | Specifies generated files that should not be uploaded to GitHub         |

## How to Run

### 1. Clone the Repository

Open **Command Prompt / Terminal** and run:

```bash
git clone <your-github-repository-link>
```

### 2. Open the Project Directory

```bash
cd Lexical-Analyzer-in-C
```

### 3. Compile the Program

```bash
gcc main.c function.c -o a.out
```

### 4. Run the Program

```bash
./a.out sample.c
```

## Run

The analyzer takes a `.c` file as a command-line argument and prints each token it finds:

```text
./a.out <source_file.c>
```

Example output:

```text
Line  1 : Preprocessor directive     : #include <stdio.h>
Line  3 : Data-type keyword          : int
Line  3 : Identifier                 : main
...
Successfully parsed
```

If braces are unbalanced or a literal is left unclosed, the analyzer reports the specific error and stops.

## Learning Outcomes

* Gained practical understanding of how compilers tokenize source code
* Learned character-by-character file parsing techniques in C
* Practiced classifying tokens such as keywords, identifiers, literals, operators, and symbols
* Improved understanding of arrays, string handling, and control flow in C
* Learned to detect and report syntax issues like unbalanced braces
* Practiced modular programming using `.c` and `.h` files
* Improved debugging and problem-solving skills

## Author

**Pavithra Jetti**
