 C program to check if a given number is an Armstrong number.


     #include <stdio.h>
    #include <math.h>

    int main() {
    int number, originalNumber, remainder, n = 0, result = 0;

    printf("Enter an integer: ");
    scanf("%d", &number);

    originalNumber = number;

    // Count the number of digits
    while (originalNumber != 0) {
        originalNumber /= 10;
        ++n;
    }

    originalNumber = number;

    // Calculate the sum of nth power of individual digits
    while (originalNumber != 0) {
        remainder = originalNumber % 10;
        result += pow(remainder, n);
        originalNumber /= 10;
    }

    // Check if the number is an Armstrong number
    if (result == number)
        printf("%d is an Armstrong number.\n", number);
    else
        printf("%d is not an Armstrong number.\n", number);

    return 0;
    }


Output of the program:

![image](https://github.com/AklavyaSangra/Homework/assets/146859465/dcc34dae-e023-4a44-8705-f95b6013fc31)

