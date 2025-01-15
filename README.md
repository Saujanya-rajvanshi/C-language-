# C-language-
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

Your code is correct and will work as expected to determine whether the entered age corresponds to a "child," "teenager," or "adult." Here's the same code with improved formatting for readability:

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




Your code contains several issues that need correction for it to work properly:

1. **`luckyNumber 7`**: The `=` operator is missing in the declaration of `luckyNumber`.
2. **Syntax in `number luckyNumber?`**: This statement is missing an operator for comparison (e.g., `==` for equality check).
3. **Line breaks**: There's an incomplete statement `printf("you are not` and missing a closing quotation mark.

Here's the corrected code:

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

### Explanation of Changes:
1. **Declaration of `luckyNumber`**: Corrected it to `int luckyNumber = 7;`.
2. **Comparison in Ternary Operator**: Changed `number luckyNumber?` to `number == luckyNumber?`.
3. **Fixed Line Breaks**: Completed the `printf("you are not lucky \n")` statement.

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

#### Input 2:
```
Enter age: 15
```
**Output:**
```
not adult 
you are lucky
```

    
