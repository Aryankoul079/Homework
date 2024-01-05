Write a c code for 2D arry.
    
    #include <stdio.h>

    // Function to print elements in a 2D array
    void print2DArray(int rows, int cols, int arr[rows][cols]) {
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            printf("%d\t", arr[i][j]);
        }
        printf("\n");
    }
    }

    int main() {
    int rows, cols;

    // Input: Number of rows and columns in the 2D array
    printf("Enter the number of rows: ");
    scanf("%d", &rows);
    printf("Enter the number of columns: ");
    scanf("%d", &cols);

    // Input: 2D array elements
    int arr[rows][cols];
    printf("Enter the elements of the 2D array:\n");
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &arr[i][j]);
        }
    }

    // Output: Print the 2D array
    printf("Elements in the 2D array:\n");
    print2DArray(rows, cols, arr);

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/48c00016-2c61-410b-8783-880096e9dea4)
