# Hands-on C

C is a general-purpose, procedural, and case-sensitive programming language developed in the early 1970s by Dennis Ritchie at Bell Labs. It is considered one of the most influential languages in computer science history and is often referred to as the "mother of all modern programming languages."

## Table of Contents

1. [Introduction](#introduction)
1. [Comments in C](#comments-in-c)
1. [Keywords in C](#keywords-in-c)
1. [Escape sequences](#escape-sequences)
1. [Variables](#variables)
1. [Input and Output](#input-and-output)
1. [Data Types & Format Specifiers](#data-types--format-specifiers)
1. [Operators](#operators)
1. [Control Structures](#control-structures)
1. [Functions](#functions)
1. [Functions](#functions)
1. [Strings](#strings)
1. [Arrays](#arrays)
1. [Pointers](#pointers)
1. [Structures and Unions](#structures-and-unions)
1. [Dynamic Memory Allocation](#dynamic-memory-allocation)
1. [File Handling](#file-handling)
1. [Preprocessor Directives](#preprocessor-directives)
1. [Error Handling](#error-handling)

## Introduction

### Key Features

- **Procedural Language:** Emphasizes functions and step-by-step procedures.

- **Low-level Access:** Offers direct memory manipulation using pointers.

- **Portability:** C programs can be compiled and run on many types of machines with minimal changes.

- **Efficient Performance:** Known for its speed and close-to-hardware behavior.

- **Rich Library Support:** Comes with a standard library for I/O, string manipulation, memory allocation, etc.

- **Modular Code:** Code can be organized into functions for reusability and clarity.

### Why C is Important

- **Foundation Language:** Languages like C++, Java, C#, and even Python are influenced by C.

- **Operating Systems:** Core components of OSs like Linux, Windows, and macOS are written in C.

- **Embedded Systems:** Used extensively in firmware and microcontroller programming.

- **Compilers & Interpreters:** Many compilers (e.g., GCC) and interpreters are themselves written in C.

### Basic Example

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

### Essential Toolkit for C Learning

#### Method 1: Text Editor or IDE

- **VS Code (Editor):** Lightweight, with C extensions (`C/C++` by Microsoft)
- **Code::Blocks (IDE):** Beginner-friendly, pre-configured

#### Method 2: C Compiler

- **GCC (GNU Compiler Collection):** Most popular, open-source

#### Method 3: Online Compilers (for quick practice)

- [Code Chef](https://www.codechef.com/ide)

#### Learning Resources

- [Problem-Solving Practices](https://github.com/msa-iqbal/c-plus-plus-code-solutions)

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Comments in C

In **C language**, comments are used to explain the code and make it more readable. Comments are ignored by the compiler, so they don’t affect program execution.

**Single-line Comment:**

```c
// This is a single-line comment
int x = 10;  // This sets x to 10
```

**Multi-line Comment:**

```c
/* This is a multi-line comment
   It can span multiple lines
*/
int y = 20;
```

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Keywords in C

Keywords are reserved words in C language that have special, predefined meanings. They cannot be used as identifiers, such as variable names, function names, or label names, because they are an essential part of the C syntax and grammar.

**C language keyword list (based on the C99 standard, which is very widely used):**

| No. | Keyword    | No. | Keyword    | No. | Keyword    | No. | Keyword          |
| --: | ---------- | --: | ---------- | --: | ---------- | --: | ---------------- |
|   1 | `auto`     |  14 | `for`      |  27 | `long`     |  40 | `void`           |
|   2 | `break`    |  15 | `goto`     |  28 | `register` |  41 | `volatile`       |
|   3 | `case`     |  16 | `if`       |  29 | `restrict` |  42 | `while`          |
|   4 | `char`     |  17 | `inline`   |  30 | `return`   |  43 | `_Bool`          |
|   5 | `const`    |  18 | `int`      |  31 | `short`    |  44 | `_Complex`       |
|   6 | `continue` |  19 | `long`     |  32 | `signed`   |  45 | `_Imaginary`     |
|   7 | `default`  |  20 | `restrict` |  33 | `sizeof`   |  46 | `_Alignas`       |
|   8 | `do`       |  21 | `signed`   |  34 | `static`   |  47 | `_Alignof`       |
|   9 | `double`   |  22 | `sizeof`   |  35 | `struct`   |  48 | `_Atomic`        |
|  10 | `else`     |  23 | `static`   |  36 | `switch`   |  49 | `_Generic`       |
|  11 | `enum`     |  24 | `struct`   |  37 | `typedef`  |  50 | `_Noreturn`      |
|  12 | `extern`   |  25 | `typedef`  |  38 | `union`    |  51 | `_Static_assert` |
|  13 | `float`    |  26 | `union`    |  39 | `unsigned` |  52 | `_Thread_local`  |

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Escape sequences

Escape sequences (also known as **backslash character constants**) are special character combinations that begin with a backslash (`\`). They are used to represent characters that cannot be typed directly or have special meaning in strings or characters.

**List of Common Escape Sequences in C:**

| Escape Sequence | Meaning                           | Example in Code              | Output          |
| --------------- | --------------------------------- | ---------------------------- | --------------- |
| `\n`            | New line                          | `printf("Hello\nWorld");`    | Hello<br>World  |
| `\t`            | Horizontal tab                    | `printf("Hello\tWorld");`    | Hello  World    |
| `\b`            | Backspace                         | `printf("Helloo\b!");`       | Hello!          |
| `\r`            | Carriage return                   | `printf("Hello\rWorld");`    | World           |
| `\f`            | Form feed (page break)            | _Rarely used_                | —               |
| `\a`            | Alert (bell sound)                | `printf("\a");`              | 🔔 (beep sound) |
| `\\`            | Backslash                         | `printf("\\");`              | `\`             |
| `\'`            | Single quote                      | `printf("\'");`              | `'`             |
| `\"`            | Double quote                      | `printf("\"");`              | `"`             |
| `\?`            | Question mark                     | `printf("\?");`              | `?`             |
| `\0`            | Null character (end of string)    | _Used in string terminators_ | —               |
| `\ooo`          | Octal number (e.g., `\141` = 'a') | `printf("\141");`            | `a`             |
| `\xhh`          | Hexadecimal (e.g., `\x61` = 'a')  | `printf("\x61");`            | `a`             |

**Example:**

```c
#include <stdio.h>

int main() {
    printf("Line1\nLine2\n");      // newline
    printf("Tab\tSpace\n");        // tab
    printf("Backslash: \\\n");     // backslash
    printf("Quote: \' \" \n");     // single and double quote
    printf("Beep\a\n");            // beep (if supported)
    return 0;
}
```

**💡 Notes:**

- Escape sequences are used in both **character** (`'\n'`) and **string** (`"\n"`) literals.
- They are vital for **text formatting**, **controlling output**, and representing special characters.
- Some (like `\f`, `\a`) may not have visible effects in modern terminals, but they are still standard.

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Variables

A **variable** is a **named memory location** used to store a value that can be changed during program execution.

- Acts as a **storage unit** for data.
- Must be **declared** with a data type before use.
- The value of a variable **can be changed** during program execution.

**Syntax:**

```c
<data_type> <variable_name>;
<data_type> <variable_name> = value;
```

**Example:**

```c
int age;         // Declaration
age = 25;        // Assignment
float pi = 3.14; // Declaration + Assignment
```

### Rules for Naming Variables

| Rule No. | Rule                                                            |
| -------: | --------------------------------------------------------------- |
|        1 | Must begin with a **letter** (A–Z or a–z) or **underscore `_`** |
|        2 | Can include **letters, digits (0–9), and underscores**          |
|        3 | **Cannot start with a digit**                                   |
|        4 | **Cannot use C keywords** (like `int`, `return`, etc.)          |
|        5 | **Case-sensitive** (`Age` and `age` are different)              |
|        6 | Should be **meaningful** (use descriptive names)                |

### Types of Variables

| Type         | Description                                                     | Scope          |
| ------------ | --------------------------------------------------------------- | -------------- |
| **Local**    | Declared inside a function/block                                | Function/block |
| **Global**   | Declared outside all functions, accessible by all functions     | Whole program  |
| **Static**   | Retains value between function calls, has local scope           | Block/function |
| **Extern**   | Declared in one file, defined in another file (shared globally) | Global         |
| **Register** | Suggests storing variable in a CPU register (faster access)     | Local          |

**Example (Different Variable Types):**

```c
#include <stdio.h>

int globalVar = 10; // Global variable

void function() {
    static int staticVar = 0; // Static variable
    staticVar++;
    printf("Static: %d\n", staticVar);
}

int main() {
    int localVar = 5; // Local variable

    printf("Global: %d\n", globalVar);
    printf("Local: %d\n", localVar);

    function();
    function();

    return 0;
}
```

**Output:**

```markdown
Global: 10
Local: 5
Static: 1
Static: 2
```

### Constants vs Variables

| Feature      | Variable                    | Constant                     |
| ------------ | --------------------------- | ---------------------------- |
| Value change | Can change during execution | Cannot change after assigned |
| Declaration  | `int age = 20;`             | `const int age = 20;`        |

**💡 Notes:**

- Variable values are stored in **RAM**.
- Use `const` for **read-only** values.
- Initialize variables to **avoid garbage values**.
- Use meaningful names for better **code readability**.

**Example - ✅ Good Practice:**

```c
int studentAge = 20;
float temperature = 36.6;
char grade = 'A';
```

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Input and Output

C uses **standard input/output functions** provided by the `stdio.h` header file for data communication between the user and the program.

**Header File:**

```c
#include <stdio.h>
```

All input/output operations in C require the `stdio.h` header file.

### Output

**`printf()` – Formatted Output**

- Used to display output to the screen.
- Supports format specifiers like `%d`, `%f`, `%c`, etc.

**Syntax:**

```c
printf("format string", variables);
```

**Example:**

```c
int age = 20;
printf("Age is %d", age);  // Output: Age is 20
```

### Input

**`scanf()` – Formatted Input**

- Used to read input from the user.
- Requires **address-of operator (`&`)** for variables (except strings).

**Syntax:**

```c
scanf("format string", &variables);
```

**Example:**

```c
int age;
scanf("%d", &age);
```

### Format Specifiers (Common)

| Data Type      | Format Specifier | Used With         |
| -------------- | ---------------- | ----------------- |
| `int`          | `%d`, `%i`       | `scanf`, `printf` |
| `float`        | `%f`             | `scanf`, `printf` |
| `double`       | `%lf`            | `scanf`, `printf` |
| `char`         | `%c`             | `scanf`, `printf` |
| `string`       | `%s`             | `scanf`, `printf` |
| `unsigned int` | `%u`             | `scanf`, `printf` |
| `long int`     | `%ld`            | `scanf`, `printf` |
| `pointer`      | `%p`             | `printf` only     |

**Example (Input and Output Program):**

```c
#include <stdio.h>

int main() {
    int age;
    float salary;
    char initial;
    char name[50];

    // Input
    printf("Enter your age: ");
    scanf("%d", &age);

    printf("Enter your salary: ");
    scanf("%f", &salary);

    printf("Enter your first initial: ");
    scanf(" %c", &initial);  // Space before %c to ignore newline

    printf("Enter your name: ");
    scanf("%s", name);  // no & for string input

    // Output
    printf("\n--- OUTPUT ---\n");
    printf("Age: %d\n", age);
    printf("Salary: %.2f\n", salary);
    printf("Initial: %c\n", initial);
    printf("Name: %s\n", name);

    return 0;
}
```

**💡 Notes:**

- `scanf("%s", str)` reads only a **single word** (no spaces). Use `fgets()` for full-line input.
- `printf()` does not require the address-of operator.
- Be careful with buffer issues when mixing `scanf()` with `gets()` or `fgets()`.

### Other I/O Functions

| Function    | Purpose                           |
| ----------- | --------------------------------- |
| `getchar()` | Reads a single character          |
| `putchar()` | Outputs a single character        |
| `gets()`    | Reads a string (⚠️ unsafe, avoid) |
| `puts()`    | Outputs a string with newline     |
| `fgets()`   | Reads a string safely (preferred) |
| `fprintf()` | Outputs to a file stream          |
| `fscanf()`  | Inputs from a file stream         |

**Example: `fgets()` and `puts()`**

```c
char name[100];
printf("Enter your full name: ");
fgets(name, sizeof(name), stdin);
puts("Hello,");
puts(name);
```

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Data Types & Format Specifiers

**Data types** specify the type of data a variable can hold. Different **format specifiers** are used in **printf** and **scanf** to handle the input and output of these data types.

#### **Basic Data Types:**

- **`char`**: Stores a single character.
  - Size: 1 byte
  - Range: `-128` to `127` (signed) or `0` to `255` (unsigned)
- **`int`**: Stores integer values.

  - Size: 2 or 4 bytes (depending on system architecture)
  - Range: `-32,768` to `32,767` (16-bit) or `-2^31` to `2^31 - 1` (32-bit)

- **`float`**: Stores single-precision floating point numbers.

  - Size: 4 bytes
  - Range: `1.2E-38` to `3.4E+38`

- **`double`**: Stores double-precision floating point numbers.

  - Size: 8 bytes
  - Range: `2.3E-308` to `1.7E+308`

- **`void`**: Represents an absence of data. It is used in functions that do not return a value.

#### **Derived Data Types:**

- **`array`**: Collection of elements of the same type.
- **`pointer`**: A variable that stores the memory address of another variable.
- **`struct`**: Collection of variables of different data types.
- **`union`**: Collection of variables that share the same memory location.
- **`enum`**: A user-defined data type with a set of named integer constants.

### **Modifiers**

Modifiers alter the range of fundamental data types.

- **`signed`**: Allows negative numbers.
- **`unsigned`**: Disallows negative numbers, expanding the positive range.
- **`long`**: Increases the range of `int` and `double`.
- **`short`**: Reduces the size of `int` to save memory.

### **Format Specifiers in C**

**For `printf` (Output)**

| Data Type      | Format Specifier | Example                      | Output         |
| -------------- | ---------------- | ---------------------------- | -------------- |
| `char`         | `%c`             | `printf("%c", 'A');`         | A              |
| `int`          | `%d`, `%i`       | `printf("%d", 25);`          | 25             |
| `float`        | `%f`             | `printf("%f", 3.14);`        | 3.140000       |
| `double`       | `%lf`            | `printf("%lf", 3.141592);`   | 3.141592       |
| `unsigned int` | `%u`             | `printf("%u", 123);`         | 123            |
| `long`         | `%ld`            | `printf("%ld", 1234567890);` | 1234567890     |
| `short`        | `%hd`            | `printf("%hd", 25);`         | 25             |
| `string`       | `%s`             | `printf("%s", "Hello");`     | Hello          |
| `pointer`      | `%p`             | `printf("%p", &x);`          | 0x7ffdfd9cdbd0 |

**For `scanf` (Input)**

| Data Type      | Format Specifier | Example               |
| -------------- | ---------------- | --------------------- |
| `char`         | `%c`             | `scanf("%c", &ch);`   |
| `int`          | `%d`, `%i`       | `scanf("%d", &num);`  |
| `float`        | `%f`             | `scanf("%f", &num);`  |
| `double`       | `%lf`            | `scanf("%lf", &num);` |
| `unsigned int` | `%u`             | `scanf("%u", &num);`  |
| `long`         | `%ld`            | `scanf("%ld", &num);` |
| `short`        | `%hd`            | `scanf("%hd", &num);` |
| `string`       | `%s`             | `scanf("%s", str);`   |
| `pointer`      | `%p`             | `scanf("%p", &ptr);`  |

**Example:**

```c
#include <stdio.h>

int main() {
    int x = 10;
    float pi = 3.14159;

    // Using format specifiers
    printf("Integer: %d\n", x);   // %d for int
    printf("Float: %f\n", pi);    // %f for float
    printf("Pointer: %p\n", &x);  // %p for pointer
    return 0;
}
```

**💡 Notes:**

- `%d` and `%i` can be used interchangeably for integers in **printf** and **scanf**.
- `%lf` is used for **double** in **printf** but can be used as `%f` in **scanf**.
- The `long` and `short` modifiers help control the size and range of data types in C.
- The `%p` specifier is used to print the address of a variable (pointer).

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Operators

Operators in C are **symbols** used to perform operations on **variables and values**.

**Types of Operators:**

### **Arithmetic Operators**

Used for mathematical operations.

| Operator | Meaning             | Example | Result       |
| -------- | ------------------- | ------- | ------------ |
| `+`      | Addition            | `a + b` | 10 + 5 = 15  |
| `-`      | Subtraction         | `a - b` | 10 - 5 = 5   |
| `*`      | Multiplication      | `a * b` | 10 \* 5 = 50 |
| `/`      | Division            | `a / b` | 10 / 5 = 2   |
| `%`      | Modulus (remainder) | `a % b` | 10 % 3 = 1   |

### **Relational (Comparison) Operators**

Used to compare two values.

| Operator | Meaning          | Example  | Result    |
| -------- | ---------------- | -------- | --------- |
| `==`     | Equal to         | `a == b` | false (0) |
| `!=`     | Not equal to     | `a != b` | true (1)  |
| `>`      | Greater than     | `a > b`  | true (1)  |
| `<`      | Less than        | `a < b`  | false (0) |
| `>=`     | Greater or equal | `a >= b` | true (1)  |
| `<=`     | Less or equal    | `a <= b` | false (0) |

### **Logical Operators**

Used to combine multiple conditions.

| Operator | Meaning     | Example           | Result               |
| -------- | ----------- | ----------------- | -------------------- |
| `&&`     | Logical AND | `a > 5 && b < 10` | true if both true    |
| `┃┃`     | Logical OR  | `a > 5 ┃┃ b < 10` | true if any one true |
| `!`      | Logical NOT | `!(a > 5)`        | reverses result      |

### **Assignment Operators**

Used to assign values.

| Operator | Meaning             | Example  | Equivalent To |
| -------- | ------------------- | -------- | ------------- |
| `=`      | Assign              | `a = 10` | —             |
| `+=`     | Add and assign      | `a += 5` | `a = a + 5`   |
| `-=`     | Subtract and assign | `a -= 5` | `a = a - 5`   |
| `*=`     | Multiply and assign | `a *= 2` | `a = a * 2`   |
| `/=`     | Divide and assign   | `a /= 2` | `a = a / 2`   |
| `%=`     | Modulus and assign  | `a %= 3` | `a = a % 3`   |

### **Increment / Decrement Operators**

Increase or decrease a value by 1.

| Operator | Meaning   | Example | Description                       |
| -------- | --------- | ------- | --------------------------------- |
| `++`     | Increment | `a++`   | Post-increment (use then add)     |
| `--`     | Decrement | `--a`   | Pre-decrement (subtract then use) |

### **Bitwise Operators**

Operate on binary digits.

| Operator | Meaning     | Example  |
| -------- | ----------- | -------- |
| `&`      | AND         | `a & b`  |
| `┃`      | OR          | `a  ┃ b` |
| `^`      | XOR         | `a ^ b`  |
| `~`      | NOT         | `~a`     |
| `<<`     | Left shift  | `a << 1` |
| `>>`     | Right shift | `a >> 1` |

### **Conditional (Ternary) Operator**

A shorthand for `if-else`.

```c
condition ? expression_if_true : expression_if_false;
```

**Example:**

```c
int a = 10, b = 20;
int max = (a > b) ? a : b;
```

### **Sizeof Operator**

Returns size of a variable or data type.

**Example:**

```c
printf("%zu", sizeof(int));  // Output: 4
```

### **Comma Operator**

Evaluates multiple expressions, returns the last.

**Example:**

```c
int x = (a = 5, b = 10);  // x = 10
```

### **Pointer Operators**

Used for pointer operations.

| Operator | Meaning     | Example |
| -------- | ----------- | ------- |
| `*`      | Dereference | `*ptr`  |
| `&`      | Address-of  | `&var`  |

**Example:**

```c
#include <stdio.h>

int main() {
    int a = 5, b = 2;

    printf("Addition: %d\n", a + b);
    printf("Greater? %d\n", a > b);
    printf("AND logic: %d\n", (a > 0) && (b > 0));
    printf("Bitwise AND: %d\n", a & b);
    printf("Ternary Max: %d\n", (a > b) ? a : b);

    return 0;
}
```

### 🕮 Summary Table

| Category            | Examples                       |
| ------------------- | ------------------------------ |
| Arithmetic          | `+`, `-`, `*`, `/`, `%`        |
| Relational          | `==`, `!=`, `>`, `<`, `>=`     |
| Logical             | `&&`, `┃┃`, `!`                |
| Assignment          | `=`, `+=`, `-=`, `*=`          |
| Increment/Decrement | `++`, `--`                     |
| Bitwise             | `&`, `┃`, `^`, `~`, `<<`, `>>` |
| Ternary             | `condition ? true : false`     |
| Sizeof              | `sizeof(var)`                  |
| Comma               | `(a = 5, b = 6)`               |
| Pointer             | `*`, `&`                       |

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Control Structures

Control structures in C determine the **flow of execution** of the program — **which blocks of code get executed** and when.

**Types of Control Structures:**

1. **Conditional Statements (Decision-making)**
2. **Looping Statements (Iteration)**
3. **Jump Statements (Branching)**

### **Conditional Statements**

Used to **execute code based on conditions**.

**`if` Statement**

```c
if (condition) {
    // code to execute if condition is true
}
```

**`if-else` Statement**

```c
if (condition) {
    // if true
} else {
    // if false
}
```

**`else-if` Ladder**

```c
if (condition1) {
    // block 1
} else if (condition2) {
    // block 2
} else {
    // default block
}
```

**Nested `if`**

```c
if (condition1) {
    if (condition2) {
        // block
    }
}
```

**Switch-case**

Used for multiple constant values.

```c
switch (expression) {
    case constant1:
        // code
        break;
    case constant2:
        // code
        break;
    default:
        // default code
}
```

### **Looping Statements**

Used to **repeat a block of code** multiple times.

**`for` Loop**

```c
for (initialization; condition; increment) {
    // code block
}
```

**`while` Loop**

```c
while (condition) {
    // code block
}
```

**`do-while` Loop**

```c
do {
    // code block
} while (condition);
```

💡 Executes at least once even if condition is false.

### **Jump Statements**

Used to **control the flow** of loops and functions.

| Keyword    | Description                                       |
| ---------- | ------------------------------------------------- |
| `break`    | Exits loop or switch block                        |
| `continue` | Skips rest of the loop for current iteration      |
| `goto`     | Jumps to a labeled part of the program (⚠️ avoid) |
| `return`   | Exits from a function                             |

**Example (break):**

```c
for (int i = 1; i <= 10; i++) {
    if (i == 5)
        break;
    printf("%d ", i);
}
```

**Example (continue):**

```c
for (int i = 1; i <= 5; i++) {
    if (i == 3)
        continue;
    printf("%d ", i);
}
```

### 🕮 Summary Table

| Structure   | Type      | Keywords Used                                        |
| ----------- | --------- | ---------------------------------------------------- |
| Conditional | Decision  | `if`, `else`, `else if`, `switch`, `case`, `default` |
| Looping     | Iteration | `for`, `while`, `do-while`                           |
| Jump        | Branching | `break`, `continue`, `goto`, `return`                |

**Example:**

```c
#include <stdio.h>

int main() {
    int num = 5;

    // Conditional
    if (num > 0)
        printf("Positive\n");

    // Looping
    for (int i = 1; i <= num; i++) {
        if (i == 3)
            continue;
        if (i == 5)
            break;
        printf("%d\n", i);
    }

    // switch-case
    switch (num) {
        case 1: printf("One\n"); break;
        case 5: printf("Five\n"); break;
        default: printf("Other\n");
    }

    return 0;
}
```

**Output:**

```markdown
Positive
1
2
4
Five
```

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Functions

A **function** in C is a **block of code** that performs a specific task. It helps in organizing code, avoiding repetition, and improving reusability.

> Real-life analogy to understand function:
>
> > A function in C is like a coffee machine — you press a button (input), it brews coffee (process), and gives you a cup (output).

### **Types of Functions**

1. **Built-in (Library) Functions:** Provided by C libraries.  
   Examples: `printf()`, `scanf()`, `strlen()`, `sqrt()`
2. **User-defined Funtions:** Created by the programmer.

### **Function Syntax & Components:**

**Function Syntax:**

```c
return_type function_name(parameter_list) {
    // function body
    return value; // optional
}
```

**The Function Components are -**

- **Function Declaration**
- **Function Definition**
- **Function Call**

**Function Declaration:**  
Tells the compiler about the function's name, return type, and parameters — before it is used.

```c
int add(int a, int b);  // Declaration
```

- Return type: `int`

- Function name: `add`

- Parameters: `int a, int b`

_💡 Think of this as informing the compiler: “Hey! I’ll use a function like this later.”_

**Function Definition**  
Contains the actual **code (body)** that runs when the function is called.

```c
int add(int a, int b) {
    return a + b;
}
```

- This is where the logic of **addition** is implemented.

**Function Call**

Used to **invoke/execute** the function and get the result.

```c
int result = add(3, 5);  // Function call
```

- Passes arguments `3` and `5` to the function

- Stores the returned value in `result`

**Full Example with All Components**

```c
#include <stdio.h>

// 1. Function Declaration
int add(int a, int b);

int main() {
    // 3. Function Call
    int sum = add(10, 20);
    printf("Sum = %d\n", sum);
    return 0;
}

// 2. Function Definition
int add(int a, int b) {
    return a + b;
}
```

**Output:**

```markdown
Sum = 30
```

### Some more examples

**Example (No return, no parameters):**

```c
#include <stdio.h>

void greet() {
    printf("Hello, World!\n");
}

int main() {
    greet();
    return 0;
}
```

**Output:**

```markdown
Hello, World!
```

**Example (With return, with parameters):**

```c
#include <stdio.h>

int add(int a, int b) {
    return a + b;
}

int main() {
    int sum = add(4, 5);
    printf("Sum = %d\n", sum);
    return 0;
}
```

**Output:**

```markdown
Sum = 9
```

**Example (Function Declaration (Prototype)):**

```c
#include <stdio.h>

int multiply(int, int); // function declaration

int main() {
    printf("Result = %d\n", multiply(3, 4));
    return 0;
}

int multiply(int x, int y) {
    return x * y;
}
```

**Output:**

```markdown
Result = 12
```

### Return Types in C Functions

| Return Type | Meaning             | Example           |
| ----------- | ------------------- | ----------------- |
| `void`      | No return value     | `void show()`     |
| `int`       | Returns integer     | `int getSum()`    |
| `float`     | Returns float value | `float avg()`     |
| `char`      | Returns a character | `char getGrade()` |

### Parameter Types

| Type               | Example                 | Description                      |
| ------------------ | ----------------------- | -------------------------------- |
| No Parameters      | `void greet(void)`      | Takes no input                   |
| With Parameters    | `int sum(int a, int b)` | Takes input values               |
| Default (Not in C) | ❌                      | C doesn’t support default params |
| Variable Arguments | `int printf(...)`       | Use `stdarg.h`                   |

### Recursive Function

A recursive function is a function that calls itself to solve smaller versions of a problem.

> Real-life analogy to understand function:
>
> > Like opening a set of nested boxes — each box opens the next, until the smallest box is reached.

```c
#include <stdio.h>

int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);
}

int main() {
    printf("Factorial of 5 = %d\n", factorial(5));
    return 0;
}
```

**Output:**

```markdown
Factorial of 5 = 120
```

### 🕮 Function Categories Summary

| Function Type              | Parameters | Return Value | Example                   |
| -------------------------- | ---------- | ------------ | ------------------------- |
| No Parameters, No Return   | No         | No           | `void greet(void)`        |
| With Parameters, No Return | Yes        | No           | `void greet(char name[])` |
| No Parameters, With Return | No         | Yes          | `int getTime(void)`       |
| With Parameters and Return | Yes        | Yes          | `int add(int a, int b)`   |

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Strings

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Arrays

An **array** in C is a **collection of elements** of the same data type stored in **contiguous memory locations**.

> Real-life analogy to understand array:
>
> > An array is like a bookshelf, where each shelf slot holds one book and you can find any book by its position number.

**Syntax:**

```c
data_type array_name[array_size];
```

💡 All elements must be of the **same type**.

**Example:**

```c
#include <stdio.h>

int main() {
    int numbers[5] = {10, 20, 30, 40, 50};

    printf("First number: %d\n", numbers[0]);  // index 0
    printf("Third number: %d\n", numbers[2]);  // index 2

    return 0;
}
```

💡 Note: For Example highlighting, specify the language immediately after the first set of triple backticks. If no Example highlighting is required, use markdown after the triple backticks (recommended).

**Output:**

```markdown
First number: 10
Third number: 30
```

**💡 Notes:**

- **Index starts at `0`:** First element is `array[0]`
- **Fixed size:** Size is defined at creation
- **Same type:** All elements must be of the same data type

**Array Accessing Diagram**

```plaintext
Index:     0    1    2    3    4
Value:    10   20   30   40   50
           ↑         ↑
     numbers[0]  numbers[2]
```

**Types of Arrays**

1. Linear or 1D Arrays
2. Multi-Dimensional:
   1. Matrix or 2D Array
   2. 3D Array

### Linear or 1D Array

A single-dimensional array is the simplest form of an array. It is a **linear collection of elements** of the same data type, accessible using a single index.

**Syntax:**

```c
datatype array_name [array_size];             // array declaration

datatype array_name [array_size] = {value};  // array initialization

array_name [index];                          // accessing array elements
```

**Example (1D Array):**

```c
#include <stdio.h>

int main() {
    int numbers[5] = {10, 20, 30, 40, 50};

    for (int i = 0; i < 5; i++) {
        printf("%d ", numbers[i]);
    }

    return 0;
}
```

**Output:**

```markdown
10 20 30 40 50
```

### **Matrix or 2D Arrays**

A two-dimensional array in C is an array of arrays, which can be visualized as a matrix with rows and columns.

**Syntax:**

```c
// array declaration
datatype array_name [rows] [columns];

// array initialization
datatype array_name [row_size] [column_size] = {

    {column1, column2, column3},   // total: 2 row and 3 columns
    {column1, column2, column3}
};

// accessing array elements
datatype variable_name = array_name [rows] [columns];
```

**Explanation:**

- **`type`**: The data type of the array elements (e.g., `int`, `float`).
- **`rows`**: The number of rows in the array.
- **`columns`**: The number of columns in the array.

**Example:**

```c
#include <stdio.h>

int main() {

    // 2D Array Declaration and Initialization
    int matrix[3][4] = {
        {1, 2, 3, 4},
        {5, 6, 7, 8},
        {9, 10, 11, 12}
    };

    // Accessing a Value from a Specific Index
    int element = matrix[1][2];  // 2nd row, 3rd column → value is 7

    printf("Access Single Element: %d\n\n", element);

    // Printing all elements of the 2D array
    printf("Matrix Elements:\n");
    for (int i = 0; i < 3; i++) {          // rows
        for (int j = 0; j < 4; j++) {      // columns
            printf("%2d ", matrix[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

**Output:**

```markdown
Access Single Element: 7

Matrix Elements:
1 2 3 4
5 6 7 8
9 10 11 12
```

**Visual Representation:**

```plaintext
      Columns →
        0   1   2   3
Rows ↓
  0     1   2   3   4
  1     5   6   7   8
  2     9  10  11  12
```

### 3D Array

A three-dimensional array can be visualized as an array of 2D arrays. It's like having multiple matrices stacked together.

**Syntax:**

```c
// array declaration
datatype array_name [size1] [size2] [size3];

// array initialization
datatype array_name [numOf_2D_Array] [rowSize_each2D] [columnSize_each2D] = {

    {
        {column1, column2, column3},   // total: 2 row and 3 columns
        {column1, column2, column3}
    },
    {
        {column1, column2, column3},   // total: 2 row and 3 columns
        {column1, column2, column3}
    }
};

// accessing array elements
datatype variable_name = array_name [size1] [size2] [size3];
```

**Explanation:**

- **`size1`**: The size of the first dimension (number of 2D arrays).
- **`size2`**: The size of the second dimension (number of rows in each 2D array).
- **`size3`**: The size of the third dimension (number of columns in each 2D array).

**💡 Notes:**

- **Fixed Size:** The size of each dimension must be specified at compile time (except for the first dimension, which can sometimes be omitted in the declaration if the array is initialized).

- **Memory Layout:** Multi-dimensional arrays are stored in a contiguous block of memory. For a 2D array, the elements are stored row by row.

- **Access:** Elements are accessed using multiple indices, one for each dimension.

**Example:**

```c
#include <stdio.h>

int main() {

    int arr[2][3][4] = {  // A 3D array with 2 "planes," each with 3 rows & 4 columns.
        {
            {1, 2, 3, 4},
            {5, 6, 7, 8},
            {9, 10, 11, 12}
        },
        {
            {13, 14, 15, 16},
            {17, 18, 19, 20},
            {21, 22, 23, 24}
        }
    };

    // Accessing Value from Specific Index
    int element = arr[1][2][3];
    // Accesses the element in the 2nd plane, 3rd row, 4th column (value is 24)

    printf("Access Single Element: %d\n\n", element); //

    // Printing all elements of the 3D array
    for (int i = 0; i < 2; i++) {
        printf("Plane %d:\n", i);
        for (int j = 0; j < 3; j++) {
            for (int k = 0; k < 4; k++) {
                printf("%2d ", arr[i][j][k]);
            }
            printf("\n");
        }
        printf("\n");
    }

    return 0;
}
```

**Output:**

```markdown
Access Single Element: 24

Plane 0:
1 2 3 4
5 6 7 8
9 10 11 12

Plane 1:
13 14 15 16
17 18 19 20
21 22 23 24
```

### Array Initialization

| Method                         | Syntax Example                   |
| ------------------------------ | -------------------------------- |
| Full initialization            | `int arr[3] = {1, 2, 3};`        |
| Partial initialization         | `int arr[3] = {1}; // {1, 0, 0}` |
| Zero initialization            | `int arr[3] = {0};`              |
| Size inferred from initializer | `int arr[] = {1, 2, 3, 4};`      |

**Example (Input from User):**

```c
#include <stdio.h>

int main() {
    int a[5];

    printf("Enter 5 numbers: ");
    for (int i = 0; i < 5; i++) {
        scanf("%d", &a[i]);
    }

    printf("You entered: ");
    for (int i = 0; i < 5; i++) {
        printf("%d ", a[i]);
    }

    return 0;
}
```

**Output (if input = 1 2 3 4 5):**

```markdown
Enter 5 numbers: You entered: 1 2 3 4 5
```

### Accessing and Modifying Array Elements

```c
arr[2] = 100;  // modifies the 3rd element
int x = arr[0];  // gets the 1st element
```

**Example (Sum of Array Elements):**

```c
#include <stdio.h>

int main() {
    int a[5] = {1, 2, 3, 4, 5};
    int sum = 0;

    for (int i = 0; i < 5; i++) {
        sum += a[i];
    }

    printf("Sum = %d\n", sum);
    return 0;
}
```

**Output:**

```markdown
Sum = 15
```

## 🔹 Passing Arrays to Functions

```c
void printArray(int arr[], int size) {
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
}
```

Call it with:

```c
printArray(numbers, 5);
```

### **Array of Pointers**

An array of pointers holds memory addresses, and each element of the array is a pointer to a variable or another array.

**Example:**

```c
#include <stdio.h>

int main() {

    int numbers[] = {10, 20, 30, 40, 50};
    int *ptrs[5]; // Array of 5 integer pointers

    // Assign pointers to elements of the numbers array
    for (int i = 0; i < 5; i++) {
        ptrs[i] = &numbers[i];
    }

    // Access elements using pointers
    for (int i = 0; i < 5; i++) {
        printf("Element %d: %d\n", i + 1, *ptrs[i]);
    }

    return 0;
}
```

**Output:**

```markdown
Element 1: 10
Element 2: 20
Element 3: 30
Element 4: 40
Element 5: 50
```

**Multi-Dimensional Arrays of Pointers**
These arrays are arrays of pointers that can be used to manage more complex data structures, such as arrays of arrays where each sub-array can be of different sizes.

**Example:**

```c
#include <stdio.h>
int main() {

    int numbers[3][4] = {{1, 2, 3, 4}, {5, 6, 7, 8}, {9, 10, 11, 12}};
    int *ptrs[3][4];

    // Assign pointers to elements of the numbers array
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 4; j++) {
            ptrs[i][j] = &numbers[i][j];
        }
    }

    // Access elements using pointers
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 4; j++) {
            printf("Element [%d][%d]: %d\n", i, j, *ptrs[i][j]);
        }
    }

    return 0;
}
```

**Output:**

```markdown
Element [0][0]: 1
Element [0][1]: 2
Element [0][2]: 3
Element [0][3]: 4
Element [1][0]: 5
Element [1][1]: 6
Element [1][2]: 7
Element [1][3]: 8
Element [2][0]: 9
Element [2][1]: 10
Element [2][2]: 11
Element [2][3]: 12
```

<!-- dgdfgfdgfdgfdg -->

# 📦 Arrays and Strings in C

In C, **arrays** are collections of data of the same type stored in contiguous memory. **Strings** are special character arrays that end with a null character `'\0'`.

---

## 🔹 Arrays in C

### 🔸 Syntax

```c
data_type array_name[size];
```

---

### 🔸 Types of Arrays

| Type          | Description                   | Example              |
| ------------- | ----------------------------- | -------------------- |
| 1D Array      | Linear collection             | `int nums[5];`       |
| 2D Array      | Table-like (matrix)           | `int matrix[3][3];`  |
| Multi-D Array | More than 2 dimensions (rare) | `int data[2][3][4];` |

---

### 🔸 Example: 1D Array

```c
#include <stdio.h>

int main() {
    int arr[5] = {1, 2, 3, 4, 5};
    for (int i = 0; i < 5; i++) {
        printf("%d ", arr[i]);
    }
    return 0;
}
```

**🔸 Output:**

```
1 2 3 4 5
```

---

### 🔸 Example: 2D Array

```c
#include <stdio.h>

int main() {
    int mat[2][2] = {{1, 2}, {3, 4}};
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            printf("%d ", mat[i][j]);
        }
        printf("\n");
    }
    return 0;
}
```

**🔸 Output:**

```
1 2
3 4
```

---

## 🔹 Strings in C

Strings are arrays of characters ending with the null character `'\0'`.

### 🔸 Declaration

```c
char str[6] = {'H', 'e', 'l', 'l', 'o', '\0'};
char str[] = "Hello";  // automatically null-terminated
```

---

### 🔸 Example: Basic String Input and Output

```c
#include <stdio.h>

int main() {
    char name[20];
    printf("Enter your name: ");
    scanf("%s", name);  // input without spaces
    printf("Hello, %s!\n", name);
    return 0;
}
```

**🔸 Output (if input is `John`):**

```
Enter your name: John
Hello, John!
```

---

### 🔸 Example: Using `gets()` and `puts()` (⚠️ not recommended due to buffer overflow)

```c
#include <stdio.h>

int main() {
    char str[50];
    gets(str);         // unsafe, use fgets instead
    puts(str);
    return 0;
}
```

---

### 🔸 Recommended: Using `fgets()`

```c
#include <stdio.h>

int main() {
    char str[50];
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    printf("You entered: %s", str);
    return 0;
}
```

---

## 🔹 String Functions (`<string.h>`)

| Function        | Description                      | Example                 |
| --------------- | -------------------------------- | ----------------------- |
| `strlen(s)`     | Returns length                   | `strlen("Hi") → 2`      |
| `strcpy(d, s)`  | Copies string `s` into `d`       | `strcpy(dest, src)`     |
| `strcat(d, s)`  | Concatenates `s` to `d`          | `strcat(dest, src)`     |
| `strcmp(s1,s2)` | Compares two strings             | Returns 0 if equal      |
| `strrev(s)`     | Reverses a string (non-standard) | `strrev("abc") → "cba"` |

---

## 🔸 Example: String Length

```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "Hello";
    printf("Length = %lu\n", strlen(str));
    return 0;
}
```

**🔸 Output:**

```
Length = 5
```

---

## 🔹 Difference Between Arrays and Strings

| Feature       | Arrays        | Strings                        |
| ------------- | ------------- | ------------------------------ |
| Type          | Any data type | Only `char` type               |
| Termination   | No terminator | Ends with `'\0'`               |
| Header Needed | None          | Use `<string.h>` for functions |

---

## 🧪 Example: Character Access in String

```c
#include <stdio.h>

int main() {
    char str[] = "World";
    printf("%c\n", str[1]);  // prints 2nd character
    return 0;
}
```

**🔸 Output:**

```
o
```

---

Would you like to cover **pointer and array/string relationships** next?

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Pointers

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Structures and Unions

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Dynamic Memory Allocation

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## File Handling

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Preprocessor Directives

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Error Handling

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Advanced Topics

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Data Structures in C

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Common Mistakes and Best Practices

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Practice Problems and Projects

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->

## Appendix: Reference Links and Resources

<!-- START "Jump to Top"-->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ▲</a>
</p>
<!-- END "Jump to Top" -->
````
