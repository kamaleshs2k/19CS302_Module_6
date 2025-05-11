# EX 29 C program to create two float variables using calloc() and find minimum among them.
## DATE: 11/05/2025
## AIM:
To write a C program to create two float variables using calloc() and find minimum among them.

## Algorithm
1.Start the program and declare two float pointers.

2.Use calloc() to dynamically allocate memory for the two float variables.

3.Read the values for both variables from the user.

4.Compare the two values to find the minimum.

5.Display the minimum value and free the dynamically allocated memory.   

## Program:
```
/*
C program to create two float variables using calloc() and find minimum among them.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>
#include <stdlib.h>

int main()
{
    float *num1, *num2;

    // Dynamically allocate memory using calloc
    num1 = (float*)calloc(1, sizeof(float));
    num2 = (float*)calloc(1, sizeof(float));

    if (num1 == NULL || num2 == NULL)  // Check for memory allocation failure
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    // Input values for num1 and num2
    printf("Enter the first float number: ");
    scanf("%f", num1);
    printf("Enter the second float number: ");
    scanf("%f", num2);

    // Find and display the minimum value
    if (*num1 < *num2)
    {
        printf("The minimum value is: %.2f\n", *num1);
    }
    else
    {
        printf("The minimum value is: %.2f\n", *num2);
    }

    // Free the dynamically allocated memory
    free(num1);
    free(num2);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/d1b4579a-fb42-4962-8c79-d4cd97fa02a0)


## Result:
Thus the program was executed and the output was verified successfully.
