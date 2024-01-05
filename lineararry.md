    #include <stdio.h>

    int linearSearch(int arr[], int size, int key) {
	int i;
    for ( i = 0; i < size; i++) {
        if (arr[i] == key) {
            return i;
        }
    }
    return -1; 
    }
    int main() {
    int arr[] = {2, 4, 6, 8, 10, 12, 14, 16};
    int size = sizeof(arr) / sizeof(arr[0]);
    int key;
    printf("Enter the element to search: ");
    scanf("%d", &key);
    int index = linearSearch(arr, size, key);
    if (index != -1) {
        printf("Element found at index %d.\n", index);
    } else {
        printf("Element not found in the array.\n");
    }
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/451f25d1-b39c-4fcf-bcd2-9976ab05be8b)

    
    
