# Temperature-converter
#include <stdio.h>

void celsiusToFahrenheit(float celsius) {
    printf("%.2f Celsius = %.2f Fahrenheit\n", celsius, (celsius * 9/5) + 32);
}

void fahrenheitToCelsius(float fahrenheit) {
    printf("%.2f Fahrenheit = %.2f Celsius\n", fahrenheit, (fahrenheit - 32) * 5/9);
}

void celsiusToKelvin(float celsius) {
    printf("%.2f Celsius = %.2f Kelvin\n", celsius, celsius + 273.15);
}

void kelvinToCelsius(float kelvin) {
    printf("%.2f Kelvin = %.2f Celsius\n", kelvin, kelvin - 273.15);
}

void fahrenheitToKelvin(float fahrenheit) {
    printf("%.2f Fahrenheit = %.2f Kelvin\n", fahrenheit, (fahrenheit - 32) * 5/9 + 273.15);
}

void kelvinToFahrenheit(float kelvin) {
    printf("%.2f Kelvin = %.2f Fahrenheit\n", kelvin, (kelvin - 273.15) * 9/5 + 32);
}

int main() {
    int choice;
    float temp;

    printf("Temperature Converter\n");
    printf("1. Celsius to Fahrenheit\n");
    printf("2. Fahrenheit to Celsius\n");
    printf("3. Celsius to Kelvin\n");
    printf("4. Kelvin to Celsius\n");
    printf("5. Fahrenheit to Kelvin\n");
    printf("6. Kelvin to Fahrenheit\n");
    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            printf("Enter temperature in Celsius: ");
            scanf("%f", &temp);
            celsiusToFahrenheit(temp);
            break;
        case 2:
            printf("Enter temperature in Fahrenheit: ");
            scanf("%f", &temp);
            fahrenheitToCelsius(temp);
            break;
        case 3:
            printf("Enter temperature in Celsius: ");
            scanf("%f", &temp);
            celsiusToKelvin(temp);
            break;
        case 4:
            printf("Enter temperature in Kelvin: ");
            scanf("%f", &temp);
            kelvinToCelsius(temp);
            break;
        case 5:
            printf("Enter temperature in Fahrenheit: ");
            scanf("%f", &temp);
            fahrenheitToKelvin(temp);
            break;
        case 6:
            printf("Enter temperature in Kelvin: ");
            scanf("%f", &temp);
            kelvinToFahrenheit(temp);
            break;
        default:
            printf("Invalid choice! Please select a valid option.\n");
    }

    return 0;
}




  ![image](https://github.com/user-attachments/assets/ba1fc7ef-d168-4c3d-841f-c53c8286b05b)
