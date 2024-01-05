Write a program to find the sum of array elements by using pointers.


    #include<stdio.h>
    void main()
    {
    int n=5,sum=0;
    //taking integer array
    int a[]={10,20,30,40,50};
    //pointer variable declaration
    int*P=a;
    //for loop statement
    for(int i=0;i<n;i++)
    {
    //statement for sum of array elements
    sum=sum+(*P);
    //increment statement
    P++;
    }
    //output statement
    printf("Sum of array elements =%d",sum);
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/742fdc2f-c5fd-450f-933a-b901d2fdbeec)



