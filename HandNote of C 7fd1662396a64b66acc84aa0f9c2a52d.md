# HandNote of C

C = Structural Programming Language

C = Case-Sensitive

C = By using 'Compiler' and Compiler: GCC

```
[❏] **Requirements**:
    Applications: Netbean (IDE) [before install, JDK(java_development_kit)]
                  OR CodeBlock (IDE)
    Compiler: GCC

[❏] **URL**:
        -->> https://en.cppreference.com/w/ (Official Site)
        -->> https://www.cprogramming.com/
        -->> https://www.oracle.com/technetwork/java/javase/downloads/index.html
                                    [Download: JDK Compiler for Java or Netbean]
        -->> https://netbeans.org [Download: NetBean (IDE)]
        -->> http://www.codeblocks.org/downloads/binaries
                              [Download CodeBlocks (IDE)]

        Tutorial
        -->> https://www.learn-c.org/
        -->> https://www.tutorialspoint.com/cprogramming/index.htm

        Exercises
        -->> https://www.learn-c.org/

```

Syntax

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{

    // Code...

    return 0;   // using 'getch()' or 'return 0'
}

```

==============================================================

**SYNTAX** || **EXAMPLE** :: ===============================================

==================== **TAG** || **PARAMETER** || **FUNCTION()** ==================

=================================================== **HINTS** || **NOTES**

**N O T E S :**

1. IntergerNumber / IntergerNumber = Interger Result  [Ex: 1/2 = 0.5 = 0]

2. FloatNumber / IntergerNumber = Float Result

3. SingleLine Code where '{ . . . }' block do not needed [Ex: if(true) cout<<"Hello"; ]

**CHAPTER**

- ----------

CHAPTER A: ('Go to Read' >> 'intro_c_code.md' file)

CHAPTER B: Input-Output

CHAPTER C: Operator

CHAPTER D: Conditional Statement

CHAPTER E: Array (DataType)

CHAPTER F: String (DataType)

CHAPTER G: Function

CHAPTER H: Structure, Union, Enum, Typedef

CHAPTER I: Pointer

CHAPTER J: File

CHAPTER K: Preprocessor

=========================================== B A S I C ________ S Y N T A X

=================================  **SYNTAX** || **TAG** || **PARAMETER** || **EXAMPLE**

// BREAK;

=========================   ==================

+                  C H A P T E R                   [ B ]                   IS                   # **INPUT - OUTPUT**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

```
/*_<block_start>

# Comment
=================================================
Single line comment: // Single line comment
Multiple line comment:  /* Multiple line comment */
/*

# Escape Sequence/Backslash Character Constant (***Only Work for Output function())
=================================================
        \a     : (Alert) Bell
        \b     : BackSpace
        \f     : Form Feed
        \n     : New Line
        \r     : Carrige Return
        \t     : Horizontal Tab
        \v     : Vertical Tab
        \0     : Null Character
        \'     : Single Quate '
        \"     : Double Quate "
        \\     : BackSlash
        \?     : QuestionMark
    *** endl   : new line

               Example:
                       cout<<" Hello, \n How are you, today?"; // \n
                       cout<<" \n Hello, \"Shakib\" "; //  \"
                       cout<<" \n Hello,\t\"Shakib\" "<<endl; //  \t

<block_close>_*/

```

**# Keywords list** (32 Keywords)

============================================

- ------- -------- -------- ---------

auto          double     int           struct

break        else          long        switch

case          enum       register   typedef

char          extern      return     union

const        float         short       unsigned

continue   for           signed     void

default      goto        sizeof      volatile

do             if              static      while

**# Datatype & Format Specifier**

============================================

[**#**] Primitive (Built-in Datatype)

____________________________________________________________________

.

| **Datatype** | **Keyword** | **Mem. Size** | **FormatSpecifier** | **Example** |
| --- | --- | --- | --- | --- |
| Boolean (T/F) | bool | 1 byte | %b | true (result: true)false (result: false)1     (result: true)0     (result: false) |
| void () | - | - | - | - |
| Character | char | 1 byte | %c | 'a', 'b', 'c' |
| Integer | int | 4 byte | %d or %i | 126, 130 |
| Float | float | 4 byte | %f | 3.18, .3.2585 (6 decimal places) [NB. After ".", use: %.2f (then show 2 num)] |
| Double | double | 8 byte | %lf | 3.25365969 (15 decimal places)   [NB. After ".",use: %.2f (then show 2 num)] |
- **------------------------** Number Conversion / System

.

| **Datatype** | **Keyword** | **Mem. Size** | **FormatSpecifier** | **Example** |
| --- | --- | --- | --- | --- |
| Integer in Hexa | int | 4 byte | %x | 255 (result: ff) |
| Integer in Octal | int | 4 byte | %o | - |

[**#**] Non-Primitive (Derived Datatype)

_________________________________________________________________________

.

| **Datatype** | **Keyword** | **Mem. Size** | **FormatSpecifier** | **Example** |
| --- | --- | --- | --- | --- |
| String [char var[]] | - | - | %s | "Abc" (result: Abc) |
| Object | - | - | %O | 1,2 (result: 1,2) |
| Print AnyThing | - | - | %A | 1,[] (result: 1,[]) |
| Array | ar_name[] | - | ar_name[index] | array_name[25];[*** Briefly describe: CHAP E: Array] |

[**#**] Custom / User-defined Datatype

_________________________________________________________________________

Structure         = Custom DataType and all members share total memory location

Union              = Like as Structure and all members share single/same memory location

Enumeration   = Consists of integral constants.

Typedef           = Renaming Primitive / User-defined DataType Name

[**#**|**#**] Bytes and Range of Datatype

Modifiers:

short = convert memory size: half from full | Example: (int: 4 bytes) to (int: 2 bytes)

long = convert mem. size double | Example: (long int/int: 4 bytes) to (int: 8 bytes)

signed = by using for positive/negative numbers

unsigned = by using for only positive numbers

_________________________________________________________________________

.

| **Datatype** | **Size(in bytes)** | **Range** |
| --- | --- | --- |
| short int | 2 | -32,768 to 32,767 |
| unsigned short int | 2 | 0 to 65,535 |
| unsigned int | 4 | 0 to 4,294,967,295 |
| int | 4 | -2,147,483,648 to 2,147,483,647 |
| long int | 4 | -2,147,483,648 to 2,147,483,647 |
| unsigned long int | 4 | 0 to 4,294,967,295 |
| long long int | 8 | -(2^63) to (2^63)-1 |
| unsigned long long int | 8 | 0 to 18,446,744,073,709,551,615 |
| signed char | 1 | -128 to 127 |
| unsigned char | 1 | 0 to 255 |
| float | 4 |  |
| double | 8 |  |
| long double | 12 |  |
| wchar_t | 2 or 4 | 1 wide character |

**# Variable**

============================================

**Variable Declaration Rules**:

Allow the following characteristics:

.

| **Variable Style** | **Status** | **Comments** |
| --- | --- | --- |
| _classNo | Allow | (Valid: A-Z, a-z, 0-9, _ , $) otherwise; other characters invalid |
| $classNo | Allow |  |
| ClassNo1 | Allow | (Digit) |
| CSE300 | Allow |  |
| Cse203 | Allow |  |
| ex2no | Allow |  |
| class_name | Allow | (Space) |
| Float | Allow | (Keyword) |
| Main | Allow | (function/method) |

Not Allow the following characteristics:

.

| **Variable Style** | **Status** | **Comments** |
| --- | --- | --- |
| "my name" | Not Allow | (Not valid) |
| #classNo | Not Allow |  |
| my_name# | Not Allow |  |
| 120name | Not Allow | (Digit) |
| my name is | Not Allow | (Space) |
| float | Not Allow | (Keyword) |
| for | Not Allow |  |
| main | Not Allow | (function/method) |

**#**_**Variable Declaration Syntax**:

DataType Veriable_Name;

Example:

```
int ver_name;  (Variable Declare)
ver_name = 10; (Value Initialization)

```

**#**_**Types of veriable**:

[**#**] Global Variable

- ------------------------------

Declare the outside of main() and others function.

Example:

```
#include <stdio.h>
#include <stdlib.h>
char name [35] = "Michael"; //Global Variable

int main()
{
    // Code...

    return 0;
}

```

**[#]** Local Variable

- ------------------------------

Declare the inside of main() and others function.

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    char name [15] = "Michael"; //Local Variable
      // Code...
    return 0;
}

```

**# Output ----------- Syntax**

============================================

Syntax:

printf **("** <your_text> **")**;

Example:

```
printf("Enter Your Text");

```

OR

Syntax:

printf **("** <your_text> <EscapeSequence> **")**;

Example:

```
printf("Enter Your Text \n");

```

OR

Syntax:

printf **("** <your_text> <format_specifier> <EscapeSequence> **",** VariableName**);**

Example:

```
printf("Your Name is: %s \n", ver_name);

```

Example Code:

```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num=10;
    printf("The Number is %d", num);
    return 0;
}

```

**# Input ----------- Syntax**

============================================

Syntax:

scanf **("** <format_specifier> **",** **&**VariableName **);**

Example:

```
scanf("%s", &ver_name);

[using '%s' format_specifier and VariableName with '&' symbol]

```

Example Code 01: (1 Input & 1 Output)

```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num;
    printf("Enter the number: \n");
    scanf("%d", &num);

    printf("The Number is: %d \n", num);
    return 0;
}

```

Example Code 02:

```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num1, num2;
    printf("Enter the number X & Y are: \n");
    scanf("%d %d", &num1, &num2);
    printf("The numbers are: %d and %d \n", num1, num2);
    return 0;
}

```

**# Type Casting**

============================================

Convert: One DataType to Another DataType

Example Code: (Calculate the summation and average from given numbers)

```
int x=12, y=12, z=13, sum; float avg;
sum = x+y+z;
avg = (float) sum/3;  //TypeCasting
printf("The summation is: %d \n", sum);
printf("The Average is: %.2f \n", avg);

*** Note: 1. IntergerNumber / IntergerNumber = Interger Result [Ex: 1/2 = 0.5 = 0]
          2. FloatNumber / IntergerNumber = Float Result

```

=========================   ==================

+                  C H A P T E R                   [ C ]                   IS                   # **OPERATOR**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

Arithmetic Operator, Assignment Operator, Relational Operator, Logical Operator,

Conditional Operator, Unary Operator, Bitwise Operator, Special Operator

**Arithmetic Operator**

___________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Plus | + | 2+5=7; | Add: 2 operands by using '+' |
| Minus | - | 5-2=3; | Subtraction: 2 operands by using '-' |
| Multiple | * | 5*7=35; | Multiplication: 2 operands by using '*' |
| Division | / | 12/3=4; | Division: 2 operands by using '/' |
| Modulus | % | 16%5=1; | Calculate reminder from '16/5' |
| Equal to | == | x == y; | Both operands are equal |

**Assignment Operator**

___________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Assignment | : = | y = x+5; | Left Statement assign to Right Statement by using assignment operator (=) |
| Plus-assignment | += | x += 5; | x = x+5; |
| Minus-assignment | -= | x -= 5; | x = x-5; |
| Multiple-assignment | *= | x *= 5; | x = x*5; |
| Division-assignment | /= | x /= 5; | x = x/5; |
| Modulus-assignment | %= | x %= 5; | x = x%5; |

**Unary Operator**

___________________________________________________________

Unary Plus : ++ (Increment) [ Prefix + Postfix ]

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Prefix | ++a | Code:          x=25;         y=++x;         //out:26        y=x;       //out:26 | before add |
| Postfix | a++ | Code:         x=25;         y=x++;         //out:25         y=x;        //out:26 | After add |

Unary Minus : -- (Decrement) [ Prefix + Postfix ]

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Prefix | --a | Code:          x=25;         y=--x;         //out:24        y=x;       //out:24 | before minus |
| Postfix | a-- | Code:         x=25;         y=x--;         //out:25         y=x;        //out:24 | After minus |

**Relational Operator**

___________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Greater-than | > | x>y | x is Greater-than y |
| Greater-than/Equal | >= | x>=y | x is Greater-than or Equal to y |
| Less-than | < | x<y | x is Less-than y |
| Less-than/Equal | <= | x<=y | x is Less-than or Equal to y |
| Equal to | == | x==y | x is Equal y |
| Not/Equal to | != | x != y | x is Not Equal to y |

**Logical Operator**

_____________________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Logical AND | && | (x>y && x>z) then x | When both side is true.then, TRUE. Else FALSE.(If both condition true then 'x' work else not work) |
| Logical OR | || | (x>y || x>z) then x | When both/any side is true.then, TRUE. Else FALSE(If both/any condition true then 'x' work else not work) |
| Logical NOT | ! | x != 5; | 'NOT' means 'No/Never'. (here, 5 is not value of x) |

**Ternary Operator**

_____________________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Ternary | ? : | x==5 ? y='A' : z='B' | If 'x==5' is true.then work 'y'. eles work 'z' |

Syntax:

condition **?** expression1 **:** expression2

NB. if condition is true,then expression1 work and condition is false,then expression2 work

**Bitwise Operator**

_____________________________________________________________________

.

| **Operator** | **Style** | **Example** | **Meaning** |
| --- | --- | --- | --- |
| Bitwise AND | & | 32 & 12 = 0 | firstly, to Binary convert, then Bitwise AND Operation[Hints: Multiplication] |
| Bitwise OR | | | 32 & 12 = 44 | firstly, to Binary convert, then Bitwise OR Operation. [Hints: Addition] |
| Bitwise EX-OR | ^ | 32 & 12 = 44 | firstly, to Binary convert, then Bitwise EX-OR Operation. |
| Bitwise NOT | ~ | ~32 = -33 | firstly, to Binary convert, then Bitwise NOT Operation.                                                             [Hints: Reverse/Opposite/Mirror Operation]   ** |
| Bitwise Shift Right | >> | a=32; c=a>>3; | ShiftRi... '3' iteration and Divided by 2 for each iteration |
| Bitwise Shift Left | << | a=32; c=a<<3; | ShiftLe. '3' iteration and Multiple by 2 for each iteration |

Condition:

- Work with bit/byte
- Work into only integer number

Operation Steps:

```
1. firstly Convert decimal/integer number to Binary number
   Example:
          let, int x=32, y=12;      128 | 64 | 32 | 16 | 8 | 4 | 2 | 1  (from: 2^n)
                                    -----------------------------------
           Convert to Binary, x=32=  0    0     1    0   0   0   0   0
           Convert to Binary, y=12=  0    0     0    0   1   1   0   0

2. Operation:
             Bitwise AND: &
             Condition: If Both input are '1' then out: 1. Otherwise; out: 0
             Binary,  x=32= 0 0 1 0 0 0 0 0
             Binary,  y=12= 0 0 0 0 1 1 0 0
             --------------------------------
             Multiply[x*y]= 0 0 0 0 0 0 0 0  (= result: 0)

             Bitwise OR: |
             Condition: If Both/Any input are '1' then out: 1. Otherwise; out: 0
             Binary,  x=32= 0 0 1 0 0 0 0 0
             Binary,  y=12= 0 0 0 0 1 1 0 0
             ---------------------------------
             Addition[x+y]= 0 0 1 0 1 1 0 0  (= result: 44)

             Bitwise EX-OR: ^
             Condition: If Both input are same then out: 0. Otherwise; out: 1
             Binary,  x=32= 0 0 1 0 0 0 0 0
             Binary,  y=12= 0 0 0 0 1 1 0 0
             ---------------------------------
             Ex-OR [x^y]  = 0 0 1 0 1 1 0 0  (= result: 44)

```

**Special Operator**

__________________________________________________________________

Comma ( , )

Pointer ( * )

sizeof()

Comma ( , ) Operation:

- ------------------------

Comma( **,** ) between seperate expression.

Example:

```
int x, y, sum;
sum = (x=10, y=16, sum=x+y);
printf(" Summation: %d \n", sum); //Out: 26

```

sizeof() Operation:

- -------------------

Syntax:

sizeof **(**dataType**)**;

Example:

```
int a;         //Out: 4 byte
float b;       //Out: 4 byte
double d;      //Out: 8 byte
char ch;       //Out: 1 byte
char name[20]; //Out: 20 byte

int x = sizeof(name);
printf(" Memory Size: %d \n",x ); //Out: 20 byte

```

=========================   ==================

+                  C H A P T E R                   [ D ]                   IS                   # **CONDITIONAL STATEMENT**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

CONDITIONAL Statement: Selector + Iteration + Jump

**# Selector**

============================================

if | if... else | if... else if | switch ========================

**if**

- ----------------------------------------------

Syntax:

if **(**condition**)**

**{**

//Code block . . .

**}**

Example Code:

```
if(n%2 == 0)
{
    printf("Even Number");
}

```

**if... else**

- ----------------------------------------------

Systax:

if **(**condition**)**

**{**

//Code block . . .

 **}**

else

 **{**

//Code block . . .

 **}**

Example Code:

```
if(n%2 == 0)
{
    printf("Even Number \n");
}
else
{
    printf("Odd Number \n");
}

```

**if... else if**       

- ----------------------------------------------

Systax:

if **(**condition**)**

**{**

//Code block . . .

**}**

else if (condition)

**{**

//Code block . . .

**}**

else

  **{**

//Code block . . .

    **}**

Example Code:

```
if(n%2 == 0)
{
    printf("Even Number \n");
}
else if(n%2 !== 0)
{
    printf("Odd Number \n");
}
else
{
    printf("invalid number! \n");
}

```

**? :** (Ternary Operator)

- ----------------------------------------------

Syntax:

condition **?** expression1 **:** expression2

NB: if condition is true,then expression1 work and condition is false,then expression2 work.

**switch**

- ----------------------------------------------

Syntax:

switch **(**expression**)**

**{**

case value 1**:**

//Code block . . .

break;

case value 2**:**

//Code block . . .

break;

case value 3**:**

//Code block . . .

break;

......

......

case value N**:**

//Code block . . .

break;

default**:**

//Code block . . .

**}**

Example 01: (digit check)

```
int digit=1;
switch(digit)
{
   case 1:
          cout<<" Digit is: "<< digit <<endl; //this block is activated...
          break;
   case 2:
          break;
   case 3:
          break;
   case 4:
          break;
   default:
           cout<<" Not a digit "<<endl;
}

```

Example 02: (vowel check)

```
char ch='u';
switch(ch)
{
    case 'a':
    case 'e':
    case 'i':
    case 'o':
    case 'u':
             cout<<" Vowel "<<endl;
             break;
    default:
            cout<<" Consonant"<<endl;
}

```

**# Iteration**

============================================

for | while | do while ==============================

**for**

- ----------------------------------------------

Syntax:

for **(**Initialization**;** Condition**;** Increment/Decrement**)**

**{**

//Code block . . .

**}**

Example Code:

```
for(int i=1; i<=50; i++)
{
    printf("%d \n",i);
}

```

**while**

- ----------------------------------------------

Syntax:

while **(**condition**)**

 **{**

//Code block . . .

  //Increment/Decrements

**}**

Example Code:

```
int i=1; //Initialization
while(i<=10)
{
    printf("%d \n",i);
    i++; //Increment/Decrement
}

```

**do while**

- ----------------------------------------------

Syntax:

//Initialization

do **{**

//Code block . . .

  //Increment/Decrement

**}** while **(**condition**)**;

- ** while vs do-while:

the do while loop, 'do' block execute at least one time even the 'while' condition will be false.

Example Code:

```
int i=1;    //Initialization

do
{
    printf("%d \n", i);
    i++;    //Increment/Decrement
} while(i<=10);

```

**# Nested Loop / Nested Condition Statement**

============================================

for | while | do while |:| if | if... else | if... else if | switch ==========

___________________________________________________________________

Loop: 'Another loop' will be work into 'main loop'

Condition: 'Another condition' will be work into 'main condition'

**nested for Loop**

- ----------------------------------------------

for **(**Initialization**;** Condition**;** Increment/Decrement**)**   //Condition is true then goto 'next loop'.

**{**

     //When this loop's work will have to done then back to 'Previous loop'.

for **(**Initialization**;** Condition**;** Increment/Decrement**)** 

**{**

//Code block . . .

**}**

**}**

**nested if condition**

- ----------------------------------------------

if **(**condition**)**       //Condition is true then goto 'next if'.

**{**

if **(**condition**)**  //When this "if's" work will have to done then this block terminate

 **{**

//Code block . . .

**}**

**}**

**# Jump**

============================================

continue | break | return ============================

**continue**

- ----------------------------------------------

Syntax:

continue;

Note: The continue statement skips the cuurent iteration of a loop.

(for, while, do....while loop)

Example:

```
for(int i=1; i<=100; i++)
{
    if(i==10) //When match then continue and back to loop again
    {
        continue; //bypass/back to loop again
        printf(i);
    }
}

//Output: 1 2 3 4 5 6 7 8 9 11 12 13  ..... 100 (without 10)

```

**break**

- ----------------------------------------------

Syntax:

break;

Notes: break statement is used to break loop or switch statement

Example:

```
for(int i=1; i<=100; i++)
{
    if(i==10) //When match then break
    {
        break;
        printf(i);
    }
}

//Output: 1 2 3 4 5 6 7 8 9 10

/* note: It breaks the current flow of the program at specified condition.
                      In case of innar loop, it breaks only inner loop. */

```

**goto**

- ----------------------------------------------

Syntax:

Level_Name**:**

 // Code Block ...

// Increment/Decrement

if **(**Condition**)**

goto Level_Name;   // Level is calling here

- ** When if condition is true then 'goto' calling 'Level_Name' and 'Level_Name' level will be work.

Otherwise; not work.

Example Code:

```
int i=1;   // Initialization

LevelN_print:
             printf("%d \n", i);
             i++;
if(i<=5)
     goto LevelN_print; // Level is calling here

```

**return**

- ----------------------------------------------

Syntax:

return;

- ** Note: The return statement return to '0' than the program is terminate.

otherwise; program is not terminate/exit.

Example:

```
return 0;

```

=========================   ==================

+                  C H A P T E R                   [ E ]                   IS                   # **ARRAY**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

An Array is collection of veriables of same type.

- Array Index start with '0'
- '0' always positive

Syntax:

DataType array_name **[**array_size**]**;

Example:

```
int student_roll [3];

/* ===== Value Insert/Index ===== */
student_roll [0]=161722;
student_roll [1]=161723;
student_roll [2]=161724;

//or
student_roll[3] = {161722,161723,161724};

//or
student_roll[] = {161722,161723,161724};  //Automatic Indexing

//or
for(i=0; i<=3; i++){
    scanf("%d", &student_roll[i]);
}

/* ===== Value Print ===== */
printf("%d", student_roll [0]); //Result: Sumon
printf("%d", student_roll [1]); //Result: Mamun
printf("%d", student_roll [2]); //Result: Sujon

//or
printf("%d %d %d", student_roll[0],student_roll[1],student_roll[2]);

//or
for(i=0; i<=3; i++){
     printf(" %d ", student_roll[i]);
}

```

Types of Array:

[#] One Dimensional array or Linear array    // Ex: int marks[10];

[#] Multi-dimensional Array:

[#] Two Dimensional(2-D) array or Matrix array     // Ex: *int* marks[2][3];

[#] Three Dimensional array         // Ex: *int* marks[2][3][2];

**# One Dimensional Array**

============================================

Syntax:

DataType array_name **[**array_size**]**;

Diagram:

int student_roll_no**[**3**]** = **{**161722, 161723, 161724**}**;

/* -------------- Value Insert Diagram ------------ */

_____________________________________________________

student_roll [0] **|** student_roll [1] **|** student_roll [2] **|**  -> Index Number [#]

-------------------------------------------------------

 **|**      161722      **|**        161723       **|**       161724       **|**  -> Values

-------------------------------------------------------

Example:

[1].

```
int num [5], sum=0;

num[0]=10;
num[1]=25;
num[2]=20;
num[3]=28;
num[4]=39;

sum=num[0]+num[1]+num[2]+num[3]+num[4];
printf("The sum is: %d \n", sum);
printf("The average is: %.2f \n", (float) sum/5);

```

[2].

```
int num [5], sum=0;

printf("Enter 5 numbers: ");
scanf("%d %d %d %d %d", &num[0], &num[1], &num[2], &num[3], &num[4]);

sum=num[0]+num[1]+num[2]+num[3]+num[4];
printf("The sum is: %d \n", sum);
printf("The average is: %.2f \n", (float) sum/5);

```

[3].

```
int num [5], sum=0, i;

printf("Enter 5 numbers: ");
for(i=0; i<5; i++){
    scanf("%d", &num[i]);
}

for(i=0; i<5; i++){
    sum=sum+num[i];
}
printf("The sum is: %d \n", sum);
printf("The average is: %.2f \n", (float) sum/5);

```

**# Two Dimensional/Matrix Array**

============================================

Syntax:

DataType array_name **[**row_size**][**col_size**]**;

Note: here, total Variables: row_size * col_size;

Diagram:

int a**[**3**][**4**]**;

/* -------------- Value Insert Diagram ------------ */

_____________________________________________

col [0]  **|** col [1]  **|** col [2]  **|** col [3] **|**

_____________________________________

Row [0] **|** a[0][0] **|** a[0][1] **|** a[0][2]  **|** a[0][3] **|**   -> Index Number

_____________________________________

Row [1] **|** a[1][0] **|** a[1][1] **|** a[1][2]  **|** a[1][3] **|**   -> Index Number

_____________________________________

Row [2] **|** a[2][0] **|** a[2][1] **|** a[2][2]  **|** a[2][3] **|**   -> Index Number

--------------------------------------

Example:

[1]. Value insert type 1

```
int a[3][4];

a[0][0]=10;
a[0][1]=11;
a[0][2]=12;
a[0][3]=13;

a[1][0]=20;
a[1][1]=21;
a[1][2]=22;
a[1][3]=23;

a[2][0]=30;
a[2][1]=31;
a[2][2]=32;
a[2][3]=33;

```

// Or

// Value insert type 2

```
int a[3][4] = { {10,10,12,13}, {20,21,22,23}, {30,31,32,33} };

```

/* -------------- Value Insert Diagram ------------ */

col [0]  **|** col [1] **|** col [2] **|** col [3] **|**

___________________________________

Row [0] **|**   10    **|**   11     **|**   12     **|**   13     **|**     -> Index Number

___________________________________

Row [1] **|**   20    **|**   21     **|**   22     **|**   23     **|**     -> Index Number

___________________________________

Row [2] **|**   30    **|**   31     **|**   32     **|**   33     **|**     -> Index Number

------------------------------------

```
//Output:

printf("%d \n", a[0][2]);       //result: 12
printf("%d \n", a[1][2]);       //result: 22
printf("%d \n", a[2][1]);       //result: 30

```

[2].

```
int a[3][4] = { {10,10,12,13}, {20,21,22,23}, {30,31,32,33} };  //Initialization

for(int row=0; row<3; row++){      //Value Print
    for(int col=0; col<4; col++){
        printf("%d ", a[row][col]);
    }
    printf("\n");
}

```

[3].

```
int a[3][4];
int row, col;

//Initialization value
for(row=0; row<3; row++){
    for(col=0; col<4; col++){
        printf(" a[%d][%d]: ", row, col);
        scanf("%d", &a[row][col]);
    }
    printf("\n");
}

//Showing matrix
for(int row=0; row<3; row++){
    for(int col=0; col<4; col++){
        printf(" %d ", a[row][col]);
    }
    printf("\n");
}

```

=========================   ==================

+                  C H A P T E R                   [ F ]                   IS                   # **STRING**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

String is characters type array.

String supported multiple characters length.

Syntax:

DataType string_name **[**string_size**]**;

Diagram:

char str_name**[**10**]** = {"Bangladesh"};

/* ----------------- Value Insert Diagram -------------- */

_________________________________________________________

name [0] **|** name [1] **|** name [2] **|** name [3] **|** name [4] **|** ...    -> Index Number [#]

-----------------------------------------------------------

**|**       B     **|**       A       **|**      N       **|**       G       **|**        L       **|** ...   -> Values

-----------------------------------------------------------

Example:

[1].

```
char name [7];

name[0]='B';
name[1]='A';
name[2]='N';
name[3]='G';
name[4]='L';
name[5]='A';
name[6]='\0';  //null character using  for avoid error from last index
printf("The string is: %s \n", name);

OR
char name []={'B', 'A', 'N', 'G', 'L', 'A', '\0'}; //here, array_size no needed
printf("The string is: %s \n", name);

OR
char name []="BANGLA";          //for Single line
printf("The string is: %s \n", name);

OR
char name []="BANGLA \ DESH"; //for Multiple line & must be use '\' line breaking char..
printf("The string is: %s \n", name);

```

[2]. String I/O

```
char name [50];
printf("Enter the name: ");
scanf("%s", &name);
printf("The string is: %s \n", name);

/* Input : Nazrul Islam
   Output: Nazrul

***Error! because, scanf() function can't work for 'Space' */

```

OR

```
char name [50];
printf("Enter the name: ");
gets(name);
printf("The string is: %s \n", name);

/* Input : Nazrul Islam
   Output: Nazrul Islam

   ***No Error! */

```

=========================   ==================

+                  C H A P T E R                   [ G ]                   IS                   # **Function**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

A function is a group of statements that together perform a task.

# 2 Types of functions: (1). library function. (2). User-defined function.

Diagram:

------------

Input--> **|** Function **|** --> Output

------------

f(x) = a^2 + 3*a*b + c^5

here, f(result) = Calculation formula

Syntax:

ReturnType Function_Name **(**Arguments**)**

**{**

//Code block . . .

 **}**

# **LIBRARY FUNCTION()**:

============================================

============== **Built-in function()** =================

**HEADER files for LIBRARY FUNCTION()**

Syntax: #include <header_file_name>

Stdio.h (Standard input-output .header)

```
f(x)_are:
printf(), scanf(), getchar(), putchar(), gets(), puts(), fopen(), fclose(), feof()

```

Conio.h (Console input-output .header)

Contains declaration for console I/O functions

```
f(x)_are: clrscr(), getch(), exit()

```

Ctype.h (Character Type .header)

Used for Caracter-handling or testing Character

```
f(x)_are: isupper(), islower(), isalpha()

```

Math.h (Mathematic. header)

Declares mathematical functions and macros.

```
f(x)_are: pow(), sqrt(), sin(), cos(), tan(), log()

```

Stdlib.h (Standard Library. header)

Used for number conversions, storage allocations

```
f(x)_are: rand(), srand()

```

String.h (String. header)

Used for manipulate strings.

```
f(x)_are: strlen(), strctp(), strcmp(), strcat(), strlwr(), strupr(),strrev()

```

Time.h   =Time. header

Used for manipulating time and date.

**||||||||||||||||||||||||||||** **Data-type**

# sizeof();

- **--------------------------------------------------------------------------** [lib./header: <stdio.h>]

Showing Variable Memory Size which datatype included

**sizeof()**;

- **-----------------------**

Example Code:

```
char a; int b; float c; double d;

printf("Size of Character is: %d \n", sizeof(a));
printf("Size of Integer is: %d \n", sizeof(b));
printf("Size of Float is: %d \n", sizeof(c));
printf("Size of Double is: %d  \n", sizeof(d));

```

**||||||||||||||||||||||||||||** **Character**

# toupper(); tolower();

- **--------------------------------------------------------------------------** [lib./header: <stdio.h>]

Convert: Uppercase to Lowercase letter and Lowercase to Uppercase letter.

(Using ASCII Formula)

**toupper()**;

- ------------------------------

Example Code: (lowercase to uppercase)

```
#include <stdio.h>

int main()
{
    char lower, upper;

    printf("Enter any lowercase letter: ");
    scanf("%c", &lower);

    upper = toupper(lower);
    printf("The uppercase letter is: %c \n", upper);
    return 0;
}

```

**tolower()**;

- ------------------------------

Example Code:(uppercase to lowercase)

```
#include <stdio.h>

int main()
{
    char upper, lower;

    printf("Enter any uppercase letter: ");
    scanf("%c", &upper);

    lower = tolower(upper);
    printf("The lowercase letter is: %c \n", lower);
    return 0;
}

```

**|||||||||||||||||||||||||||| Mathematical**

# abs(), sqrt(), pow(); exp(); sin(); cos(); sec(); cosec(); tan(); cot();

log(); log10(); round(); ceil(); floor(); trunc(); rand();

- **--------------------------------------------------------------------------** [lib./header: <math.h>]

Calculate 'Mathematical equation'

**abs()**;

- ------------------------------

Calculate 'Absolute value' from a mathematical equation.

Example Code:

```
int x= -12;
x = abs(-12);
printf("%d \n", x);  //result: 12

```

**sqrt()**;

- ------------------------------

Calculate 'Square Root' from a mathematical equation.

Example Code:

```
int x=4;
double result = sqrt(x);
printf("%.2lf \n", result); //result: 2

```

OR (problem: Quadratic equation)

```
double a=3, b=5, c=2, d, x1, x2;
d=sqrt(b*b - 4*a*c);
x1=(-b+d) / (2*a);
x2 =(-b-d) / (2*a);
printf("The value of x1 is: %.2lf \n", x1);
printf("The value of x2 is: %.2lf \n", x2);

```

**pow()**;

- ------------------------------

Calculate 'Power' from any value from a mathematical equation.

Syntax & Example:

pow(base, exponent) =  Base^Exponent = x^y = 2^3 = 8

Example Code:

```
double x = pow(4,2);    //formula: 4^2=16
printf("%.2lf \n", x);  //result: 16

```

**log()**;

- ------------------------------

Calculate 'log' from any value from a mathematical equation.

Example Code:

```
int x=10.5;
double result = log(x);
printf("%.2lf \n", result); //result: 2.30

```

**log10()**;

- ------------------------------

Calculate 'log10' from any value from a mathematical equation.

Example Code:

```
int x=10.5;
double result = log10(x);
printf("%.2lf \n", result); //result: 1.00

```

**exp()**;

- ------------------------------

Calculate 'Experiential' from any value from a mathematical equation.

Example Code:

```
int x=5;
double result = exp(x);
printf("%.2lf \n", result); //result: 148.41

```

**sin()**; **cos()**; **sec()**; **cosec()**; **tan()**; **cot()**;

-------------------------------------------

Calculate 'Experiential' from any value from a mathematical equation.

Example Code:

```
int x=46;
double result = sin(x);
printf("%.2lf \n", result); //result: 0.90

/* Similarly Replace: sin(x) to cos(); || sec(); || cosec(); || tan(); || cot(); */

```

**round()**;

- ------------------------------

Calculate 'Round or Fraction-less number' from any value from a mathematical equation

Example: 5.36=5 and 5.56=6 and 5.99=6

Example Code:

```
int x=4.6;
double result = sin(x);
printf("%.2lf \n", result); //result: 4.00

```

**ceil()**; **floor()**;

-------------------------------

Calculate 'Ceiling and floor' from any value from a mathematical equation

Work with Ceiling and floor formula from 'Discreate math'.

--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--

-7 -6 -5 -4 -3 -2 -1  0  1  2  3  4  5  6  7

Always different between 'Ceiling and floor' is 1. (Ceiling-floor=1)

(Ceiling) Example: 5.36=6 and 5.12=6 and 5.99=6 [find nearest large integer value]

(floor)    Example: 5.36=5 and 5.56=5 and 5.99=5  [find nearest small integer value]

Example Code: (Ceiling)

```
int x=4.6;
double result = ceil(x);
printf("%.2lf \n", result); //result: 5.00

```

Example Code: (floor)

```
int x=4.6;
double result = floor0(x);
printf("%.2lf \n", result); //result: 4.00

```

**trunc()**;

- ------------------------------

Convert 'Integer' from float or fraction number.

Example Code:

```
int x=6.6;
double result = sin(x);
printf("%.2lf \n", result); //result: 6.00

```

**rand()**;

- ------------------------------

Create Random numbers.

Example:

```
#include <stdio.h>
#include <stdlib.h>  //Using header file for random numbers

int main()
{
    for (int i=1; i<=5; i++){
        int randonNum = rand(); //Random numbers create
        printf(" Random Number: %d \n", randonNum);
    }
    return 0;
}

```

OR

```
#include <stdio.h>
#include <stdlib.h>  //Using header file for random numbers

int main()
{
    for (int i=1; i<=5; i++)
    {
        //calc. remainder upto 4 and +1. bcz, random num, create 0 to up so, +1.
        int randonNum = rand()%5 +1;
        printf(" Random Number: %d \n", randonNum);
    }
    return 0;
}

```

**|||||||||||||||||||||||||||| String**

# strlen(); strcpy(); strcat(); strcmp(); strrev(); strupr(); strlwr();

- **--------------------------------------------------------------------------** [lib./header: <cstring>]

Working for String DataType.

**strlen()**;

- ------------------------------

Calculate the String length.

Example Code:

```
char name [] = "Nazrull";
int len = strlen(name);
printf("Length: %d", len);

```

**strcpy()**;

- ------------------------------

Copy string Using function.

Example Code:

```
char source [] = "Michael Scofield";
char destination [100];
strcpy(destination, source);
printf("Check 'strcpy()' for 'destination': %s \n", destination);

```

**strcat()**;

- ------------------------------

String Concatenation by using function. (Adding Every Characters)

Example Code:

```
char name1 [] = "Michael ";
char name2 [] = "Scofield";
strcat(name1, name2);
printf("Print the Concatenation: %s \n", name1);

```

OR

```
char name1 [] = "Michael ";
strcat(name1, "Scofield");
printf("Print the Concatenation: %s \n", name1);

```

**strcmp()**;

- ------------------------------

Compare different different String for check they equal or not.

Example Code:

```
char name1 [50] = "Michael ";
char name2 [] = "Scofield";
int result = strcmp(name1, name2); //If both string are same then return '0'
if(result == 0)
    printf("String are equal");
else
    printf("String aren't equal");

```

**strrev()**;

- ------------------------------

Reverse String from given string.

Example Code:

```
char name [] = "Michael Scofield";
strrev(name); //Only Support One parameter
printf("The reverse string is: %s", name);

```

**strupr()**;

- ------------------------------

For UpperCase Letter from given string.

Example Code:

```
char name [] = "Michael Scofield";
strupr(name); //Only Support One parameter
printf("The UpperCase string is: %s", name);

```

**strlwr()**;

- ------------------------------

For Lowercase Letter from given string.

Example Code:

```
char name [] = "Michael Scofield";
strlwr(name); //Only Support One parameter
printf("The Lowercase string is: %s", name);

```

# **USER-DEFINED FUNCTION()**:

============================================

============== **Custom function()** =================

It is called User-defined function. here,

(1). 'Arguments' gets input and 'Return-type' return output.

(2). 'Arguments': one or more than Arguments.

(3). Program run/starts in 'Main function'.

(4). 'Main function' set the values of Arguments/Parameters for 'User-defined function'.

(5). 'Main function' called 'User-defined function'. then we gets result from 'User-defined function'

Syntax:

ReturnType Function_Name **(**Arguments**)**

 **{**

 //Code block . . .

**}**

Example:

[1]

```
int summation (int a, int b){ //User-defined Function
    return a+b;
}

int main() //Main Function & starts to run a program
{
    int num1=5, num2=13;
    int result;

    /*Set the values of Arguments for 'User-defined function' and called it for run. */
    result=summation(num1, num2);
    printf(" The summation is: %d \n", result); //Out: 18
    return 0;
}

```

OR

```
int summation (int a, int b){ //User-defined Function
    return a+b;
}

int main() //Main Function & starts to run a program
{
    int num1=5, num2=13;
    printf(" The summation is: %d \n", summation(num1, num2)); //Out: 18
    return 0;
}

```

OR

```
int summation (int a, int b){ //User-defined Function
    return a+b;
}

int main() //Main Function & starts to run a program
{
    printf(" The summation is: %d \n", summation(5, 13)); //Out: 18
    printf(" The summation is: %d \n", summation(6, 14)); //Out: 20
    return 0;
}

```

OR

```
int summation (int a, int b){ //User-defined Function
            return a+b;
}

int main() //Main Function & starts to run a program
{
    summation(5, 13);
    printf(" The summation is: %d \n", summation()); //Out: 18
    return 0;
}

```

**# Void() function**:

- --------------------------------------------------

It is called Void User-defined function. here,

(1). 'Void' is ReturnType of function

(2). 'Void' does not return values of calculation

Syntax:

void Function_Name **(**Arguments**)**

**{**

//Code block . . .

**}**

Example:

[1] Function (using void)

```
void summation (int a, int b){ //User-defined Function & using 'Void' ReturnType
    int result;
    result=a+b;
    printf(" The summation is: %d \n", result);
}

int main() //Main Function & starts to run a program
{
    summation(5, 13); //Function Call
    return 0;
}

```

**# Recursive function()**

- --------------------------------------------------

Recursion is the process of repeating items in a self-similar way.

if a program allows you to call a function inside the same function,

then it is called a recursive call of the function.

# Two Part: (i). recursive call (ii). base case

----------

Input --> | Function |  --> Output --

^               ----------                         |

|                                                       |

|---<------- Call by itself <--------- |

Example:

[1]

```
int fact(int n){   //User-defined Function
    if(n==1)       //Base case of recursion function
        return 1;
    else
        return n * fact(n-1);   //Recursive Call
}

int main()   //Main Function & starts to run a program
{
    result=fact(5);
    printf(" Factorial is: %d \n",result); /Out: 120
    return 0;
}

```

=========================   ==================

+                  C H A P T E R                   [ H ]                   IS                   # **Structure, Union, Enum, Typedef**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

**# Structure**

============================================

Structure is a collection of variables of different types under a single name

- A Structure is a user User-defined DataType in C/C++

Diagram:

Step 1:

--> Structure <--

____________________________________________________

|    User-defined DataType + Variables Declare    |

------------------------------------------------------

Step 2:

Create Structure_Variables

Step 3: Assign Structure_Variables Values

Step 4: Ready to work

Systax:

[1] Global Structure -------------------------------------------------

struct structure_name **{**       //Create Structure

Structure_Variables     //Declare DataType with variable

**};**

@main function**()**   //Call to main function

**{**

// Local Variable

structure_name variable_name;         //Create structure variable

variable_name.Structure_Variables    //Insert/Assign Values

/* Code block. . .

printf **(**"FormatSpecifier", variable_name.Structure_Variables**)**;

....

*/

**}**

[OR] Global Structure + Global Variables ------------------------------

struct structure_name **{**         //Create Structure

Structure_Variables        //Declare DataType with variable

**};**

  // Global Variables

structure_name variable_name;          //Create structure variable

variable_name.Structure_Variables     //Insert/Assign Values

@main function**()**   //Call to main function

**{**

/* Code block. . .

printf("FormatSpecifier", variable_name.Structure_Variables);

....

*/

**}**

[2] Local Structure --------------------------------------------------

@main function**()**       //Call to main function

**{**

struct structure_name **{**        //Create Structure

Structure_Variables //Declare DataType with variable

**};**

// Local Variables

structure_name variable_name;         //Create structure variable

variable_name.Structure_Variables    //Insert/Assign Values

/* Code block...

  printf **(**"FormatSpecifier", variable_name.Structure_Variables**)**;

  ....

*/

 **}**

Example:

[1] ------- Global Structure + Local Variables -------------

```
struct teacher{  //Create Structure
    int age;
    float salary;
};

int main()  //main function & starts to run a program
{
    struct teacher info1, info2; //Create structure variable
    info1.age = 26;       //Insert/Assign Values
    info2.salary = 1560.90;

    printf("Teacher age: %d \n", info1.age);
    printf("Teacher salary: %.2f \n", info2.salary);
    return 0;
}

```

[2] ------- Input Structure Elements -----------------------

```
struct teacher{
    int age;
    float salary;
};

int main()    //main function & starts to run a program
{
    struct teacher info1, info2;

    // Input Structure Elements
    printf("Teacher age: ");
    scanf("%d", &info1.age);
    printf("Teacher salary: ");
    scanf("%f", &info2.salary);

    // Showing Result
    printf("Teacher age: %d \n", info1.age);
    printf("Teacher salary: %.2f \n", info2.salary);
    return 0;
}

```

[3] ------- Initialized values to Structure Variables --------

```
struct teacher{
    int age;
    float salary;
};

int main()            //main function & starts to run a program
{
    struct teacher info1 = {26, 1687.362}; // Initialize Structure Variables
    struct teacher info2, info3;

    //Structure Element Assignment
    info2.age=27;
    info2.salary=1547.369;

    //Structure Variable Assignment
    info3 = info2;

    printf("Information 1: \n");
    printf("Teacher age: %d \n", info1.age);
    printf("Teacher salary: %.2f \n", info1.salary);

    printf("Information 2: \n\n");
    printf("Teacher age: %d \n", info2.age);
    printf("Teacher salary: %.2f \n", info2.salary);

    printf("Information 3: \n\n");
    printf("Teacher age: %d \n", info3.age);
    printf("Teacher salary: %.2f \n", info3.salary);
    return 0;
}

```

[4] ------------------ Structure Comparison ------------------

```
struct teacher{
    int age;
    float salary;
};

int main()   //main function & starts to run a program
{
    struct teacher info1 = {26, 1687.362};
    struct teacher info2, info3;

    //Structure Element Assignment
    info2.age=27;
    info2.salary=1547.369;

    //Structure Variable Assignment
    info3 = info2;

    if(info1.age==info2.age && info1.salary == info2.salary)
        printf(" Information1 == Information2");
    else
        printf(" Information1 != Information2");
    return 0;
}

```

[5] -------------------- Array of Structure -------------------

```
struct teacher{
    int age;
    float salary;
};

int main()     //main function & starts to run a program
{
    struct teacher info[3]; //Create Structure Array
    int i;

    //Insert values to structure_array
    for(i=0; i<3; i++){
        printf(" Enter Information %d : \n", i+1);
        printf(" Enter Age: ");
        scanf("%d", &info[i].age);
        printf(" Enter Salary: ");
        scanf("%f", &info[i].salary);
    }

    //Showing values from structure_array
    for(i=0; i<3; i++){
        printf("\n\n Information %d : \n", i+1);
        printf(" Age: %d \n", info[i].age);
        printf(" Salary: %.2f \n", info[i].salary);
    }
    return 0;
}

```

[OR] ---------- Structure_Array within Structure ---------------

```
struct teacher{
    char name[50];
    int age;
    float salary;
};

int main()          //main function & starts to run a program
{
    struct teacher info[3]; int i;

    //Insert values to structure_array
    for(i=0; i<3; i++){
        printf("\n Enter Information %d : \n", i+1);
        printf(" Enter Name: ");
        fflush(stdin); //for using gets() function
        gets(info[i].name);
        printf(" Enter Age: ");
        scanf("%d", &info[i].age);
        printf(" Enter Salary: ");
        scanf("%f", &info[i].salary);
    }

    //Showing values from structure_array
    for(i=0; i<3; i++){
        printf("\n\n Information %d : \n", i+1);
        printf(" Name: %s \n", info[i].name);
        printf(" Age: %d \n", info[i].age);
        printf(" Salary: %.2f \n", info[i].salary);
    }
    return 0;
}

```

[6] --------- Passing Structure_Variables to a function ---------

```
struct teacher{ //Create Structure
    char name[50];
    int age;
    float salary;
};

//function declare
void display (struct teacher in){   // void f_name(struct structure_name parameter)
    printf("\n Name: %s \n", in.name);
    printf(" Age: %d \n", in.age);
    printf(" Salary: %.2f \n", in.salary);
}

//main function & starts to run a program
int main()
{
    struct teacher info1, info2;

    strcpy(info1.name, "Michael Scofield"); //bcz, string doesn't directly initialize
    info1.age=26;
    info1.salary=2569.90;
    display(info1);

    strcpy(info2.name, "Jonior LJ");
    info2.age=15;
    display(info2);
    return 0;
}

```

**# Union**

============================================

- Like structures, union is a User-defined Datatype.
- In Union, all members share the same/single memory location
- Memory location size: highest priority of all variables

What are Application of union?

- Union can be useful in many situations where we want to use same memory for two or more members.

Example: Binary tree

- ** **Different between structure and union**

<----------- Memory Size ----------->

[#] Structure

```
struct basic
{
    char ch;   // 1 byte + priority 4
    int x;     // 4 byte + priority 3
    float x;   // 4 byte + priority 2
    double x;  // 8 byte + priority 1
};

struct basic ver_name;
[ver_name = 1+4+4+8 = 15 bytes] //memory size

```

[#] Union

```
union basic
{
    char ch;   // 1 byte + priority 4
    int x;     // 4 byte + priority 3
    float x;   // 4 byte + priority 2
    double x;  // 8 byte + priority 1
};

union basic ver_name;
[ver_name = 1+4+4+8 = 8 bytes] //memory size because, highest priority of all variables

```

Systax:

[1] Global Union -------------------------------------------------

union union_name **{**      //Create Union

union_Variables      //Declare DataType with variable

**};**

@main function**()**        //Call to main function

  **{**

 // Local Variable

union_name variable_name;         //Create union variable

variable_name.Union_Variables   //Insert/Assign Values

/* Code block. . .

printf **(**"FormatSpecifier", variable_name.Union_Variables**)**;

....

*/

**}**

Example:

[1] Share same memory location

```
union basic{  //Create Union
    int x, y;
};

//@main function()
int main(){
    union basic verName;
    verName.x=10;
    printf(" X = %d \n", verName.x);
    printf(" Y = %d \n", verName.y);
}
//Result: x=10; y=10;

```

**# Enum (Enumeration)**

============================================

An enumeration is a User-defined data type that consists of integral constants.

- Consists of integral constants.
- Many Constants work together.
- Sequence maintainance of integral constants. (0 to endOfNumbers)

Syntax:

enum enum_varName **{**var1, var2, var3, ....., varN**}**;

Example:

[1] Declare Enum

```
enum days_of_week {Sun, Mon, Tue, Wed, Thu, Fri, Sat};

```

[2] Initialize enum_variable and their initialize position

```
enum days_of_week{
    Sun, Mon, Tue, Wed, Thu, Fri, Sat
};

int main()
{
    enum days_of_week day1, day2;
    day1=Sun;
    day2=Tue;

    printf(" Size of day1 = %d \n", day1);  //Out: 0
    printf(" Size of day2 = %d \n", day2);  //Out: 2
}

```

**# Typedef (Type Definition)**

============================================

Renaming to User-defined/Primitive Datatype

Syntax:

typedef DataTypeName NewDataType_Name;

NewDataType_Name VarName;

Example:

[1] Renaming Primitive DataType Name

```
typedef char Letter;  //Renaming 'char' to 'Letter'
Letter ch;
ch='A';
printf(" Ch = '%c' \n", ch);

```

[2] Renaming Custom DataType Name

```
struct teach{
    char name[20];
    int age;
};

int main()
{
    typedef struct teach Teacher;      //Renaming DataType Name
    Teacher t = {"Rayhan Kabir", 45600};
    printf(" Teacher Name: %s \n", t.name);
    printf(" Teacher's age: %d \n", t.age);
}

```

=========================   ==================

+                  C H A P T E R                   [ I ]                   IS                   # **Pointer**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

Pointer is a variable that stores/points the address of another variable. Here,

1. '&' symbol is used to get the address of the variable.

2. '*' symbol is used to get the value of the variable that the pointer is pointing to.

------------------

Variable Name ---> |     x      |     y     |

------------------

Value -------------->|     5    |    10     |

------------------

VariableAddress--->|   100   |   104   |

------------------

Why Pointer?

> Pointers are powerful features of C and (C++) Programming

that differentiates it from other popular Programming Language like: Java and Python

> Using pointer makes the software more efficient cause it works with memory management.

> But Excessive usage may take the application less understandable.

Syntax:

Datatype *Var_Name;

Example:

[1] Initialize Pointer Variable

```
int x = 5, y = 10;
int *p; //Create pointer variable
p=&x; //assign 'x' variable_address to pointer_variable

printf(" Value of x = %d \n", x);     //Out: 5
printf(" Address of x = %d \n", &x);  //Out: 6356728 (ChangeForPC)
printf(" Address of p = %d \n", p);   //Out: 6356728 (ChangeForPC)
printf(" Content of p = %d \n", *p);  //Out: 5
printf(" Address of p variable = %d \n", &p);  //Out: 6356724 (ChangeForPC)

```

[2] Swapping 2 numbers by using pointer

```
int x = 5, y = 10, temp;
int *p1, *p2; //Create pointer variable
p1=&x;   //assign 'x' variable_address to pointer_variable
p2=&y;   //assign 'y' variable_address to pointer_variable

// Swapping x and y
temp = *p1;
*p1 = *p2;
*p2 = temp;
printf(" Value of x = %d \n", x);
printf(" Value of y = %d \n", y);

```

=========================   ==================

+                  C H A P T E R                   [ J ]                   IS                   #  **File**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

> In C Programming, File is place on disk where a group of related data is stored.

> File is a structure which is stored in 'stdio.h' header.

File Operation:

1. Creating a new file

2. Opening existing file

3. Closing a file

4. Reading from and writing information to a file

[**#**] **Built-In functions**:

```
To write something in a file              To read something in a file
----------------------------              ---------------------------
fputc()                                   fgetc()
fputw()                                   fgetw()
fputs()                                   fgets()
fprintf()                                 fscanf()
fwrite()                                  fread()

Others function
----------------------------
fopen() = File Create / File Open [ fopen("File_name", "Operation_mode") ]

fclose() = File Close/Exit [ fclose(fileName/pointerName) ]
gets()   = User Input (Only for String) [ gets(variable/stringName) ]
feof()   = File_end_of: Goto end of file [ feof(pointerName) ]

```

[**#**] **Operation Mode**:

```
Mode || Description
-----------------------
r    = Open a file for read only. Opens an existing text file for reading purpose.
w    = Open a file for write only. If it does not exist, then a new file is created.
       Here your program will start writing content from the beginning of the file.
       [ Write new file or write existing file & replacing existing contents ]
a    = Open a file for write only. Opens a text file for writing in appending mode.
       The existing data in file is preserved. File pointer starts at the end of
       the file. Creates a new file if the file doesn't exist.
       [ Write existing file & overwrite existing contents ]
r+   = Open a file for read/write. If the file exist, loads it into memory and
       set up a pointer to the first character in it.
       It the file does not exist it returns null.
w+   = Open a file for read/write. If the is present, it first destroys the file
       to zero length if it exists, Otherwise; creates a file if it does not exist.
a+   = Open a file for read/write. It creates the file if it does not exist.
       The reading will start from the beginning but writing can only be appended.

```

Syntax:

FILE *****name_of_file;

Example:

[1] File Open and Close

```
FILE *file; //create a pointer for 'file operation'
file = fopen("basic.txt", "w"); //new file create

if(file==NULL){
    printf(" File doesn't exist");
}else{
    printf(" File is created");
    fclose(file); //file close
}

```

[2] Writing to a file using fputc()

> Writing characters, single by single in existing file

> fputc(stringName, pointerName);

```
FILE *file; //create a pointer for 'file operation'
char name[20] = "Hello World!";
int length = strlen(name); //finding string length
file = fopen("basic.txt", "w"); //new file create

if(file==NULL){
    printf(" File doesn't exist");
}else{
    printf(" File is created \n");

    /* ----- file written by string ----- */
    for(int i=0; i<length; i++){
        fputc(name[i], file); //writing characters, single by single in a file
    }
    printf(" File is written successfully \n");
    fclose(file); // file close
}

```

[3] Writing to a file by using fputs()

> Writing full string in a file

> fputs(stringName, pointerName);

```
FILE *file; //Create a pointer for 'file operation'
char name[20]; //Create Character String
file = fopen("basic.txt", "w"); //New file create

if(file==NULL){
    printf(" File doesn't exist");
}
else{
    printf(" File is created \n");

    /* ----- file written by string ----- */
    printf(" Enter the string: ");
    gets(name);   //Input String and passing string to 'Character String'
    fputs(name, file);  //writing full string in a file
    printf(" File is written successfully \n");
    fclose(file); //file close
}

```

[4] Writing to a file by using fprintf()

> Written by more than variable by one function

> fprintf(filePointer, FormatSpecifier, VarName);

```
FILE *file; //Create a pointer for 'file operation'
char fname[50]; //Create Character String
char lname[50]; //Create Character String
int age;
file = fopen("basic.txt", "w"); //New file create

if(file==NULL){
    printf(" File doesn't exist");
}
else{
    printf(" File is created \n");

    /* ----- file written by user and passing file ----- */
    printf(" Enter the first name: ");
    gets(fname);   //Input String and passing to 'CharacterString'
    printf(" Enter the last name: ");
    gets(lname);   //Input String and passing to 'CharacterString'
    printf(" Enter Age: ");
    scanf("%d", &age);
    fprintf(file, "Full Name: %s %s \nAge: %d", fname, lname, age);
    printf(" File is written successfully \n");
    fclose(file); //file close
}

```

[5] Reading a file by using fgetc()

> Reading an existing file with single character by character by fgetc()

> feof(pointerName)

```
FILE *file; //create a pointer for 'file operation'
char ch;
file = fopen("basic.txt", "r"); //reading existing file

if(file==NULL){
    printf(" File doesn't exist");
}
else{
    printf(" File is created \n");

    /*  Reading a file single character by character by fgetc() */
    while(!feof(file))
    {
        ch = fgetc(file);  //reading from existing file & passing characters to variable
        printf("%c", ch);
    }
    fclose(file); //file close
}

```

[6] Reading a file by using fgets();

> How many string (length) can be reading in a line from an existing file.

> fgets(VarName, Size, filePointer)

```
FILE *file; //create a pointer for 'file operation'
char ch[50];
file = fopen("basic.txt", "r"); //reading existing file

if(file==NULL){
    printf(" File doesn't exist");
}
else{
        printf(" File is opened \n");

        /*  Reading a file single character by character by fgetc() */
        while( !feof(file)){
            fgets(ch, 20, file); //read from an existing file & pass String to StringVar
            printf("%s \n", ch);
        }
        fclose(file); //file close
}

```

[7] Reading a file by using fscanf();

> Read single/multiple word(s) by single/multiple FormatSpecifier (with _var) by fscanf()

> fscanf(filePointer, FormatSpecifier, VarName);

```
FILE *file; //create a pointer for 'file operation'
char ch[50];
file = fopen("basic.txt", "r"); //reading existing file

if(file==NULL){
    printf(" File doesn't exist");
}
else{
    printf(" File is opened \n");
    /* Read single/multiple word(s) by single/multiple FormatSpecifier (with _var) */
    while( !feof(file))
    {
        fscanf(file, "%s", &ch); //read an existing file & pass String to StringVar.
        printf("%s \n", ch);
    }
    fclose(file); //file close
}

```

=========================   ==================

+                  C H A P T E R                   [ K ]                   IS                   #  **Preprocessor**

=========================   ==================╰☆☆_______________▀▄▀▄▀▄☆☆╮

Preprocessor like as header.

> Firstly, compiler execute header/Preprocessor .

> Secondly, compiler execute source code.

Syntax:

  **#**define Preprocessor_Name Code/Values

Example:

[1] Create a simple preprocessor by using #define

```
#include <stdio.h>
#define name "Hello World!"

int main()
{
    printf(" %s \n", name);
    return 0;
}
//Out: Hello World!

```

[2] How to create a simple preprocessor by using #define

```
#include <stdio.h>
#define name printf(" Hello World! \n");

int main()
{
    name //call the preprocessor
    return 0;
}
//Out: Hello World!

```

**# Create a User-defined header file**

============================================

Steps:

1. Create a header file like as "example.h"

2. Create a preprocessor like as

#define PreprocessorName Code/Values (Example)

3. Write the code/values within 'PreprocessorName' like as

#define name "Michael Scofield" (Example)

4. Call the header file:

#include <stdio.h>

#include "header_location"

5. Call the preprocessor in main source code:

int main**()**

**{**

 // . . . Call the preprocessor

**}**

" Let's done! "

Syntax:

#include "locationOfHeaderFile"

Example:

[1] How

```html
#include <stdio.h>
#include "E:\DocX\Codeblocks\header\header.h" //get header file

int main()
{
    printf(" Name: %s \n", name); //call the preprocessor
    printf(" Age: %d \n", age);   //call the preprocessor
    return 0;
}

/* ===== Output / Result: */

/* Input:
------------------
> Input from "header.h" file with specific location
  Example: #include "E:\DocX\Codeblocks\header\header.h"
  Input Values:
  ------------------------------------
  #define name "Michael Scofield"
  #define age 39
*/

/* Output:
------------------
      Name: Michael Scofield
      Age: 39
*/

```