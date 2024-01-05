write a program to find maximum of n numbers by using for loop.


    int main()
    {
    int limit,num,count,big;
    printf("Enter the limit\n");
    scanf("%d",& limit);
    printf("Enter %d numbers\n",limit);
    for(count=1; count<=limit;count++)
    {
    scanf("%d",&num);
    if(num> big|| count==1)
    {
    big=num;
    }
    }
    printf("Biggest number is%d\n",big);
    return 0;
    }


output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/6edfc249-43ed-49e8-ad00-ddb388c2e60f)



    
