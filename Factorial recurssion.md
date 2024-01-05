    #include <stdio.h>
    unsigned int factorial(unsigned int n)
    {
    int result = 1, i;

    for (i = 2; i <= n; i++) {
        result *= i;
    }
 
    return result;
    }
    int main()
    {
    int num = 5;
    printf("Factorial of %d is %d", num, factorial(num));
    return 0;
    }


Output of the progrma:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/1abf9623-d981-46a0-9947-62cc47b6743d)

    
