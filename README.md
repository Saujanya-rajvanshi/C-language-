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
