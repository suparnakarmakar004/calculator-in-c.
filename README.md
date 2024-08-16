# calculator-in-c.
#include <stdio.h>

int main() {
    char operator;
    float num1, num2;

    
    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &operator);

    
    printf("Enter two numbers: ");
    scanf("%f %f", &num1, &num2);

    
    if (operator == '+') {
        printf("%.2f + %.2f = %.2f\n", num1, num2, num1 + num2);
    } else if (operator == '-') {
        printf("%.2f - %.2f = %.2f\n", num1, num2, num1 - num2);
    } else if (operator == '*') {
        printf("%.2f * %.2f = %.2f\n", num1, num2, num1 * num2);
    } else if (operator == '/') {
      
        if (num2 != 0) {
            printf("%.2f / %.2f = %.2f\n", num1, num2, num1 / num2);
        } else {
            printf("Error: Division by zero is not allowed.\n");
        }
    } else {
        printf("Error: Invalid operator\n");
    }

    return 0;
}

