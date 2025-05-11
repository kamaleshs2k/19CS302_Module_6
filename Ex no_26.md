# EX 26 C program demonstrating a self-referential structure where an employee has a pointer to their manager.
## DATE: 11/05/2025
## AIM:
To write a C program to demonstrate a self-referential structure where an employee has a pointer to their manager.

## Algorithm
1.Start the program and define a structure Employee that contains fields for employee details and a pointer to another Employee (manager).

2.Declare instances of the structure for employees and managers.

3.Read the employee details and assign a pointer to the manager's details.

4.Display the employee's details along with the manager's details using the pointer.

5.End the program.

## Program:
```
/*
C program demonstrating a self-referential structure where an employee has a pointer to their manager.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

struct Employee
{
    int empno;
    char name[50];
    struct Employee *manager;  // Pointer to another Employee (self-referential structure)
};

int main()
{
    struct Employee emp1, emp2;  // Two employees (one with manager, the other as manager)

    // Employee 1 details
    printf("Enter Employee 1 details:\n");
    printf("Employee Number: ");
    scanf("%d", &emp1.empno);
    printf("Employee Name: ");
    scanf("%s", emp1.name);

    // Employee 2 details (manager)
    printf("\nEnter Employee 2 (Manager) details:\n");
    printf("Employee Number: ");
    scanf("%d", &emp2.empno);
    printf("Employee Name: ");
    scanf("%s", emp2.name);

    // Set Employee 1's manager to Employee 2
    emp1.manager = &emp2;

    // Display Employee 1's details and their manager's details
    printf("\nEmployee 1 Details:\n");
    printf("Employee Number: %d\n", emp1.empno);
    printf("Employee Name: %s\n", emp1.name);
    printf("Manager's Name: %s\n", emp1.manager->name);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/60405279-c0e2-46e6-8524-d1447620f26e)


## Result:
Thus the program was executed and the output was verified successfully.
