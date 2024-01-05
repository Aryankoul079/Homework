c program to implement an arry of structures for students mark for each student and pass it to function for various operations


    #include <stdio.h>

    // Define a structure for storing student marks
    struct Student {
    char name[50];
    float marks[3]; // Assuming 3 subjects
    };

    // Function to calculate the average marks for a student
    float calculateAverage(struct Student student) {
    float totalMarks = 0;
    for (int i = 0; i < 3; ++i) {
        totalMarks += student.marks[i];
    }
    return totalMarks / 3.0;
    }

    // Function to display details for a student
    void displayDetails(struct Student student) {
    printf("Student Name: %s\n", student.name);
    printf("Subject-wise Marks: %.2f, %.2f, %.2f\n", student.marks[0], student.marks[1], student.marks[2]);
    printf("Average Marks: %.2f\n", calculateAverage(student));
    }

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
        }
    }


Output of the program:



![image](https://github.com/AklavyaSangra/Homework/assets/146859465/295124b4-ca67-4e9e-946c-27f6bb9226af)

    

    // Pass each student to functions for various operations
    for (int i = 0; i < numStudents; ++i) {
        printf("\nDetails for student %d:\n", i + 1);
        displayDetails(students[i]);
    }

    return 0;
    }


Output of the program:



    
