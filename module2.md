# EXP NO:6 C PROGRAM TO PRINT THE STRING "WELCOME" N NUMBER OF TIMES

## Aim:
To write a C program to print the string "WELCOME" a given number of times using a for loop.

## Algorithm:
1. Declare two integer variables n and i.
2. Read the value of n from the user using scanf.
3. Use a for loop that runs from i = 1 to i <= n.
4. Inside the loop, print the string "WELCOME".
5. End the program with return 0.
 
## Program:
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    for(i=1;i<=n;i++)
    {
        printf("WELCOME\n");
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/b4209adb-82eb-4866-881d-e360eba4d1f6)

## Result:
Thus, the program is verified successfully
 
# EXP NO:7 C PROGRAM TO PRINT TRIANGULAR NUMBER PATTERN USING LOOP
## Aim:
To write a C program to print a triangular number pattern using nested loops.

## Algorithm:
1. Declare three integer variables: n, i, and j.
2. Read the value of n (number of rows) from the user using scanf.
3. Use an outer for loop from i = 1 to i <= n to handle rows.
4. Use an inner for loop from j = 1 to j <= i to print numbers in each row.
5. Print the numbers in increasing order for each row and add a newline after each row.
6. End the program with return 0.
 
## Program:

```
#include<stdio.h>
int main()
{
    int n,i,j;
    scanf("%d",&n);
    for(i=1;i<=n;i++)
    {
        for(j=1;j<=i;j++)
        {
            printf("%d ",j);
        }
        printf("\n");
    }
}
```

## Output:
![image](https://github.com/user-attachments/assets/a67eaef6-86cf-487d-8cbe-23b699d67b7e)

## Result:
Thus, the program is verified successfully

# EXP NO:8 C PROGRAM TO PERFORM MULTIPLICATION AND DIVISION USING FUNCTIONS
## Aim:
To write a C program to perform multiplication and division of two numbers a and b using functions.

## Algorithm:
1. Define a function fun() that:
2. Declares variables a, b, mul, and div.
3. Reads two integer values a and b from the user.
4. Calculates multiplication (mul = a * b) and division (div = a / b).
5. Prints the multiplication and division results.
6. In the main() function, call the fun() function.
7. End the program with return 0.
 
## Program:
```
#include<stdio.h>
void fun();
int main()
{
    fun();
}
void fun()
{
    int a,b,mul,div;
    scanf("%d%d",&a,&b);
    mul=a*b;
    div=a/b;
    printf("Multiplication: %d",mul);
    printf("\nDivision: %d",div);
}

```
## Output:

![image](https://github.com/user-attachments/assets/9e2dbdde-d7d0-43dc-8ef7-7d146c81bd6c)


## Result:
Thus, the program is verified successfully
 
# EXP NO:9 C PROGRAM TO CHECK WHETHER A NUMBER IS PALINDROME OR NOT USING FOR LOOP
## Aim:
To write a C program to check if the input number is a palindrome or not using a loop.

## Algorithm:
1. Declare integer variables n, a, r, and s (sum) initialized to 0.
2. Read the number n from the user.
3. Store the original number in variable a.
4. Use a loop to reverse the number:
5. Extract the last digit r by n % 10.
6. Update s = s * 10 + r.
7. Remove the last digit from n by n = n / 10.
8. After the loop ends, compare the original number a with the reversed number s.
9. If they are equal, print "Palindrome Number". Otherwise, print "Not a Palindrome Number".
10. End the program with return 0.
 
## Program:
```
#include<stdio.h> 
int main()
{
    int n,a,r,s=0;
    scanf("%d",&n);
    a=n;
    do
    {
        r=n%10;
        s=s*10+r;
        n=n/10;
    }while(n>0);
    if(a==s)
    {
        printf("Palindrome Number");
    }
    else
    {
         printf("Not a Palindrome Number");
    }
    return 0;
}    
```
## Output:
![image](https://github.com/user-attachments/assets/d705aec0-9082-4d0d-99be-55d94da9c1d8)

## Result:
Thus, the program is verified successfully

# EXP NO:10 C PROGRAM TO GENERATE FIBONACCI SERIES USING FUNCTION WITH ARGUMENTS AND WITHOUT RETURN TYPE

## Aim:
To write a C program to generate Fibonacci series up to n terms using a function that takes arguments but does not return any value.
## Algorithm:
1. Define a function fibonacci(int n) that:
2. Initializes variables a = 0, b = 1, and c.
3. Prints the first two Fibonacci numbers 0 and 1.
4. Uses a for loop from i = 2 to i < n to calculate the next Fibonacci numbers:
  c = a + b
  Print c
  Update a = b and b = c
5. In main(), declare integer n.
6. Read the number n (number of Fibonacci terms) using scanf.
7. Call the function fibonacci(n).
8. End the program with return 0.

## Program:

```
#include <stdio.h>
void fibonacci(int n);
int main()
{
    int n;
    scanf("%d ",&n);
    fibonacci(n);
    return 0;
}

void fibonacci(int n)
{
    int a=0,b=1,c,i;
    
    printf("%d %d",a,b);
    for(i=2;i<n;i++)
    {
        c=a+b;
        printf(" %d",c);
        a=b;
        b=c;
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/77b3f5a9-d54f-4e87-8265-b1c01521ad51)

## Result:
Thus, the program is verified successfully
