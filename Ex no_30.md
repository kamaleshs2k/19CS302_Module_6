# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE: 11/05/2025
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
1.Start the program and dynamically allocate memory for an array of 3 integers using malloc().

2.Read 3 integers from the user and store them in the array.

3.Use realloc() to resize the array and add space for 1 more integer.

4.Read the 4th integer and add it to the array.

5.Calculate and display the sum of all elements in the array, then free the allocated memory.

## Program:
```
/*
C program to add two integer elements in an array using realloc() and that array already has three elements.

Developed by: Kamalesh S
RegisterNumber: 212223060108 
*/
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int *arr, i;

    arr = (int*)malloc(3 * sizeof(int));

    printf("Enter 3 integers:\n");
    for(i = 0; i < 3; i++)
    {
        scanf("%d", &arr[i]);
    }

    arr = (int*)realloc(arr, 4 * sizeof(int));

    printf("Enter the 4th integer:\n");
    scanf("%d", &arr[3]);

    int sum = 0;
    for(i = 0; i < 4; i++)
    {
        sum += arr[i];
    }

    printf("The sum of the array elements is: %d\n", sum);

    free(arr);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/9de1e0d0-707e-475d-9469-4709fc75ed0a)


## Result:
Thus the program was executed and the output was verified successfully.
