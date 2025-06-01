# EXP NO 26: C PROGRAM TO CALCULATE THE AREA OF A TRIANGLE USING POINTERS
## Aim:
To write a C program to calculate the area of a triangle using pointer variables.

## Algorithm:
1. Start the program.
2. Declare two float variables a (base) and b (height).
3. Declare two pointers *c and *d pointing to a and b respectively.
4. Read the base and height values using scanf().
5. Calculate the area using the formula: (base × height) / 2 through pointers.
6. Print the result using the pointer values.
7. End the program.

## Program:
```
# include<stdio.h>
int main()
{
    float a,b,*c=&a,*d=&b;
    scanf("%f %f",&a,&b);
    float area = ((*c)*(*d))/2;
    printf("area of the triangle with base %f and height%f=%f",*c,*d,area);
}
```
## Output:

![image](https://github.com/user-attachments/assets/f5dafbcb-1eae-4eaf-9d51-33702c720d75)

## Result:
Thus, the program to calculate the area of a triangle using pointers is verified successfully.
 

# EXP.NO 27: C PROGRAM TO COUNT TOTAL NUMBER OF EVEN ELEMENTS IN AN ARRAY USING MALLOC()
## Aim:
To write a C program that counts the total number of even elements in a dynamically allocated array using malloc().

## Algorithm:
1. Start the program.
2. Declare an integer pointer ptr and a variable n for the number of elements.
3. Allocate memory dynamically using malloc() for n integers.
4. Initialize the array elements directly: 3, 5, 32, 21, 20.
5. Use a loop to check each element.
6. If the element is divisible by 2, increment the even counter.
7. Print the total number of even elements.
8. Free the dynamically allocated memory.
9. End the program.
 
## Program:
```
#include<stdio.h>
#include<stdlib.h>
int main()
{
int i, n=5, even = 0, *ptr;
ptr = (int*)malloc(n*sizeof(int));
ptr[0] = 3;
ptr[1] = 5;
ptr[2] = 32;
ptr[3] = 21;
ptr[4] = 20;
for(i=0;i<n;i++)
{
if(ptr[i]%2 == 0)
{
even++;
}
}
printf("Total even elements: %d\n", even);
return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/929be39a-28c5-4ab2-995c-fafe75c5a683)

## Result:
Thus, the program to count total number of even elements in an array using malloc() is verified successfully.
 
# EXP NO:28 C PROGRAM TO STORE AND DISPLAY STUDENT INFORMATION USING STRUCTURE
## Aim:
To write a C program that stores and displays the information of a student using structures.
## Algorithm:
1. Start the program.
2. Define a structure student with members: name, rollno, and marks.
3. Declare a variable of the structure.
4. Use scanf() to read name, roll number, and marks.
5. Use printf() to display the stored information.
6. End the program.
 
## Program:
```
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
   
struct student
{
    char name[50];
    int rollno;
    float marks;
}s[1];

int main()
{
    int i;
    for(i=0;i<1;i++)
    {
        scanf("%s",s[i].name);
        scanf("%d",&s[i].rollno);
        scanf("%f",&s[i].marks);
    }
    for(i=0;i<1;i++)
    {
        printf("Displaying Information:\n");
        printf("Name: %s\n",s[i].name);
        printf("Roll number: %d\n",s[i].rollno);
        printf("Marks: %.1f",s[i].marks);
    }
};
```

## Output:
![image](https://github.com/user-attachments/assets/3490c0d9-65d8-4294-bdd1-5d21438cc5b4)


## Result:
Thus, the program to store the student information and display it using structure is verified successfully.


# EXP NO:29 C PROGRAM TO CALCULATE WORKER PAYMENT USING STRUCTURE POINTER

## Aim:
To write a C program to read the name, daily wages, and number of days of a worker, and calculate the total payment using a structure pointer.

## Algorithm:
1. Start the program.
2. Define a structure Worker with members: name, dailyWages, and numberOfDays.
3. Declare a structure variable and a pointer to it.
4. Read input values using the structure pointer.
5. Calculate payment as dailyWages * numberOfDays.
6. Display the name and total payment.
7. End the program.
 
## Program:
```
#include <stdio.h>

struct Worker {
    char name[50];
    float dailyWages;
    int numberOfDays;
};

int main() {
    struct Worker worker;
    struct Worker *workerPtr = &worker;
    scanf("%s", workerPtr->name);
    scanf("%f", &(workerPtr->dailyWages));
    scanf("%d", &(workerPtr->numberOfDays));

    float payment = workerPtr->dailyWages * workerPtr->numberOfDays;

    printf("Name of Worker : %s\n", workerPtr->name);
    printf("Payment of Worker : %.f\n", payment);

    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/57315a93-65a6-4b2d-9a1b-abc22982f4dc)


## Result:
Thus, the program to calculate the payment of a worker using structure pointer is verified successfully.



# EXP NO:30 C PROGRAM TO MULTIPLY TWO INTEGERS USING POINTERS AND CALLOC()


## Aim:
To write a C program to multiply two integer numbers using pointers with memory dynamically allocated using calloc().

## Algorithm:
1. Start the program.
2. Declare two integer variables a and b.
3. Declare a pointer p to store the result.
4. Read two integers from the user.
5. Allocate memory for the result using calloc().
6. Perform multiplication and store the result in the allocated memory.
7. Print the result.
8. Free the allocated memory (optional but recommended).
9. End the program.

## Program:
```
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int a,b,*p;
    scanf("%d%d",&a,&b);
    p=(int*)calloc(2,sizeof(int*));
    *p=a*b;
    printf("The result is %d",*p);
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/312c195f-a264-4c79-8a02-5d728ce8793b)

## Result:
Thus, the program to multiply two integers using pointers and dynamic memory allocation with calloc() is verified successfully.
