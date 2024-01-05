Write a c program to check whether the number is prime or not.


    #include <stdio.h>
    int main()
    {
    int i,num,a= 0; 
    printf("Enter the number:");
    scanf("%d", &num);
    for (i = 2; i <= num/2; i++)
    {
        if (num % i == 0)
        {
            a++;
            break;
        }
    }  
    if (a == 0 && num != 1)
    {
        printf("%d is a Prime number", num);
    }
    else
    {
        printf("%d is not a Prime number", num);
    }
    return 0;
    }
  
    
    Output of the program:


   ![image](https://github.com/AklavyaSangra/Homework/assets/146859465/65f166e3-c6c5-499c-a165-bfcfb516ab77)



    
