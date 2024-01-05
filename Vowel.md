Write a c program to check whether an alphabet is vowels or consonants.


    #include<stdio.h>
    void main()
    {
    char A;
    printf("Enter the Alphabet:");
    scanf("%C",&A);
    if(A=='a'||A=='e'||A=='i'||A=='o'||A=='u'||A=='A'||A=='E'||A=='I'||A=='O'||A=='U')
    {
        printf("The alphabet is vowel",A);
    }
    else
    {
        printf("the alphabet is consonant",A);
    }
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/931352a3-c880-4c30-ba18-64f39fbda783)
