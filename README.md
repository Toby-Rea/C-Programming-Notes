# C Programming Notes

## Table of contents <!-- omit in toc -->

- [C Programming Notes](#c-programming-notes)
  - [Preface](#preface)
  - [Fundamentals](#fundamentals)
  - [Escape Sequences](#escape-sequences)
  - [Sources](#sources)

## Preface

Notes on the C programming language focused on the GCC. 

## Fundamentals

You'll need to write your own programs to learn to code because this allows you to apply your knowledge. Let's take a look at the "Hello World" program:

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
