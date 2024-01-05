Write a c code finding the distance between two points.

   
    #include<stdio.h>
    #include<math.h>
    void main()
    {
    float a,b,c,d,e;
    printf("Enter the value of a");
    scanf("%f",&a);
    printf("Enter the value of b");
    scanf("%f",&b);
    printf("Enter the value of c");
    scanf("%f",&c);
    printf("Enter the value of d"); 
    scanf("%d",&d);
    float dist;
    dist=sqrt(b-a)*(b-a)+(c-d)*(c-d);
    printf("The distance between two point=%.2f",dist);
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/6e4bc621-1a77-42d9-877a-f9111b9788d0)




