Write a program to use various string operation.


    #include <stdio.h>
    #include <string.h>

    int main() {
    char str1[100], str2[100];

    // Input the first string
    printf("Enter the first string: ");
    gets(str1);

    // Input the second string
    printf("Enter the second string: ");
    gets(str2);

    // Calculate and display the length of the first string
    printf("Length of the first string: %lu\n", strlen(str1));

    // Concatenate and display the two strings
    strcat(str1, str2);
    printf("Concatenated string: %s\n", str1);

    // Compare the two strings
    int compareResult = strcmp(str1, str2);
    if (compareResult == 0) {
        printf("The strings are equal.\n");
    } else if (compareResult < 0) {
        printf("The first string is lexicographically smaller than the second string.\n");
    } else {
        printf("The first string is lexicographically greater than the second string.\n");
    }

    // Copy and display the second string
    strcpy(str1, str2);
    printf("Copied string: %s\n", str1);

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/c4f75576-1d76-4726-8f46-7eda26269e3a)



