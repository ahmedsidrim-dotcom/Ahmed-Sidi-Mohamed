#include <stdio.h>
#include <math.h> 

int main() {
    double result = 0.0;
    double current_number;
    char operation;
    int first_calculation = 1; 
    int running = 1;         

    printf("                    Scientific Calculator  \n");
    while (running) {
        if (first_calculation) {
                                    // STEP 1: Get the first number 
            printf("\nEnter initial number: ");
            if (scanf("%lf", &result) != 1) {
                printf("Error: Invalid number input.\n");
                
                while (getchar() != '\n');
                continue; 
            }
            first_calculation = 0;
            printf("Current Result: %.2lf\n", result);
        }

                          // STEP 2: Get the operation
        printf("Choose opperation (+, -, *, /, s, c, t, l, r, ^, q): ");
        // Skip whitespace 
        if (scanf(" %c", &operation) != 1) { 
            // Clear input buffer
            while (getchar() != '\n');
            continue; 
        }
            if (operation==q){
                printf("thank you"):
                break;
            }
           
        if (operation == 's' || operation == 'c' || operation == 't' || operation == 'l' || operation == 'r') {
            
            
            if (operation == 'l' && result <= 0) {
                printf("Error: Logarithm undefined for non-positive number.\n");
                continue; 
            }
            
            if (operation == 'r' && result < 0) {
                printf("Error: Square root of a negative number is not real.\n");
                continue; 
            }
            if (operation == 's') {
                result = sin(result);
                printf("Operation: sin(%.2lf)\n", result);
            } else if (operation == 'c') {
                result = cos(result);
                printf("Operation: cos(%.2lf)\n", result);
            } else if (operation == 't') {
                result = tan(result);
                printf("Operation: tan(%.2lf)\n", result);
            } else if (operation == 'l') {
                result = log10(result);
                printf("Operation: log10(%.2lf)\n", result);
            } else if (operation == 'r') {
                result = sqrt(result);
                printf("Operation: sqrt(%.2lf)\n", result);
            }
            
            
            printf("= %.2lf\n", result);
            continue; 
        }

        
        
        // STEP 3: Get the second number
        printf("Enter second number: ");
        if (scanf("%lf", &current_number) != 1) {
            printf("Error: Invalid number input.\n");
            
            while (getchar() != '\n');
            continue; // Restart loop
        }

        
        
        if (operation == '+') {
            result = result + current_number;
        } else if (operation == '-') {
            result = result - current_number;
        } else if (operation == '*') {
            result = result * current_number;
        } else if (operation == '/') {
            if (current_number == 0) {
                printf("Error: Division by zero is not allowed.\n");
            } else {
                result = result / current_number;
            }
        } else if (operation == '^') {
            result = pow(result, current_number); 
        } else {
           
            printf("Error: Invalid operation chosen or operation requires only one number.\n");
        }

        
        printf("= %.2lf\n", result);
    }

    printf("\nCalculator shutdown Final Result: %.2lf\n", result);
    printf("                     thank you !\n");
    printf("powered by: Ahmed Sidi Mohamed\n");
    printf("Sohaib Abdlmawgoyd \n");
    printf("Jana El Sherbiny\n");
    printf("Nour Amr\n");
    
    return 0;
}
