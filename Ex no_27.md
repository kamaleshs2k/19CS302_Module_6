# EX 27 C program that demonstrates the use of typedef to create a new alias name for a data type.
## DATE: 11/05/2025
## AIM:
To write a C program that demonstrates the use of typedef to create a new alias name for a data type.

## Algorithm
1.Start the program and use typedef to create an alias for a data type.

2.Declare a variable using the new alias.

3.Perform some operations or calculations using the variable.

4.Display the result using the typedef alias name.

5.End the program.

## Program:
```
/*
C program that demonstrates the use of typedef to create a new alias name for a data type.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

// Create an alias for the data type 'int' using typedef
typedef int Integer;

int main()
{
    Integer num1, num2, sum;  // Declare variables using the typedef alias

    // Input values for num1 and num2
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);

    // Calculate the sum
    sum = num1 + num2;

    // Display the sum
    printf("The sum of %d and %d is: %d\n", num1, num2, sum);

    return 0;
}


```

## Output:
![image](https://github.com/user-attachments/assets/639e01bd-2ef0-45fb-a2db-41cee0e5e496)



## Result:
Thus the program was executed and the output was verified successfully.
