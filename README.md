# C Programming Notes

## Table of contents <!-- omit in toc -->

- [C Programming Notes](#c-programming-notes)
  - [Preface](#preface)
  - [Fundamentals](#fundamentals)
  - [Code Commenting](#code-commenting)
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
