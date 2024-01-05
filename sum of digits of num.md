Write a c program to find sum of the digits of numbers.


    #include <stdio.h>

    int main() {
    int number, digit, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &number);

    while (number > 0) {
        digit = number % 10;
        sum += digit; 
        number /= 10; 
    }

    printf("The sum of the digits is: %d\n", sum);

    return 0;
    }
    

Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/783dc8ab-4221-4dd5-abea-1f8b685e7774)
