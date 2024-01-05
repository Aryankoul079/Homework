write a C program for a calculator using a switch case.


    #include <stdio.h>

    int main() {
    char operator;
    double num1, num2, result;

    // Input operator
    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &operator);

    // Input two numbers
    printf("Enter two numbers: ");
    scanf("%lf %lf", &num1, &num2);

    // Perform operation based on the operator
    switch (operator) {
        case '+':
            result = num1 + num2;
            printf("%.2lf + %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '-':
            result = num1 - num2;
            printf("%.2lf - %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '*':
            result = num1 * num2;
            printf("%.2lf * %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                printf("%.2lf / %.2lf = %.2lf\n", num1, num2, result);
            } else {
                printf("Error! Division by zero is not allowed.\n");
            }
            break;
        default:
            printf("Error! Invalid operator.\n");
            break;
    }

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/51db17fc-0e42-4d8b-aae7-11e3d04c6a1d)
