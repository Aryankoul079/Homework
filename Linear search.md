program to search an element in an arry using linear search.


    #include <stdio.h>

    int linearSearch(int arr[], int size, int target) {
    for (int i = 0; i < size; ++i) {
        if (arr[i] == target) {
            return i; // Return the index where the element is found
        }
    }
    return -1; // Return -1 if the element is not found
    }

    int main() {
    int size, target;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &size);

    // Input array elements
    int array[size];
    printf("Enter %d elements:\n", size);
    for (int i = 0; i < size; ++i) {
        scanf("%d", &array[i]);
    }

    // Input the element to be searched
    printf("Enter the element to be searched: ");
    scanf("%d", &target);

    // Perform linear search
    int index = linearSearch(array, size, target);

    // Display the result
    if (index != -1) {
        printf("Element %d found at index %d.\n", target, index);
    } else {
        printf("Element %d not found in the array.\n", target);
    }

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/b6f230c2-6f5b-450f-9a06-61346538db56)
