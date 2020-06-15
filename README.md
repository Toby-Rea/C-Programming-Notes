# C Programming Notes <!-- omit in toc -->

## Table of contents <!-- omit in toc -->

- [Preface](#preface)
- [Fundamentals](#fundamentals)
- [Code Commenting](#code-commenting)
- [Variables](#variables)
- [Ternary Operator](#ternary-operator)
- [Escape Sequences](#escape-sequences)
- [Sources](#sources)

## Preface

Notes on the C programming language focused on the GCC. 

## Fundamentals

You'll need to write your own programs to learn to code because it allows you to apply your knowledge. Let's take a look at the "Hello World" program:

**Source Code:**

```c
#include <stdio.h>

int main() {
  printf("Hello World!\n");
  return 0;
}
```

**Output:**

```Hello World!```

**Explanation**

- `#include <stdio.h>` is a preprocessor directive which tells the compiler to include the `stdio.h` (standard input and output) library file in the program. This file contains the definitions of common Input/Output functions, such as `printf`.
- `int main()` is a function called `main()` with an integer return type. Every C program must have a `main()` function because the execution of the program begins there.
- `printf()` is a library function which prints formatted output to the terminal, and in this case, `printf("Hello World!\n")` will print `Hello World!`.
- `return 0` is known as the "Exit status" of the program. **0** reports successful execution, and terminates the execution. Other return values such as **1** could suggest errors.

## Code Commenting

Comments are important. They allow yourself and others to understand what your code does and why it does it. Comments are ignored by the compiler and therefore have no effect on the resulting object files. There are two types of comments:

- Single-line comments.
- Multi-line comments.

**Single-line comments**

Anything preceded by `//` up to the end of that line is considered a comment.

**Multi-line comments**

Anything preceded by `/*` and succeeded by `*/` is considered a comment.

## Variables

A variable is a named location in memory where we can manipulate data. Variables in C have their own specific type, which determines the size and layout of the variable's memory, and determines the operations which can be performed on the data.

| Basic Variable Type | Description                          |
| :-----------------: | :----------------------------------- |
|         int         | Integer.                             |
|        char         | Character represented as an integer. |
|        float        | Single-Precision floating point.     |
|       double        | Double-Precision floating point.     |
|        void         | Type absence.                        |

### Variable Declarations <!-- omit in toc -->

**Syntax:** `<data_type> <variable_name>;`

**Examples:**

```c
int cookies;
char letter;
float temperature;
```

### Variable Initializations <!-- omit in toc -->

**Syntax:** `<data_type> <variable-name> = <value>;`

**Examples:**

```c
int cookies = 12;
char letter = 'z';
float temperature = 27.2;
```

## Ternary Operator

Used in place of longer if / else statements.

`condition ? value_if_true : value_if_false`

**Example:**

```c
int c = (a < b) ? a : b;
```

**Explanation**

If a is less than b, the value of c is set to the value of a, otherwise, the value of c is set to b.

## Escape Sequences

Escape sequences are sequences of characters which don't represent themselves when used inside a string literal / character, typically used to provide literal representations of non-printing characters and characters that would otherwise have a special meaning, e.g. double quotation marks (").

| Escape Sequence | Represents        |
| :-------------: | :---------------- |
|       \0        | Null              |
|       \n        | New Line          |
|       \t        | Tab (Horizontal)  |
|       \v        | Tab (Vertical)    |
|       \\'       | Single Quote      |
|       \\"       | Double Quote      |
|       \\\       | Backslash         |
|       \\?       | Question Mark     |
|       \b        | Backspace         |
|       \a        | Alarm (Beep/Bell) |
|       \r        | Carriage Return   |

## Sources

- <https://www.javatpoint.com/escape-sequence-in-c> [Accessed 03-06-2020]
- <https://docs.microsoft.com/en-us/cpp/c-language/escape-sequences?view=vs-2019> [Accessed 03-06-2020]
- <https://www.programiz.com/c-programming/examples/print-sentence> [Accessed 04-06-2020]
- <https://beginnersbook.com/2017/09/c-hello-world-program> [Accessed 04-06-2020]
- <https://www.guru99.com/c-comments.html> [Accessed 04-06-2020]
- <https://www.geeksforgeeks.org/comments-in-c-c> [Accessed 04-06-2020]
- <https://www.tutorialspoint.com/cprogramming/c_variables.htm> [Accessed 05-06-2020]
- <https://www.studytonight.com/c/variables-in-c.php> [Accessed 05-06-2020]
- <https://www.freecodecamp.org/news/c-ternary-operator> [Accessed 15-06-2020]