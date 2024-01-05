Write a program to set an arry using double sort.


    #include <stdio.h>
    #include <stdlib.h>

    // Comparison function for ascending order
    int compareAsc(const void *a, const void *b) {
    return (*(int *)a - *(int *)b);
    }

    // Comparison function for descending order
    int compareDesc(const void *a, const void *b) {
    return (*(int *)b - *(int *)a);
    }

    int main() {
    int size;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &size);

    // Input array elements
    int array[size];
    printf("Enter %d elements:\n", size);
    for (int i = 0; i < size; ++i) {
        scanf("%d", &array[i]);
    }

    // Sort in ascending order
    qsort(array, size, sizeof(int), compareAsc);

    // Display sorted array in ascending order
    printf("Sorted array in ascending order:\n");
    for (int i = 0; i < size; ++i) {
        printf("%d ", array[i]);
    }
    printf("\n");

    // Sort in descending order
    qsort(array, size, sizeof(int), compareDesc);

    // Display sorted array in descending order
    printf("Sorted array in descending order:\n");
    for (int i = 0; i < size; ++i) {
        printf("%d ", array[i]);
    }
    printf("\n");

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/379967e0-6ad4-4f87-b02d-ba65d18383fe)
