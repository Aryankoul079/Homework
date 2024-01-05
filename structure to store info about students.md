write a c code that uses structure to store info about students make and calculate total marks


    #include <stdio.h>

    // Define a structure for storing student information
    struct Student {
    char name[50];
    float marks[3]; // Assuming 3 subjects
    float totalMarks;
    };

    int main() {
    int numStudents;

    // Input the number of students
    printf("Enter the number of students: ");
    scanf("%d", &numStudents);

    // Declare an array of structures to store student information
    struct Student students[numStudents];

    // Input information for each student
    for (int i = 0; i < numStudents; ++i) {
        printf("\nEnter details for student %d:\n", i + 1);

        // Input student name
        printf("Enter student name: ");
        scanf("%s", students[i].name);

        // Input marks for each subject
        printf("Enter marks for three subjects:\n");
        for (int j = 0; j < 3; ++j) {
            printf("Subject %d: ", j + 1);
            scanf("%f", &students[i].marks[j]);
            students[i].totalMarks += students[i].marks[j]; // Calculate total marks
        }
    }

    // Display information and total marks for each student
    printf("\nStudent Details and Total Marks:\n");
    for (int i = 0; i < numStudents; ++i) {
        printf("\nStudent %d\n", i + 1);
        printf("Name: %s\n", students[i].name);
        for (int j = 0; j < 3; ++j) {
            printf("Subject %d Marks: %.2f\n", j + 1, students[i].marks[j]);
        }
        printf("Total Marks: %.2f\n", students[i].totalMarks);
    }

    return 0;
    }


Output of the program:



![image](https://github.com/AklavyaSangra/Homework/assets/146859465/db85606a-3068-4f5d-9b04-79b813cbc06d)
