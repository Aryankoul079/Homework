Write a c program for fibonacci series.

    #include <stdio.h>
    int main()
    {
    
    int n1 = 0, n2 = 1, n3, i, number;
    
    printf("Enter the number of elements: ");
    scanf("%d", &number);

    printf("%d %d ", n1, n2); // Separate the initial two numbers by a space, not a newline

    for (i = 2; i < number; ++i) { // Removed the semicolon and added the loop condition
        n3 = n1 + n2;
        printf("%d ", n3); // Separate the Fibonacci numbers by a space
        n1 = n2;
        n2 = n3;
    }

    return 0;




 Output of the program:![image](https://github.com/AklavyaSangra/Homework/assets/146859465/560c38fc-188a-4311-8bca-50dca9104256)


