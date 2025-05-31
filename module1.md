# EXP NO:1 C PROGRAM TO FIND THE ASCII VALUE OF A GIVEN CHARACTER

## Aim:
To write a C program to find and display the ASCII value of a given character.

## Algorithm:
1. Declare a character variable ch.
2. Read the character input from the user using scanf.
3. Print the ASCII value of the character using %d format specifier.
4. Return 0.
 
## Program:
```
#include<stdio.h>
int main() {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);
    printf("ASCII value of %c is %d", ch, ch);
    return 0;
}
```


## Output:

![image](https://github.com/user-attachments/assets/6de3ebfc-3a92-4b84-803d-f38c230b7453)



## Result:
Thus, the program is verified successfully. 



# EXP NO:2 C PROGRAM TO CHECK WHETHER THE GIVEN NUMBER IS EVEN AND GREATER THAN 50 OR NOT USING NESTED IF
## Aim:
To write a C program using nested if statements to check whether a given number is even and whether it is greater than or equal to 50.

## Algorithm:
1. Declare an integer variable n.
2. Read the value of n from the user using scanf.
3. Use the first if to check whether n is even (i.e., n % 2 == 0).
4. If the number is even, use nested if to check:
5. If n >= 50, print: "The number is even" and "The number is greater than or equal to 50".
6. Else, print: "The number is even" and "The number less than 50".
7. If the number is not even, print: "The number is NOT an even number".
8. Return 0.
 
## Program:
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);

    if (n % 2 == 0) {
        printf("The number is even\n");
        if (n >= 50) {
            printf("The number is greater than or equal to 50");
        } else {
            printf("The number less than 50");
        }
    } else {
        printf("The number is NOT an even number");
    }

    return 0;
}


```
## Output:
![image](https://github.com/user-attachments/assets/c2072fea-01fb-429a-8785-402c6f096455)

## Result:
Thus, the program is verified successfully


 
# EXP.NO:3 C PROGRAM TO FIND THE DIFFERENCE BETWEEN SIMPLE INTEREST AND COMPOUND INTEREST

## Aim:
To write a C program to calculate the simple interest and compound interest for given principal, rate, and time, and to find the difference between them.

## Algorithm:
1. Declare float variables: p (principal), r (rate), y (time), SI (simple interest), CI (compound interest), amt (amount), and diff (difference).
2. Read the values of p, y, and r from the user using scanf.
3. Calculate simple interest using the formula:
SI = (p * y * r) / 100
4. Calculate amount for compound interest using the formula:
amt = p * pow((1 + r / 100), y)
5. Calculate compound interest:
CI = amt - p
6. Print simple interest, compound amount, and the difference between compound interest and simple interest.
7. Return 0.
 
## Program:
```
#include <stdio.h>
#include <math.h>

int main() {
    float p, y, r, SI, CI, amt, diff;

    printf("Enter Principal, Time (years), and Rate of Interest:\n");
    scanf("%f %f %f", &p, &y, &r);

    SI = (p * y * r) / 100;
    amt = p * pow((1 + r / 100), y);
    CI = amt - p;
    diff = CI - SI;

    printf("Simple Interest = %.2f", SI);
    printf("\nAmount = %.2f", amt);
    printf("\nAmount Difference between simple interest & Compound Interest = %.2f", diff);

    return 0;
}

```
## Output:
![image](https://github.com/user-attachments/assets/8dad07e4-8bb4-4b84-b2a7-04172890fee4)

## Result:
Thus, the program is verified successfully
 


# EXP NO:4   C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS POSITIVE

## Aim:
To write a C program to read a value and check whether it is a positive number or not.

## Algorithm:
1. Declare an integer variable A.
2. Read the value of A from the user using scanf.
3. Use an if statement to check if A > 0:
4. If true, print "a is positive number".
5. End the program with return 0.

 ## Program:
```
#include <stdio.h>

int main() {
    int A;
    printf("Enter a number: ");
    scanf("%d", &A);

    if (A > 0) {
        printf("a is positive number");
    }

    return 0;
}
```
## Output:

![image](https://github.com/user-attachments/assets/2bf58921-a313-4196-99d2-457489008d53)

## Result:
Thus, the program is verified successfully



# Ex No 5 : C PROGRAM TO SIMULATE ARITHMETIC OPERATORS (+, -) USING SWITCH STATEMENT

## Aim:
To write a C program to perform arithmetic operations (addition and subtraction) using the switch statement.

## Algorithm:
1. Declare integer variables a, b, and res, and a character variable op.

2. Read the input values for a, op, and b from the user using scanf.

3. Use a switch statement to evaluate the operator op:

4. If op is '+', calculate res = a + b and print the result.

5. If op is '-', calculate res = a - b and print the result.

6. For any other operator, print "Invalid Input".

7. End the program with return 0.

## Program:
```
#include<stdio.h>
int main()
{
    int a,b,res;
    char op;
    scanf("%d %c %d", &a, &op, &b);
    switch(op)
    {
        case '+':
            res = a + b;
            printf("Result = %d",res);
            break;
        case '-':
            res=  a - b;
            printf("Result = %d",res);
            break;
        default: printf("Invalid Input");    
    }
}
```
## Output:

![image](https://github.com/user-attachments/assets/9ac58886-29c6-4e61-999b-1a7f85d4f45a)

## Result:
Thus, the program is verified successfully
