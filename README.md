# C-language-
C language starting 
//first code
#include<stdio.h>
void main()
{
printf("hello world");
}
\\output
hello world 





#include<stdio.h>
void main()
{
    int a,b,sum,sub,mul,di;
    printf("enter number a and b");
    scanf(" %d%d",&a,&b);
    sum=a+b;
    printf("%d+%d=%d\n",a,b,sum);
    sub=a-b;
    printf("%d-%d=%d\n",a,b,sub);
    mul=a*b;
    printf("%d*%d=%d\n",a,b,mul);
    di=a/b;
    printf("%d+%d=%d\n",a,b,di)
}
\\output
enter number a and b
200
25
200+25=225
200-25-175
200*25=5000
200/25=8



//valid declaration 
int a,b,c;
a=b=c=5;
printf("%d\n%d\n%d\n",a,b,c);

#include <stdio.h>
void main()
{    
int a,b=2,c=3;
printf("%d\n",c%b);
printf("%d\n",-c%b);
}

//output
1
-1


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
