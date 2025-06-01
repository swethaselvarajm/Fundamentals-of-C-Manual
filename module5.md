# EXP NO:21 C PROGRAM TO PRINT STRING 'COMPUTER' USING POINTER
## Aim:
To write a C program to read and print a string using pointers.

## Algorithm:
1. Start the program.
2. Declare a character array s and a character pointer p.
3. Point p to the base address of s.
4. Read a string using scanf() through the pointer.
5. Print each character of the string using a while loop and pointer traversal.
6. End the program.
 
## Program:
```
#include<stdio.h>
 int main(){
 char s[100],*p;
 p=s;
 scanf("%s",p);
 printf("The entered string is :: ");
 while(*p!='\0')
 printf("%c",*p++);
 return 0;
 }
```

## Output:
![image](https://github.com/user-attachments/assets/e58cdc6b-eb48-482f-9884-39f662ae0c9c)


## Result:
Thus, the program to print the string 'COMPUTER' using pointer is verified successfully.

 
# EXP NO:22 C PROGRAM TO SWAP TWO VALUES USING FUNCTION POINTERS (WITHOUT TEMPORARY VARIABLE)
## Aim:
To write a C program to swap any two values using function and pointers without using a temporary variable.

## Algorithm:
1. Start the program.
2. Declare two integer variables a and b.
3. Read the values of a and b from the user.
4. Define a function swap() that takes two integer pointers.
5. Inside the function, swap values using arithmetic operations without using a temporary variable:
    *x = *x + *y
    *y = *x - *y
    *x = *x - *y
6. Call the function swap(&a, &b) in main().
7. Display the swapped values.
8. End the program.
 
## Program:
```
#include<stdio.h>
 void swap(int *x,int *y){
 int temp;
 temp=*x;
 *x=*y;
 *y=temp;
 }
 int main(){
 int a,b;
 scanf("%d%d",&a,&b);
 printf("Before Swapping a=%d b=%d\n",a,b);
 swap(&a,&b);
 printf("After Swapping a=%d b=%d",a,b);
 return 0;
 }
```

## Output:
![image](https://github.com/user-attachments/assets/0e2873d4-2b39-49fa-8b3f-5946d430cf60)


## Result:
Thus, the program to swap two values using function pointers without using a temporary variable is verified successfully.


 
# EXP NO:23 C PROGRAM TO ADD TWO MATRICES USING 2-DIMENSIONAL ARRAYS
## Aim:
To write a C program to add two matrices using 2-dimensional arrays.

## Algorithm:
1. Start the program.
2. Read the number of rows and columns.
3. Declare three matrices matrix1[row][col], matrix2[row][col], and result[row][col].
4. Read elements of the first matrix.
5. Read elements of the second matrix.
6. Add corresponding elements of the two matrices and store the result in the result matrix.
7. Display the result matrix.
8. End the program.
 
## Program:
```
 #include<stdio.h>
 intmain(){
 introw,col;
 scanf("%d%d",&row,&col);
 intmatrix1[row][col],matrix2[row][col],result[row][col];
 printf("Sumoftwomatrices:\n");
 for(inti=0;i<row;i++){
 for(intj=0;j<col;j++){
 scanf("%d",&matrix1[i][j]);
 }
 }
 for(inti=0;i<row;i++){
 for(intj=0;j<col;j++){
 scanf("%d",&matrix2[i][j]);
 }
 }
 for(inti=0;i<row;i++){
 for(intj=0;j<col;j++){
 result[i][j]=matrix1[i][j]+matrix2[i][j];
 }
 }
 for(inti=0;i<row;i++){
 for(intj=0;j<col;j++){
 printf("%d",result[i][j]);
}
 printf("\n");
 }
 return 0;
 }
```

## Output:
![image](https://github.com/user-attachments/assets/9fdd074f-521e-4a3f-b8a9-a2970811db5d)

## Result:
Thus, the program to add two matrices using 2-dimensional arrays is verified successfully.


 
# EXP NO:24 C PROGRAM TO REPLACE THE SPACES OF A STRING WITH A SPECIFIC CHARACTER

## Aim:
To write a C program to replace the spaces in a string with a specific character.

## Algorithm:
1. Start the program.
2. Read a string using fgets().
3. Read the character to replace spaces.
4. Traverse the string using a for loop.
5. Whenever a space is found (' '), replace it with the given character.
6. Print the modified string.
7. End the program.

## Program:
```
 #include<stdio.h>
 #include<string.h>
 int main(){
 char str[100],ch;
 fgets(str,sizeof(str),stdin);
 scanf("%c",&ch);
 for(int i=0;i<strlen(str);i++){
 if(str[i]==' '){
 str[i]=ch;
 }
 }
 printf("After replacing the space with @ the new string is :\n");
 printf("%s",str);
 return 0;
 }
```

## Output:
![image](https://github.com/user-attachments/assets/0d1136c0-2024-4390-9473-108f70709b19)

## Result:
Thus, the program to replace the spaces of a string with a specific character is verified successfully.

 
# EXP NO 25: C PROGRAM TO CALCULATE SUM OF FIRST 10 NATURAL NUMBERS USING RECURSION

## Aim:
To write a C program to calculate the sum of the first 10 natural numbers using recursion.

## Algorithm:
1. Start the program.
2. Define a recursive function f(n):
    -> If n == 1, return 1.
    -> Otherwise, return n + f(n - 1).
3. In main(), initialize n = 10.
4. Call the recursive function and store the result.
5. Display the result.
6. End the program.

## Program:
```
#include<stdio.h>
 int f(int n)
 {
 if(n==1)
 return 1;
 return (n+f(n-1));
 }
 int main()
 {
 int n,result;
 n=10;
 if(n>0)
 result=f(n);
 printf("Sum = %d",result);
 }
```

## Output:
![image](https://github.com/user-attachments/assets/84f44e2c-20f7-4540-a630-f806d8882c37)

## Result:

Thus, the program to calculate the sum of the first 10 natural numbers using recursion is verified successfully.
