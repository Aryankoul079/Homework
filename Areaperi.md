Write a c program to find area and perimeter of circle,square and rectangle.


    #include<stdio.h>
    void main()
    {float r,l,b,s;
    printf("enter the radius of circle:");
    scanf("%f",&r);
    printf("enter the side the square:");
    scanf("%f",&s);
    printf("enter the lngth of rectangle:");
    scanf("%f",&l);
    printf("enter the breadth of rectangle:");
    scanf("%f",&b);
    float area,peri;
    area=3.14*r*r;
    peri=2*3.14*r;
    printf("the area of circle:%.2f\n",area);
    printf("the perimeter of circle:%.2f\n",peri);
    float arrea,perri;
    arrea=s*s;
    perri=4*s;
    printf("the area of square:%.2f\n",arrea);
    printf("the perimeter of square:%.2f\n",perri);
    float areas,peris;
    areas=l*b;
    peris=2*(l+b);
    printf("area of rectangle:%.2f\n",areas);
    printf("perimeter of rectangle:%.2f\n",peris);
    }



Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/5ba1cce8-54fd-4661-95a5-4575cc45c4ea)



![image](https://github.com/AklavyaSangra/Homework/assets/146859465/ef973c2c-f02f-4b08-aba0-2c84974d2f3a)

