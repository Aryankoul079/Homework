 C to calculate the area and perimeter of different geometric shapes. 


     #include <stdio.h>

    int main() {
    int choice;
    float length, width, radius, area, perimeter;

    printf("Choose a geometric shape:\n");
    printf("1. Rectangle\n");
    printf("2. Circle\n");
    printf("3. Square\n");
    printf("Enter your choice (1-3): ");
    scanf("%d", &choice);

    switch (choice) {
        case 1: // Rectangle
            printf("Enter length and width of the rectangle: ");
            scanf("%f %f", &length, &width);
            area = length * width;
            perimeter = 2 * (length + width);
            printf("Area of the rectangle: %.2f\n", area);
            printf("Perimeter of the rectangle: %.2f\n", perimeter);
            break;

        case 2: // Circle
            printf("Enter the radius of the circle: ");
            scanf("%f", &radius);
            area = 3.14 * radius * radius;
            perimeter = 2 * 3.14 * radius;
            printf("Area of the circle: %.2f\n", area);
            printf("Perimeter of the circle: %.2f\n", perimeter);
            break;

        case 3: // Square
            printf("Enter the side length of the square: ");
            scanf("%f", &length);
            area = length * length;
            perimeter = 4 * length;
            printf("Area of the square: %.2f\n", area);
            printf("Perimeter of the square: %.2f\n", perimeter);
            break;

        default:
            printf("Invalid choice! Please enter a number between 1 and 3.\n");
            break;
    }

    return 0;
    }


Output of the program:


![image](https://github.com/AklavyaSangra/Homework/assets/146859465/b4f39f4e-0c0d-4309-b67c-66a67b3634d3)

    
