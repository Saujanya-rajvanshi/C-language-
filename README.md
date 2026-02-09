# C-language-

### Index - C Programming

- [History of C](#history-of-c)
- [Features of C](#Features)
- [Basics](#basics)
- [Header Files](#header)
- [Data Handling](#Data-Handling)
- [Flow of Control](#flow-of-control)
- [Functions](#functions)
- [Arrays](https://github.com/Saujanya-rajvanshi/Arrays-)
- [Pointers](#pointers)
- [Dynamic Memory Allocation](#dynamic-memory-allocation)
- [Structures & Unions](#structures-unions)
- [Object-Oriented Programming (OOP)](https://github.com/Saujanya-rajvanshi/THEORY?tab=readme-ov-file#Oops)
- [Exception Handling](#exception-handling)
- [File Handling](#file-handling)
- [Templates](#templates)
- [STL (Standard Template Library)](https://github.com/Saujanya-rajvanshi/STL)
- [Advanced C++ Concepts](#advanced-concept)
- [Competitive Programming / DSA Readiness](#competitive-programming)
- [string manipulation](#string-manipulation)
- [basic maths codes](https://github.com/Saujanya-rajvanshi/basic-maths)

---











###### history of c
# 🎗 HISTORY

* C is a procedural, general-purpose programming language.
* It was developed by Dennis Ritchie in 1972 at Bell Laboratories (AT&T).
* C was designed mainly for system programming and to implement UNIX.
* By 1973, the UNIX operating system was mostly rewritten in C.
* C overcame limitations of B and BCPL, such as lack of data types and weak structure.
* It is widely used because it is memory-efficient, portable, and offers low-level control.
* Dennis Ritchie and Brian Kernighan authored *The C Programming Language* (K&R).
* The K&R book established the standard syntax and semantics of C.

<img width="1042" height="745" alt="image" src="https://github.com/user-attachments/assets/ea14c032-6b0e-45cd-94d7-c0b11ab615b8" />

| **C Standard**       | **Year**    | **Key Features / Changes**                                                                                                                                |
| -------------------- | ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ANSI C (C89/C90)** | 1989 / 1990 | Introduced function prototypes, standard libraries, formal libraries, and stricter type checking. Approved by ANSI (C89) and ISO (C90).                   |
| **C99**              | 1999        | Added inline functions, variable-length arrays, complex numbers, `long long` data type, single-line comments (`//`), and improved floating-point support. |
| **C11**              | 2011        | Focused on safety and concurrency; introduced generic programming, multithreading support (`threads.h`), and Unicode support.                             |
| **C17 / C18**        | 2017        | Minor revision of C11; fixed bugs and clarified ambiguities, with no major new features.                                                                  |
| **C23**              | 2023        | Latest standard; introduced features like `nullptr`, binary literals, and improved support for modern hardware architectures.                             |


---

###### Features
# 🎗 FEATURES

###### Applications
* **Operating Systems:** Used in UNIX, Linux, Windows, and macOS for kernels, drivers, and system utilities.
* **Embedded Systems:** Widely used in microcontrollers, IoT devices, automotive systems, and Arduino due to hardware-level control.
* **Compilers & Interpreters:** Used to build GCC and Python’s CPython interpreter for speed and portability.
* **Databases:** Backend of databases like SQLite, MySQL, and PostgreSQL for fast data processing.
* **Networking:** Used in TCP/IP stacks, web servers (Apache, Nginx), and network drivers.
* **Game Development:** Handles performance-critical tasks like graphics and physics in game engines.
* **Scientific Computing:** Used in simulations and high-performance libraries like BLAS.
* **Real-Time Systems:** Essential in aerospace, medical devices, robotics, and industrial automation for precise timing.

###### Features
* **Simple**: Easy to learn and use.
* **Structured**: Uses functions for modular programming.
* **Portable**: Programs can run on different systems.
* **Fast**: Compiled language; high performance.
* **Rich library**: Standard library for I/O, string, math, etc.
* **Low-level access**: Can manipulate memory using pointers.

---
















###### basics
## 🎗 BASICS 
- [character set](#character-set)
- [tokens](#Tokens)
- [Barebones of C Program](#barebones-of-C-program)
- [Data Types (overview)](#Data-Types-Overview)
- [Variables & Constants](#Variables-Constants)
- [Type Modifiers](#Type-Modifiers)
- [Type Conversion Type Casting](#Type-Conversion-Type-Casting)
- [sizeof operator](#sizeof-operator)
- [Comments](#Comments)
- [data handling](#data-handling-basics)
- [boiler plate code](#boile-plate-code)
- [next line](#next-line)
- [Escape Sequences](#Escape-Sequences)
- [output & input](#output-and-input)

## character set
✅ **NO difference**
* **Letters:** A–Z, a–z
* **Digits :** 0–9
* **Special symbols:** `+  -  *  /  %  =  <  >  !  &  |  ^  ~  ?  :  ;  ,  .  '  "  #  $  @  _  ( )  { }  [ ]
* **Whitespace characters:** space, tab (`\t`), newline (`\n`), carriage return (`\r`)

## Tokens
 Tokens are the **smallest units** of a C++ program.
* **Keywords:** -> less than c++
* **Identifiers:** -> same as c++
* **Constants (literals):** -> 0 , 1 and null
* **Operators:** -> same as c++
*  **Separators (punctuators):** -> same as c++

### 💎 KEYWORDS

### ❌ NOT in C (C++ only)
* bool
* wchar_t
* class, public, private, protected
* this, new, delete
* virtual, override, final, friend
* dynamic_cast, static_cast, reinterpret_cast, const_cast
* template, typename, namespace, export
* try, catch, throw, noexcept
* inline (limited in C), constexpr, decltype
* operator (overloading)
* nullptr, true, false
* asm (C has asm but compiler-dependent)

### ✅ Present in C
* int, float, double, char, void
* if, else, for, while, switch
* break, continue, goto, return
* auto, register, static, extern
* const, volatile, typedef, sizeof
* struct, union, enum

📌 **Keyword count**

* **C ≈ 32 keywords**
* **C++ ≈ 95 keywords (C++20)**

### 💎 IDENTIFIER

✅ **NO difference**
Rules are **exactly same** in C and C++.

### 💎 LITERALS

❌ C++ only
* Boolean literals → `true`, `false`
* Null pointer literal → `nullptr`

✅ C
* Uses `0` or `NULL` instead of `nullptr`
* Boolean handled using `int` (0 or 1)

##### **INTEGER LITERALS**
❌ C++ only
* **Binary literals** → `0b1010`
✅ C
* Decimal, Octal, Hexadecimal only

##### **FLOATING-POINT**
✅ **NO difference**
* float, double, long double
* IEEE-754 format
* Precision rules same

##### **CHARACTER LITERALS**
✅ **NO difference**
* char type
* ASCII values
* Escape sequences same

### 💎 STRING

❌ C++ only
* `string` (STL)
* `<string>` header
* Functions like `length()`, `append()`

✅ C
* Strings are **character arrays**

```c
char str[20] = "Hello";
```

* Uses `<string.h>` functions: `strlen`, `strcpy`


### 💎 BOOLEAN

❌ C++ only
* `bool` type
* `true` / `false`

✅ C
* Uses `int`

```c
int flag = 1; // true
```

### 💎 NULL POINTER

❌ C++ only
* `nullptr`

✅ C
* Uses `NULL` or `0`

```c
int *p = NULL;
```

### 💎 OPERATORS
❌ C++ only
* `::` scope resolution
* `->` with classes
* Operator overloading

✅ C
* No scope resolution
* No operator overloading
* Basic arithmetic, logical, bitwise same

### 💎 PUNCTUATORS
❌ C++ only
* `::`
* `...` (limited use in C via stdarg)

✅ C
* `; { } ( ) [ ] #`


## Barebones of C program
✅ **NO difference**

### 🔹 Program Structure

* Execution starts from **`main()`**.
* **Statements** end with `;`.

### 🔹 Expressions

* **Produce a value**.
* Examples: `a + b`, `x > 5`.

### 🔹 Statements

* **Perform actions**.
* Examples:

  * Declaration: `int x;`
  * Assignment: `x = 5;`
  * Conditional: `if (x > 0) {...}`
  * Output: `cout << x;`

### 🔹 Comments

* **Single-line:** `// comment`
* **Multi-line:**

```c
/* comment 
   continues here */
```

### 🔹 Blocks

* Defined using `{ }`.
* **Same braces → same scope** (variables inside are local).

---

## Data Types Overview
✅ **NO difference**

## Variables Constants

### Variables

* **True:** A variable stores data whose value can change, while a constant stores fixed data.

* **Declaration vs Definition:**

  * **Declaration:** Tells the compiler about the variable’s type and name.

    ```c
    extern int x; // declaration only
    ```
  * **Definition:** Allocates memory for the variable.

    ```c
    int x; // definition
    ```

* **Initialization vs Assignment:**

  * **Initialization:** Giving a value when defining:

    ```c
    int x = 10; // initialization
    ```
  * **Assignment:** Giving/changing a value later:

    ```c
    x = 20; // assignment
    ```

* **Scope:**

  * **Local:** Inside a function/block.
  * **Global:** Outside all functions.
  * **Block:** Same as local in a block `{ }`.
  * **Namespace:** ❌ Not in C (namespace is C++ feature).

* **Lifetime & Storage Duration:**

  * **Automatic:** Local variables, disappear after function ends.
  * **Static:** Retains value between function calls.
  * **Dynamic:** Allocated via `malloc()`.
  * **Register:** Suggests storing in CPU register (rarely used).

* **Linkage:**

  * **Internal (`static`)**: Visible only in the file.
  * **External (`extern`)**: Shared across files.

### Constants

* **`const`** → Read-only after initialization. ✅ Supported in C.
* **`constexpr`** → ❌ **C++ only**, not in C.
* **`volatile`** → Value may change unexpectedly, often used with hardware registers. ✅ Supported in C.
* **`mutable`** → ❌ **C++ only**, not in C.

So in **C**, everything is correct **except `namespace`, `constexpr`, and `mutable`** — they are **C++ features**.

---

## Type Modifiers 

Type modifiers also change **range** and **storage size** in C.

### Common Modifiers (C)

* `short`
* `long`
* `long long`
* `signed`
* `unsigned`

### Validity in C

* Modifiers must be applied to **integer types** (`int`, `char`)
* `long long` is valid **from C99 onward**
* `signed` / `unsigned` work with `char`, `short`, `int`, `long`, `long long`

## Type Conversion Type Casting 

Type conversion changes one data type into another.

#### Implicit Conversion

* Done automatically by compiler
* Happens during expressions
* May cause **data loss**

```c
int a = 5;
float b = a;   // implicit
```

#### Explicit Conversion

* Programmer controlled
* Done using **C-style casting only**

```c
float x = 5.6;
int y = (int)x;
```

#### Casting Types in C

* **Only C-style cast** available
* Syntax: `(type)expression`

📌 C does **not support**:

* `static_cast`
* `const_cast`
* `reinterpret_cast`
* `dynamic_cast`

#### Important Concepts

* Narrowing conversions possible
* No user-defined conversions
* No conversion constructors
* No `explicit` keyword in C


## sizeof Operator 

`sizeof` is a **compile-time operator** used to find memory size.

#### Key Points

* Returns value in bytes
* Result type is `size_t`
* `sizeof(array)` gives total array size
* `sizeof(pointer)` gives pointer size
* Structure padding affects result
* No side effects
* `sizeof(char) == 1`

📌 Example:

```c
int a;
printf("%zu", sizeof(a));
```


## Comments (C)

Comments are used to **explain code** and are ignored by the compiler.

#### Types

* **Single-line:** `//`  (C99 onwards)
* **Multi-line:** `/* */`

📌 Nested comments are **not allowed**



## Data Handling 

**Data handling** means storing, reading, modifying, and managing data in a program.

* Data is stored using **variables**

* Data types define stored data:

  * `int` → integers
  * `float / double` → decimal values
  * `char` → single character
  * `char[]` → strings

* Operations on data:

  * Assignment (`=`)
  * Arithmetic (`+ - * / %`)
  * Comparison (`== != < > <= >=`)

* Proper data handling avoids:

  * Overflow
  * Undefined behavior
  * Type mismatch errors

📌 Example:

```c
int age = 20;
float price = 99.5;
```


## Boiler Plate Code (C)

**Boilerplate code** is the **minimum required code** to run a C program.

### Standard C boilerplate:

```c
#include <stdio.h>

int main() {
    return 0;
}
```

### Explanation:

* `#include <stdio.h>` → input/output
* `int main()` → program execution starts here
* `return 0;` → successful program termination

📌 `using namespace std;` ❌ **not used in C**


## Next Line 

To move output to the **next line**, C uses:

### `\n`

```c
printf("Hello\n");
```

📌 `endl` ❌ **not available in C**


## Escape Sequences 

Escape sequences are **special character combinations** used inside **character and string literals**.

They start with a **backslash (`\`)**.

### Common Escape Sequences

| Escape | Meaning         |
| ------ | --------------- |
| `\n`   | New line        |
| `\t`   | Horizontal tab  |
| `\v`   | Vertical tab    |
| `\b`   | Backspace       |
| `\r`   | Carriage return |
| `\f`   | Form feed       |
| `\a`   | Alert (beep)    |
| `\\`   | Backslash       |
| `\'`   | Single quote    |
| `\"`   | Double quote    |
| `\0`   | Null character  |

### Numeric Escape Sequences

* **Octal** → `\nnn`
* **Hexadecimal** → `\xhh`

📌 Unicode escapes ❌ **not standard in C**

---

### Important Concepts

* Used in `' '` and `" "`
* Interpreted at compile time
* `\0` marks end of C strings
* Invalid sequences → warnings or undefined behavior


## Output & Input 

### Output → `printf()`

Used to display output.

```c
printf("Hello World");
printf("%d", x);
```

### Input → `scanf()`

Used to take input from user.

```c
scanf("%d", &x);
scanf("%d %d", &a, &b);
```

### Important rules:

* Format specifiers are mandatory
* Address operator `&` required
* Strings need character arrays

📌 Example:

```c
int n;
scanf("%d", &n);
printf("Value: %d", n);
```

---










###### header
# 🎗 Header Files (C)

Header files are files with extension .h that contain function declarations, macros, constants, and data type definitions.

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <math.h>
```

* Headers usually end with `.h`
* C headers **do not contain classes**

## Why Header Files Are Used

* Separate **declaration** from **definition**
* Avoid code duplication
* Enable modular programming
* Improve readability and maintenance
* Allow sharing of functions across files

📌 **Rule:**

> Function definitions are written in `.c` files, declarations in `.h` files.


### ❌ Namespaces

* **Namespaces are NOT supported in C**
* `using namespace std;` ❌ not allowed
* No `std::` prefix

📌 Reason: C does not support OOP or name scoping via namespaces


### ❌ Scope Resolution Operator `::`

* `::` ❌ **NOT available in C**
* Cannot access:

  * namespace members
  * class static members

📌 Global variables accessed directly by name


## Including Header Files

Header files are included using **`#include`** (preprocessor directive).

### 1️. System Header Files

```c
#include <stdio.h>
#include <stdlib.h>
```

* Written inside `< >`
* Provided by compiler
* Stored in system directories

### 2️. User-Defined Header Files

```c
#include "myfile.h"
```

* Written inside `" "`
* Searched in current directory first
* Created by programmer


## Common Standard Header Files

| Header File | Purpose                        |
| ----------- | ------------------------------ |
| `stdio.h`   | Input / Output functions       |
| `stdlib.h`  | Memory allocation, conversions |
| `string.h`  | String handling functions      |
| `math.h`    | Mathematical functions         |
| `ctype.h`   | Character testing              |
| `time.h`    | Date & time                    |
| `limits.h`  | Data type limits               |
| `float.h`   | Floating-point limits          |
| `stdbool.h` | Boolean type (C99)             |
| `assert.h`  | Debugging                      |

## What Header Files Contain

Header files may contain:

* Function **prototypes**
* `#define` macros
* `typedef` declarations
* `struct`, `union`, `enum` definitions
* Global constants (`const`)

📌 **Should NOT contain:**

* Function definitions (except inline/macros)
* Variable definitions

## Example of User-Defined Header

### `mathutils.h`

```c
#ifndef MATHUTILS_H
#define MATHUTILS_H

int add(int a, int b);
int sub(int a, int b);

#endif
```

### `mathutils.c`

```c
#include "mathutils.h"

int add(int a, int b) {
    return a + b;
}
```

### `main.c`

```c
#include <stdio.h>
#include "mathutils.h"

int main() {
    printf("%d", add(2,3));
    return 0;
}
```

## Header Guards

Header guards prevent **multiple inclusion errors**.

### Syntax

```c
#ifndef FILE_NAME_H
#define FILE_NAME_H

// declarations

#endif
```

📌 Prevents:

* Redefinition errors
* Multiple compilation issues

## Preprocessor Directives Used in Headers

| Directive      | Purpose               |
| -------------- | --------------------- |
| `#include`     | Include files         |
| `#define`      | Macros                |
| `#ifndef`      | If not defined        |
| `#ifdef`       | If defined            |
| `#endif`       | End condition         |
| `#pragma once` | Alternative to guards |

## `#pragma once`

```c
#pragma once
```

* Ensures file included only once
* Compiler-specific but widely supported
* Simpler than header guards

## Difference: Header vs Source File

| Header (.h)  | Source (.c)    |
| ------------ | -------------- |
| Declarations | Definitions    |
| Shared       | Compiled       |
| No main()    | Contains logic |

## Important Exam Points ⭐

* Header files are processed by **preprocessor**
* They do **not produce object code**
* Order of inclusion matters
* Circular inclusion causes errors
* Header files improve modularity

## Common Mistakes ❌

* Defining variables in headers
* Missing header guards
* Including `.c` files
* Multiple definitions
* Wrong include path


## C Standard Header Files 

| Header File       | Purpose                    | Important Functions / Contents                                                                                                            |
| ----------------- | -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| **`stdio.h`**     | Standard input/output      | `printf()`, `scanf()`, `getchar()`, `putchar()`, `gets()`, `puts()`, `fopen()`, `fclose()`, `fprintf()`, `fscanf()`, `fgets()`, `fputs()` |
| **`stdlib.h`**    | General utilities          | `malloc()`, `calloc()`, `realloc()`, `free()`, `exit()`, `atoi()`, `atof()`, `rand()`, `srand()`, `system()`                              |
| **`string.h`**    | String handling            | `strlen()`, `strcpy()`, `strcat()`, `strcmp()`, `strncpy()`, `strncat()`, `strncmp()`, `strchr()`, `strstr()`                             |
| **`math.h`**      | Mathematical functions     | `sqrt()`, `pow()`, `sin()`, `cos()`, `tan()`, `log()`, `log10()`, `ceil()`, `floor()`, `fabs()`                                           |
| **`ctype.h`**     | Character handling         | `isalpha()`, `isdigit()`, `isalnum()`, `isspace()`, `islower()`, `isupper()`, `tolower()`, `toupper()`                                    |
| **`time.h`**      | Date & time                | `time()`, `clock()`, `difftime()`, `ctime()`, `localtime()`, `strftime()`                                                                 |
| **`limits.h`**    | Integer limits             | `INT_MAX`, `INT_MIN`, `CHAR_MAX`, `CHAR_MIN`, `LONG_MAX`                                                                                  |
| **`float.h`**     | Floating-point limits      | `FLT_MAX`, `FLT_MIN`, `DBL_MAX`, `DBL_MIN`                                                                                                |
| **`assert.h`**    | Debugging                  | `assert()`                                                                                                                                |
| **`errno.h`**     | Error handling             | `errno`, error macros                                                                                                                     |
| **`setjmp.h`**    | Non-local jumps            | `setjmp()`, `longjmp()`                                                                                                                   |
| **`signal.h`**    | Signal handling            | `signal()`, `raise()`                                                                                                                     |
| **`stdarg.h`**    | Variable arguments         | `va_start()`, `va_arg()`, `va_end()`                                                                                                      |
| **`stdbool.h`**   | Boolean support (C99)      | `bool`, `true`, `false`                                                                                                                   |
| **`stddef.h`**    | Common definitions         | `size_t`, `ptrdiff_t`, `NULL`, `offsetof()`                                                                                               |
| **`stdint.h`**    | Fixed-width integers       | `int8_t`, `int16_t`, `int32_t`, `uint32_t`                                                                                                |
| **`inttypes.h`**  | Integer formatting         | `printf` macros for `stdint`                                                                                                              |
| **`locale.h`**    | Localization               | `setlocale()`, `localeconv()`                                                                                                             |
| **`wchar.h`**     | Wide characters            | `wprintf()`, `wcscpy()`, `wcslen()`                                                                                                       |
| **`wctype.h`**    | Wide char classification   | `iswalpha()`, `towlower()`                                                                                                                |
| **`complex.h`**   | Complex numbers            | `creal()`, `cimag()`, `csqrt()`                                                                                                           |
| **`tgmath.h`**    | Type-generic math          | Generic math macros                                                                                                                       |
| **`fenv.h`**      | Floating-point environment | `feclearexcept()`, `feraiseexcept()`                                                                                                      |
| **`stdalign.h`**  | Alignment (C11)            | `alignas`, `alignof`                                                                                                                      |
| **`stdatomic.h`** | Atomic operations (C11)    | `atomic_int`, atomic functions                                                                                                            |
| **`threads.h`**   | Multithreading (C11)       | `thrd_create()`, `mtx_lock()`                                                                                                             |
| **`uchar.h`**     | Unicode characters         | `char16_t`, `char32_t`                                                                                                                    |

---













###### Data Handling
# 🎗 Data Handling (C)

### 🔹 Strings

❌ C does **not** have `string` data type

```c
char name[20];
```

* Uses `char[]`
* Requires `<string.h>`
* Manual memory handling

---

### 🔹 Boolean Type

* `bool` ❌ **not native in C (before C99)**

```c
#include <stdbool.h>
bool flag = true;
```

📌 In old C:

* `0` → false
* `1` → true

---

### 🔹 Mutable / Immutable

* No concept of immutability by default
* Only achievable using `const`
* No string immutability like C++ STL

---

### ❌ References

* References (`int &x`) ❌ **not supported**
* Only pointers are available

---

### ❌ Classes

* `class` ❌ **not supported**
* Use `struct` only
* No access specifiers (`private`, `public`)

---

### ❌ `using` keyword

* `using` for type alias ❌ not available
* Use `typedef`

```c
typedef unsigned int uint;
```

---













###### flow of control
# 🎗 FLOW OF CONTROL (C)

### ✅ Same Flow Control Structures

These are **identical** in C and C++:

* `if`
* `if-else`
* `switch`
* `for`
* `while`
* `do-while`
* `break`
* `continue`
* `goto`
* `return`
* Ternary operator `?:`


### ❌ switch limitations

* `switch` in C supports:

  * `int`
  * `char`
* ❌ No `enum class` (C++ only)
* ❌ No `string` in switch


### ❌ Range-based for loop

* **Not supported in C**

```cpp
for (int x : arr)  // C++ only
```


### ❌ Boolean conditions

* No `true` / `false` keywords (pre-C99)
* Conditions rely on:

  * `0` → false
  * non-zero → true

---














###### functions
# 🎗 FUNCTION
### ✅ SAME in C

* Function definition & declaration
* Function call
* Return type
* Void functions
* Call by value
* Recursion
* Advantages of functions
* Call stack concept

### ❌ REMOVE / CHANGE for C

| C++ Feature in Your Notes    | Status in C     | What to Do           |
| ---------------------------- | --------------- | -------------------- |
| Call by reference (`int &x`) | ❌ Not supported | Use pointers instead |
| Default arguments            | ❌ Not supported | Remove completely    |
| Inline keyword               | ❌ Not standard  | Remove               |
| Function overloading         | ❌ Not supported | Remove               |
| Compile-time polymorphism    | ❌ Not supported | Remove               |
| Reference-based passing      | ❌ Not available | Use pointer-based    |

### ✅ C Replacement Example

```c
void fun(int *x);   // instead of int &x
```

📌 **Exam Line (C):**

> C supports only **call by value** and **call by address (pointer)**.

---










###### pointers
# 🎗 POINTERS

### ✅ SAME in C

* Pointer declaration & initialization
* Dereferencing
* Null pointer
* Void pointer
* Wild pointer
* Dangling pointer
* Pointer arithmetic
* Pointer & arrays
* Pointer to pointer
* Call by reference using pointers
* Advantages & disadvantages
* Common mistakes

### ❌ REMOVE / CHANGE for C

| C++ Feature         | Status in C     |
| ------------------- | --------------- |
| `nullptr`           | ❌ Not available |
| Smart pointers      | ❌ Not available |
| References (`int&`) | ❌ Not available |
| `new` / `delete`    | ❌ Not available |

### ✅ C Version

```c
int *p = NULL;   // use NULL, not nullptr
```

📌 **Exam Line (C):**

> C uses **raw pointers only**, no automatic memory management.

---












###### dynamic memory allocation
# 🎗 DYNAMIC MEMORY ALLOCATIONS 

### ✅ SAME in C

* Runtime allocation
* Heap memory
* Stack vs Heap concept
* Use in data structures
* Common errors (memory leak, dangling pointer)
* Advantages & disadvantages

### ❌ REMOVE / CHANGE for C

| C++ Feature                     | Status in C     |
| ------------------------------- | --------------- |
| `new`                           | ❌ Not supported |
| `delete`                        | ❌ Not supported |
| Constructors/destructors        | ❌ Not supported |
| Smart pointers                  | ❌ Not supported |
| Exception on allocation failure | ❌ Not supported |

### ✅ C Replacement

```c
int *p = (int*)malloc(sizeof(int));
free(p);
```

### Dynamic Array (C)

```c
int *arr = (int*)malloc(n * sizeof(int));
free(arr);
```

📌 **Exam Line (C):**

> C uses `malloc`, `calloc`, `realloc`, and `free` for dynamic memory.

---

###### structures and unions
# 🎗 STRUCTURES AND UNIONS 

### ✅ SAME in C

* Structure definition
* Union definition
* Memory behavior
* Structure vs Union comparison
* Nested structures
* Access using `.` and `->`
* Use cases
* Padding concept

### ❌ REMOVE / CHANGE for C

| C++ Feature              | Status in C      |
| ------------------------ | ---------------- |
| Functions inside struct  | ❌ Not allowed    |
| Object-like usage        | ❌ Not allowed    |
| `using` keyword          | ❌ Not available  |
| C++ style struct = class | ❌ Not applicable |

### ✅ C Structure Usage

```c
struct Student {
    int roll;
};
struct Student s1;
```

📌 **Exam Line (C):**

> In C, a structure **contains only data**, not functions.

---

## 🎯 FINAL VERDICT (VERY IMPORTANT)

### ✔️ You **CAN reuse** these notes for C IF:

* You **remove C++-only features**
* You **replace references with pointers**
* You **replace `new/delete` with `malloc/free`**
* You **remove OOP-related behavior**

### ❌ You **CANNOT directly use** them for C without modification.

---























* **Structure of C Program**:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

* **Data types**: `int`, `float`, `double`, `char`, `void`
* **Variables**: Named memory locations to store data
* **Constants**: `#define PI 3.14` or `const int a = 10;`
* **Operators**: Arithmetic (`+ - * / %`), Relational (`> < == !=`), Logical (`&& || !`), Assignment (`=`)

---

## **4. Header Files** <a name="header-files"></a>

* **Purpose**: Contains **function declarations** and macros.
* **Common headers**:

  * `stdio.h` → Input/output (`printf`, `scanf`)
  * `stdlib.h` → Memory allocation, process control (`malloc`, `exit`)
  * `string.h` → String manipulation (`strcpy`, `strlen`)
  * `math.h` → Math functions (`sqrt`, `pow`)
* Include using: `#include <header.h>`

---

## **5. Data Handling** <a name="data-handling"></a>

* **Input/Output**:

```c
printf("Enter number: ");
scanf("%d", &num);
```

* **Type Casting**:

```c
int a = 10;
float b = (float)a; // convert int to float
```

* **Constants**: `const` or `#define`
* **Enumerations**:

```c
enum Day {Mon, Tue, Wed};
enum Day today = Mon;
```

---

## **6. Flow of Control** <a name="flow-of-control"></a>

* **Decision Making**:

```c
if (condition) { }
else if (condition) { }
else { }
switch (var) { case 1: break; default: break; }
```

* **Loops**:

  * `for (init; condition; increment) { }`
  * `while (condition) { }`
  * `do { } while (condition);`
* **Jump Statements**: `break`, `continue`, `goto`, `return`

---

## **7. Functions** <a name="functions"></a>

* **Definition**:

```c
return_type function_name(parameters) {
    // code
    return value;
}
```

* **Types**:

  * No return, no parameters
  * Return value, no parameters
  * No return, with parameters
  * Return value, with parameters
* **Example**:

```c
int add(int a, int b) {
    return a + b;
}
```

---

## **8. Arrays**

[Go to Arrays Notes](https://github.com/Saujanya-rajvanshi/Arrays-)

* **One-dimensional**: `int arr[5];`
* **Two-dimensional**: `int arr[3][3];`
* Access: `arr[i]` or `arr[i][j]`
* Initialization: `int arr[5] = {1,2,3,4,5};`

---

## **9. Pointers** <a name="pointers"></a>

* **Pointer**: Variable storing **address** of another variable.

```c
int x = 10;
int *ptr = &x;
printf("%d", *ptr); // prints 10
```

* **Pointer operations**: `*`, `&`, pointer arithmetic.
* **Applications**: Dynamic memory, arrays, functions (pass by reference).

---

## **10. Dynamic Memory Allocation** <a name="dynamic-memory-allocation"></a>

* Functions: `malloc()`, `calloc()`, `realloc()`, `free()`

```c
int *ptr = (int*)malloc(5 * sizeof(int)); // allocate 5 ints
free(ptr); // free memory
```

---

## **11. Structures & Unions** <a name="structures-unions"></a>

* **Structure**: Group different data types.

```c
struct Student {
    char name[20];
    int age;
};
struct Student s1;
```

* **Union**: Stores **one member at a time**, saves memory.

```c
union Data {
    int i;
    float f;
    char str[20];
};
```

---

## **12. File Handling** <a name="file-handling"></a>

* **File operations**: Open, read, write, close.

```c
FILE *fp;
fp = fopen("file.txt","w"); // write mode
fprintf(fp, "Hello");
fclose(fp);
```

* Modes: `r` (read), `w` (write), `a` (append), `r+` (read/write)

---

## **13. Preprocessor & Macros** <a name="preprocessor-macros"></a>

* **Macro**: Constant or function-like replacement.

```c
#define PI 3.14
#define SQUARE(x) ((x)*(x))
```

* **Conditional compilation**: `#ifdef`, `#ifndef`, `#endif`

---

## **14. String Handling** <a name="string-handling"></a>

* **String**: Array of characters ending with `\0`
* **Common functions**: `strlen()`, `strcpy()`, `strcat()`, `strcmp()`

---

## **15. Standard Libraries** <a name="standard-libraries"></a>

* `stdio.h` → I/O
* `stdlib.h` → Memory & process
* `string.h` → String functions
* `math.h` → Math operations
* `ctype.h` → Character functions (`isdigit`, `isalpha`)

---

## **16. Advanced Concepts** <a name="advanced-concepts"></a>

* **Recursion**: Function calling itself.
* **Bitwise operations**: `& | ^ ~ << >>`
* **Command-line arguments**: `int main(int argc, char *argv[])`
* **Typedef**: Create new type names

```c
typedef unsigned int uint;
```

---

## **17. Competitive Programming / DSA Readiness** <a name="competitive-programming"></a>

* Focus on: Arrays, Strings, Pointers, Recursion, Sorting, Searching
* Practice **Time & Space Optimization**
* Use **standard templates** for faster coding

---

## **18. Basic Maths Codes**

[Go to Basic Maths Codes](https://github.com/Saujanya-rajvanshi/basic-maths)

* Includes: Factorials, GCD/LCM, Prime checking, Fibonacci, Power, Modular arithmetic

---

If you want, I can **also make this into a fully clickable Markdown with small code snippets inside the index**, exactly like your C++ notes style. It will be ready to use in GitHub or your PDF notes.

Do you want me to do that next?


C language starting 
//first code <br>
#include<stdio.h><br>
void main()<br>
{<br>
printf("hello world");<br>
}<br>
<br>
<br>
\\output<br>
hello world <br>

<br>
#include<stdio.h><br>
void main() <br>
{ <br>
    int a,b,sum,sub,mul,di;<br>
    printf("enter number a and b");<br>
    scanf(" %d%d",&a,&b);<br>
    sum=a+b;<br>
    printf("%d+%d=%d\n",a,b,sum);<br>
    sub=a-b;<br>
    printf("%d-%d=%d\n",a,b,sub);<br>
    mul=a*b;<br>
    printf("%d*%d=%d\n",a,b,mul);<br>
    di=a/b;<br>
    printf("%d+%d=%d\n",a,b,di); <br>
}<br>
   <br> 
\\output<br>
enter number a and b<br>
200<br>
25<br>
200+25=225<br>
200-25-175<br>
200*25=5000<br>
200/25=8<br>
<br>


//valid declaration <br>
int a,b,c;<br>
a=b=c=5;<br>
printf("%d\n%d\n%d\n",a,b,c);<br>
<br>
#include <stdio.h><br>
void main() <br>
{    <br>
int a,b=2,c=3;<br>
printf("%d\n",c%b);<br>
printf("%d\n",-c%b);<br>
}<br>
<br>
//output<br>
1<br>
-1<br>
--- 

//operator

Here's a consolidated code example that demonstrates the use of various operators:

```c
#include <stdio.h>

void main()
{
    int a, b, c, sum, sub, mul, div, mod;
    a = 10;
    b = 3;

    // Arithmetic Operators
    sum = a + b; // Addition
    sub = a - b; // Subtraction
    mul = a * b; // Multiplication
    div = a / b; // Division
    mod = a % b; // Modulus

    printf("Arithmetic Operators:\n");
    printf("a + b = %d\n", sum);
    printf("a - b = %d\n", sub);
    printf("a * b = %d\n", mul);
    printf("a / b = %d\n", div);
    printf("a %% b = %d\n", mod); // %% to print %

    // Relational Operators
    printf("\nRelational Operators:\n");
    printf("a > b: %d\n", a > b);
    printf("a < b: %d\n", a < b);
    printf("a == b: %d\n", a == b);
    printf("a != b: %d\n", a != b);

    // Logical Operators
    printf("\nLogical Operators:\n");
    printf("(a > b) && (a != 0): %d\n", (a > b) && (a != 0));
    printf("(a < b) || (b != 0): %d\n", (a < b) || (b != 0));
    printf("!(a == b): %d\n", !(a == b));

    // Assignment Operators
    printf("\nAssignment Operators:\n");
    c = a; 
    printf("c = a: %d\n", c);
    c += b; 
    printf("c += b: %d\n", c);
    c -= b; 
    printf("c -= b: %d\n", c);
    c *= b; 
    printf("c *= b: %d\n", c);
    c /= b; 
    printf("c /= b: %d\n", c);
    c %= b; 
    printf("c %%= b: %d\n", c);

    // Bitwise Operators
    printf("\nBitwise Operators:\n");
    printf("a & b: %d\n", a & b);
    printf("a | b: %d\n", a | b);
    printf("a ^ b: %d\n", a ^ b);
    printf("~a: %d\n", ~a);
    printf("a << 1: %d\n", a << 1);
    printf("a >> 1: %d\n", a >> 1);

    // Unary Operators
    printf("\nUnary Operators:\n");
    printf("++a: %d\n", ++a);
    printf("--b: %d\n", --b);
}
```

### Explanation of Operators Used:
1. **Arithmetic Operators**: Perform mathematical operations (`+`, `-`, `*`, `/`, `%`).
2. **Relational Operators**: Compare values (`>`, `<`, `==`, `!=`).
3. **Logical Operators**: Logical AND (`&&`), OR (`||`), NOT (`!`).
4. **Assignment Operators**: Assign values (`=`, `+=`, `-=`, `*=`, `/=`, `%=`).
5. **Bitwise Operators**: Work on binary representations (`&`, `|`, `^`, `~`, `<<`, `>>`).
6. **Unary Operators**: Increment (`++`), Decrement (`--`).

### Example Output:
```
Arithmetic Operators:
a + b = 13
a - b = 7
a * b = 30
a / b = 3
a % b = 1

Relational Operators:
a > b: 1
a < b: 0
a == b: 0
a != b: 1

Logical Operators:
(a > b) && (a != 0): 1
(a < b) || (b != 0): 1
!(a == b): 1

Assignment Operators:
c = a: 10
c += b: 13
c -= b: 10
c *= b: 30
c /= b: 10
c %= b: 1

Bitwise Operators:
a & b: 2
a | b: 11
a ^ b: 9
~a: -11
a << 1: 20
a >> 1: 5

Unary Operators:
++a: 11
--b: 2


```


```c
#include <stdio.h>

int main() 
{
    int age;

    // Prompt the user to enter age
    printf("Enter age: ");
    scanf("%d", &age);

    // Check the age category
    if (age < 12) 
    {
        printf("child\n");
    } 
    else if (age < 18) 
    {
        printf("teenager\n");
    } 
    else 
    {
        printf("adult\n");
    }

    return 0;
}
```

### Example Input/Output:

#### Example 1:
**Input:**
```
Enter age: 10
```
**Output:**
```
child
```

#### Example 2:
**Input:**
```
Enter age: 15
```
**Output:**
```
teenager
```

#### Example 3:
**Input:**
```
Enter age: 20
```
**Output:**
```
adult
```





### ternary operator 
```c
#include <stdio.h>

int main() 
{
    int age;

    printf("Enter age: ");
    scanf("%d", &age);

    // Ternary operator to check if age is greater than 18
    age > 18 ? printf("adult \n") : printf("not adult \n");

    int number = 7;
    int luckyNumber = 7;

    // Ternary operator to check if number equals luckyNumber
    number == luckyNumber ? printf("you are lucky \n") : printf("you are not lucky \n");

    return 0;
}
```



### Example Input/Output:

#### Input 1:
```
Enter age: 20
```
**Output:**
```
adult 
you are lucky
```


Here’s the code:

```c
#include <stdio.h>

int main()
{
    char day;

    // Prompt the user to enter a character
    printf("Enter the first letter of a day (e.g., m for Monday, T for Thursday): ");
    scanf(" %c", &day); // Note the space before %c to handle newline characters

    // Switch statement for day
    switch (day)
    {
    case 'm':
        printf("Monday\n");
        break;
    case 't':
        printf("Tuesday\n");
        break;
    case 'w':
        printf("Wednesday\n");
        break;
    case 'T':
        printf("Thursday\n");
        break;
    case 'f':
        printf("Friday\n");
        break;
    case 's':
        printf("Saturday\n");
        break;
    case 'S':
        printf("Sunday\n");
        break;
    default:
        printf("Invalid input. Please enter a valid day character.\n");
        break;
    }

    return 0;
}
```



### Example Input/Output:

#### Input 1:
```
Enter the first letter of a day (e.g., m for Monday, T for Thursday): m
```
**Output:**
```
Monday
```

#### Input 2:
```
Enter the first letter of a day (e.g., m for Monday, T for Thursday): z
```
**Output:**
```
Invalid input. Please enter a valid day character.
```


###  Code:
```c
#include <stdio.h>

int main() 
{
    // For loop
    printf("Using for loop:\n");
    for (int i = 1; i <= 100; i++) 
    {
        printf("%d\n", i);
    }

    // While loop
    printf("\nUsing while loop:\n");
    int i = 1; // Initialize
    while (i <= 100) 
    {
        printf("%d\n", i);
        i++; // Increment
    }

    // Do-while loop
    printf("\nUsing do-while loop:\n");
    i = 1; // Re-initialize
    do 
    {
        printf("%d\n", i);
        i++; // Increment
    } while (i <= 100);

    return 0;
}
```



### Example Output:
```
Using for loop:
1
2
3
...
100

Using while loop:
1
2
3
...
100

Using do-while loop:
1
2
3
...
100
```


### Corrected Code:
```c
#include <stdio.h>

// Function to print factorial of n
int factorial(int n);

int main() {
    int n;

    printf("Enter n: ");
    scanf("%d", &n);

    // Handle negative inputs
    if (n < 0) {
        printf("Factorial of a negative number is undefined.\n");
    } else {
        printf("Factorial is: %d\n", factorial(n));
    }

    return 0;
}

int factorial(int n) {
    if (n == 0) {
        return 1; // Base case: factorial of 0 is 1
    }

    int factnm1 = factorial(n - 1); // Recursive call
    int factn = factnm1 * n;       // Multiply n with factorial of (n-1)
    return factn;
}
```



### Example Input/Output:

#### Input:
```
Enter n: 5
```
#### Output:
```
Factorial is: 120
```

#### Input:
```
Enter n: -3
```
#### Output:
```
Factorial of a negative number is undefined.
``` 

Here is an example of a simple **call by value** program in C:

### Code:
```c
#include <stdio.h>

// Function to demonstrate call by value
void modifyValue(int num) {
    printf("Inside function (before modification): num = %d\n", num);
    num = 20; // Modify the value of the parameter
    printf("Inside function (after modification): num = %d\n", num);
}

int main() {
    int num = 10;

    printf("Before function call: num = %d\n", num);

    // Call the function
    modifyValue(num);

    printf("After function call: num = %d\n", num);

    return 0;
}
```

### Explanation:
1. **Call by Value**:
   - In call by value, the value of the variable is passed to the function.
   - The function creates a copy of the variable in its own memory space.
   - Any changes made to the variable inside the function do not affect the original variable.

2. **How It Works**:
   - In the `main()` function, the value of `num` is 10.
   - When the `modifyValue()` function is called, a copy of `num` is passed to the function.
   - Modifications inside `modifyValue()` do not affect the original `num` in `main()`.

### Output:
```
Before function call: num = 10
Inside function (before modification): num = 10
Inside function (after modification): num = 20
After function call: num = 10
```

Here is an example of a **call by reference** program in C using pointers:

### Code:
```c
#include <stdio.h>

// Function to demonstrate call by reference
void modifyValue(int *num) {
    printf("Inside function (before modification): *num = %d\n", *num);
    *num = 20; // Modify the value of the variable using the pointer
    printf("Inside function (after modification): *num = %d\n", *num);
}

int main() {
    int num = 10;

    printf("Before function call: num = %d\n", num);

    // Call the function and pass the address of num
    modifyValue(&num);

    printf("After function call: num = %d\n", num);

    return 0;
}
```

### Explanation:
1. **Call by Reference**:
   - In call by reference, the address of the variable is passed to the function.
   - The function uses the pointer to directly access and modify the original variable.

2. **How It Works**:
   - In the `main()` function, the variable `num` has an initial value of `10`.
   - The address of `num` is passed to the `modifyValue()` function.
   - Inside `modifyValue()`, the dereferenced pointer (`*num`) is used to modify the value of the original variable.

### Output:
```
Before function call: num = 10
Inside function (before modification): *num = 10
Inside function (after modification): *num = 20
After function call: num = 20
```

### Key Point:
- The value of `num` in the `main()` function is changed after the function call, demonstrating **call by reference**.


### checking character 

```
char = input("Enter a character: ")

if char.isdigit():
    print("It is a number.")
else:
    print("It is not a number.")
```
