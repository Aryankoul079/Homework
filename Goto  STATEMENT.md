Write a program of a simple example of goto statement.


    #include<stdio.h>
    //main function heading
    void main()
    {
    //assignment of value
    int i=0;
    //loop is starting(statement)
    loop_start:
    //if statement
    if(i<6)
    {
    //output statement
    printf("%d",i);
    //increment statement
    i++;
    //goto loop start (statement)--->closed
    goto loop_start;
    } 
    //output statement for loop finished
    printf("\n Loop finished.\n");
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/e903c435-009a-434e-b71e-45d87d6c01c4)
