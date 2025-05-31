# EXP NO:11 C PROGRAM TO CONVERT BINARY TO DECIMAL USING FUNCTION WITH RETURN TYPE AND WITHOUT ARGUMENTS.

## Aim:
To write a C program to convert a binary number to its decimal equivalent using a function that returns a value and takes no arguments.
## Algorithm:
1. Define a function convert() that:
2. Reads the binary number as a long long integer inside the function (since no arguments).
3. Initializes dec (decimal result), i (position index), and rem (remainder).
4. Extracts each digit of the binary number from right to left and converts it to decimal using dec += rem * pow(2, i).
5. Returns the decimal value dec.
6. In main(), declare variable n to store binary number input.
7. Read the binary number from user using scanf.
8. Call convert() function and print the decimal equivalent.
9. End the program with return 0.
 
## Program:
```
#include <stdio.h>
#include <math.h>

int convert(long long);

int main()
{
  long long n;
  scanf("%lld", &n);
  printf("%lld in binary = %d in decimal", n, convert(n));
  return 0;
}

int convert(long long n) 
{
  int dec = 0, i = 0, rem;

  while (n!=0)
  {
    rem = n % 10;
    n /= 10;
    dec += rem * pow(2, i);
    ++i;
  }

  return dec;
}
```
## Output:

![image](https://github.com/user-attachments/assets/e41769cc-9b53-431f-afa3-2e3b4ae98321)

## Result:
Thus, the program to convert binary to decimal using a function with return type and without arguments is verified successfully.
 

# EXP NO:12  C PROGRAM TO GENERATE FIBONACCI SERIES USING DO-WHILE LOOP
## Aim:
To write a C program to generate the Fibonacci series for a given number n using a do-while loop.
## Algorithm:
1. Declare and initialize variables: a = 0, b = 1, i = 2, and sum = 0.
2. Read the input number n (number of terms).
3. Print the first two Fibonacci numbers: a and b.
4. Use a do-while loop until i < n:
  Calculate sum = a + b.
  Print sum.
  Update a = b and b = sum.
  Increment i.
5. End the program with return 0.
 
## Program:
```
#include<stdio.h>
int main()
{
    int i=2,a=0,b=1,n,sum=0;
    scanf("%d",&n);
    printf("%d %d",a,b);
    do
    {
       
       sum=a+b;
       printf(" %d",sum);
       a=b;
       b=sum;
       i++;
    }
    while(i<n);
    return 0;
}
```


## Output:

![image](https://github.com/user-attachments/assets/c25fb50f-8203-421e-8178-ed38c9dc413c)
## Result:
Thus, the program to generate Fibonacci series using a do-while loop is verified successfully.


# EXP NO:13 C PROGRAM TO PRINT ELEMENTS PRESENT AT EVEN POSITIONS IN AN ARRAY
## Aim:
To write a C program to read n elements into an array and print the elements present at even positions.

## Algorithm:
1.	Read the number of elements n.
2. Declare an integer array of size n.
3. Use a loop to read n elements into the array.
4. Loop through the array starting from index 1 (second element, as indexing starts at 0), incrementing by 2, to access elements at even positions.
5. Print those elements.
6. End the program with return 0.

 ## Program:
```
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(int i = 1; i < n; i += 2) {
        printf("%d ", arr[i]);
    }
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/4891eea9-c6f4-4e45-8cbb-f8083deab0c9)

## Result:
Thus, the program to print elements present at even positions in an array is verified successfully.


 
# EXP NO:14 C PROGRAM TO DELETE THE FIRST ELEMENT IN AN ARRAY
## Aim:
To write a C program to delete the first element from an array by shifting all other elements one position to the left.

## Algorithm:
1. Define a function deleteFirstElement that takes the array and its size as arguments.
2. Loop from the second element to the last, copying each element one position to the left.
3. In main(), initialize the array and calculate its size.
4. Call deleteFirstElement to remove the first element.
5. Decrement the size by one to reflect the deletion.
6. Print the updated array elements from index 0 to size-1.
7. End the program with return 0.

## Program:
```
#include <stdio.h>
void deleteFirstElement(int arr[], int size) {
    for (int i = 1; i < size; i++) {
        arr[i - 1] = arr[i];
    }
}
int main() {
    int arr[] = {10, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    int size = sizeof(arr) / sizeof(arr[0]);
    deleteFirstElement(arr, size);
    size--;  
    for (int i = 1; i < size; i++) {
        printf("%d ", arr[i]);
    }
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/719721dc-9ed1-402d-b003-9f58896fa359)


## Result:
Thus, the program to delete the first element in an array is verified successfully.
 
# EXP NO:15 C PROGRAM TO CHECK WHETHER A NUMBER IS AN ARMSTRONG NUMBER OR NOT

## Aim:
To write a C program to check whether the given number is an Armstrong number or not.

## Algorithm:
1. Read the input number a.
2. Initialize variables for sum and temporary storage.
3. Extract each digit of the number using modulus operator and cube it.
4. Add the cube of each digit to a sum.
5. Compare the sum with the original number.
6. If equal, print that the number is an Armstrong number; else print it is not.
7. End the program.

## Program:
```
#include<stdio.h>
int main()
{
    int a,b,i;
    scanf("%d",&a);
    for(i=1;i<a;i++)
    {
        b=a*a*a;
    }
    if(b==a)
    printf("%d is armstrong number",a);
    else
    printf("%d is not a armstrong number",a);
}
```

## Output:

![Screenshot 2025-05-31 212133](https://github.com/user-attachments/assets/45a0a20d-510e-4dd7-bd92-e9dff1d48926)


## Result:
Thus, the program to check whether a number is an Armstrong number or not is verified successfully.
