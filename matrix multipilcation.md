Write a c code for matrix muktiplication


    #include <stdio.h>
    void multiplyMatrices(int firstMatrix[][10], int secondMatrix[][10], int result[][10], int rowsFirst, int colsFirst, int rowsSecond, int colsSecond) {
    for (int i = 0; i < rowsFirst; ++i) {
        for (int j = 0; j < colsSecond; ++j) {
            result[i][j] = 0;
        }
    }
    for (int i = 0; i < rowsFirst; ++i) {
        for (int j = 0; j < colsSecond; ++j) {
            for (int k = 0; k < colsFirst; ++k) {
                result[i][j] += firstMatrix[i][k] * secondMatrix[k][j];
            }
        }
    }
    }
    void displayMatrix(int matrix[][10], int rows, int cols) {
    for (int i = 0; i < rows; ++i) {
        for (int j = 0; j < cols; ++j) {
            printf("%d\t", matrix[i][j]);
        }
        printf("\n");
    }
    }

    int main() {
    int rowsFirst, colsFirst, rowsSecond, colsSecond;

    
    printf("Enter the number of rows and columns for the first matrix: ");
    scanf("%d %d", &rowsFirst, &colsFirst);
    printf("Enter the number of rows and columns for the second matrix: ");
    scanf("%d %d", &rowsSecond, &colsSecond);
    if (colsFirst != rowsSecond) {
        printf("Matrix multiplication is not possible.\n");
        return 0;
    }

    int firstMatrix[10][10], secondMatrix[10][10], result[10][10];
    printf("Enter elements of the first matrix:\n");
    for (int i = 0; i < rowsFirst; ++i) {
        for (int j = 0; j < colsFirst; ++j) {
            printf("Enter element a%d%d: ", i + 1, j + 1);
            scanf("%d", &firstMatrix[i][j]);
        }
    }
    printf("Enter elements of the second matrix:\n");
    for (int i = 0; i < rowsSecond; ++i) {
        for (int j = 0; j < colsSecond; ++j) {
            printf("Enter element b%d%d: ", i + 1, j + 1);
            scanf("%d", &secondMatrix[i][j]);
        }
    }
    multiplyMatrices(firstMatrix, secondMatrix, result, rowsFirst, colsFirst, rowsSecond, colsSecond);
    printf("\nResultant matrix:\n");
    displayMatrix(result, rowsFirst, colsSecond);

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/d7bc2c60-0d4a-4ec4-b890-a2db084cbba9)

    

