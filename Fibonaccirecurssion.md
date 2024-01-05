Function to calculate Fibonacci sequence using recursion.
       
         
    #include <stdio.h>


    int fibonacci(int n) {
    if (n <= 1) {
        return n;
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
    }

    int main() {
    int n;

    // Input: Number of terms in the Fibonacci sequence
    printf("Enter the number of terms in the Fibonacci sequence: ");
    scanf("%d", &n);

    // Output: Fibonacci sequence
    printf("Fibonacci sequence:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", fibonacci(i));
    }

    return 0;
    }


Output of the progrma:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/f01b1c85-9158-4696-bdd3-f7e7033ddbba)
