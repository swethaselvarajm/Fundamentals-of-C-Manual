# EXP NO:16 C PROGRAM TO PERFORM BITWISE AND AND OR OPERATIONS OF TWO INTEGERS
## Aim:
To write a C program to perform bitwise AND and bitwise OR operations on two integer inputs.

## Algorithm:
1. Start the program and declare two integer variables a and b.
2. Read two integers from the user.
3. Perform bitwise AND operation using the & operator and display the result.
4. Perform bitwise OR operation using the | operator and display the result.
5. End the program with return 0.
 
## Program:
```
#include <stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    printf("Bitwise-AND result is = %d\n", a&b);
    printf("Bitwise-OR result is = %d", a|b);
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/ef35e91f-866b-4674-a8d6-1607912ca9ea)

## Result:
Thus, the program to perform bitwise AND and OR operations of two integers is verified successfully.

 
# EXP NO:17  C PROGRAM TO CHECK THE POLLUTION CONDITION USING SIMPLE IF STATEMENT

## Aim:
To write a C program to check the pollution condition based on the pollution value. Assume the pollution cutoff is 3.

## Algorithm:
1. Start the program.
2. Declare an integer variable a.
3. Read the pollution value from the user.
4. If the value is less than or equal to 3, print "Good Condition".
5. If the value is greater than 3, print "Bad Condition".
6. End the program.
 
## Program:

```
# include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a<4)
    {
     printf("Good Condition");   
    }
    else if(a>4)
    {
     printf("Bad Condition");   
    }
    else
    {
      printf("Bad Condition");  
    }
}
```

## Output:

![image](https://github.com/user-attachments/assets/a47c229e-332d-46c8-9ac3-77be332ae4f8)

## Result:
Thus, the program to check the pollution condition using a simple if statement is verified successfully.

 
# EXP NO:18 C PROGRAM TO READ A STRING
## Aim:
To write a C program to read and display a string entered by the user.

## Algorithm:
1. Start the program.
2. Declare a character array to store the input string.
3. Use scanf() to read the string from the user.
4. Display the string using printf() with a message.
5. End the program.
 
## Program:

```
#include <stdio.h>
int main() {
    char str[100]; 
    scanf("%s", str);
    printf("You have entered %s.\n", str);
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/9bec94c9-a313-4d6a-aacf-6a111a5f194d)

## Result:
Thus, the program to read and display a string is verified successfully.


# EXP NO:19 C PROGRAM TO COUNT THE TOTAL NUMBER OF WORDS IN A GIVEN STRING USING FUNCTION
## Aim:
To write a C program to count the total number of words in a given string using a function.

## Algorithm:
1. Start the program.
2. Declare a character array to store the input string.
3. Read the string using fgets() to support multi-word input.
4. Create a function countWords() to count words in the string:
5. Initialize a counter and a flag to track if inside a word.
6. Loop through each character:
7. If the character is not a space and not already in a word, increase the word count.
8. If the character is a space, reset the in-word flag.
9. Print the result.
10. End the program.
 
## Program:
```
#include <stdio.h>
#include<string.h>
#include <ctype.h>
int countWords(char str[]) {
    int count = 0;
    int inWord = 0;
    for (int i = 0; str[i] != '\0'; i++) {
        if (!isspace(str[i])) {
            if (!inWord) {
                inWord = 1;  
                count++;
            }
        } else {
            inWord = 0;  
        }
    }
    return count;
}

int main() {
    char str[100];
    fgets(str, sizeof(str), stdin);
    str[strcspn(str, "\n")] = 0;
    int wordCount = countWords(str);
    printf("%d\n", wordCount);

    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/ba207fcb-ca68-47bc-8721-5df79e43a042)

## Result:
Thus, the program to count the total number of words in a given string using a function is verified successfully.

# EXP NO:20 C PROGRAM TO PERFORM THE BASIC LEFT AND RIGHT SHIFT OPERATION FOR A 22 INTEGER NUMBER

## Aim:
To write a C program to perform left and right shift operations on an integer value using bitwise operators.

## Algorithm:
1. Start the program.
2. Initialize an integer variable n with the value 22.
3. Perform right shift operation using n >> 2 and store the result in a.
4. Perform left shift operation using n << 2 and store the result in b.
5. Print the values after left and right shift operations.
6. End the program.

## Program:

```
#include<stdio.h>
#include<string.h>
int main()
{
    int n=22,a,b;
    
    a=n>>2;
    b=n<<2;
    printf("After Left Shift Operation value of a is:%d",b);
    printf("\nAfter Right Shift Operation value of a is:%d",a);
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/9e54fd0f-ce58-40ef-b00b-14adb705d76b)

## Result:
Thus, the program to perform the basic left and right shift operations using bitwise operators is verified successfully.
