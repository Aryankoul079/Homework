C program that uses a union to store information about a person.


    #include <stdio.h>

    // Define a union to store information about a person
    union PersonInfo {
    char name[50];
    long employeeID;
    long studentID;
    };

    // Define a structure to hold additional details based on the role (employee or student)
    struct PersonDetails {
    int age;
    char role; // 'E' for Employee, 'S' for Student
    union PersonInfo info;
    };

    int main() {
    struct PersonDetails person;

    // Input common details
    printf("Enter person's name: ");
    scanf("%s", person.info.name);
    printf("Enter person's age: ");
    scanf("%d", &person.age);

    // Input role-specific details
    printf("Enter role ('E' for Employee, 'S' for Student): ");
    scanf(" %c", &person.role);

    // Depending on the role, input and display relevant information
    if (person.role == 'E') {
        printf("Enter employee ID: ");
        scanf("%ld", &person.info.employeeID);
        printf("Employee Details:\n");
        printf("Name: %s\n", person.info.name);
        printf("Age: %d\n", person.age);
        printf("Employee ID: %ld\n", person.info.employeeID);
    } else if (person.role == 'S') {
        printf("Enter student ID: ");
        scanf("%ld", &person.info.studentID);
        printf("Student Details:\n");
        printf("Name: %s\n", person.info.name);
        printf("Age: %d\n", person.age);
        printf("Student ID: %ld\n", person.info.studentID);
    } else {
        printf("Invalid role entered.\n");
    }

    return 0;
    }


Output of the program:



![image](https://github.com/AklavyaSangra/Homework/assets/146859465/9df94318-8b2b-4df8-ac56-c9e18e7f563d)

