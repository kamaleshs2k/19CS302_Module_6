# EX 28 C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.
## DATE: 11/05/2025
## AIM:
To write a C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.

## Algorithm
1.Start the program and define an enum for various named integer constants.

2.Declare variables of the enum type.

3.Assign values to the variables based on the enum constants.

4.Display the values of the enum constants.

5.End the program.  

## Program:
```
/*
C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

// Define an enum for days of the week
enum Weekdays
{
    Sunday = 1,  // Starting from 1
    Monday,
    Tuesday,
    Wednesday,
    Thursday,
    Friday,
    Saturday
};

int main()
{
    enum Weekdays today;  // Declare an enum variable

    // Assign a value from the enum
    today = Wednesday;

    // Display the value of the enum constant
    printf("The day of the week is: %d\n", today);  // Prints the integer value of Wednesday (4)

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/61831a6c-c84b-403c-b784-4b4879cb3a8c)


## Result:
Thus the program was executed and the output was verified successfully.
