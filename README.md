#include <iostream>
using namespace std;

int main() {
    char operation;
    double num1, num2;

    // Get input from the user
    cout << "Enter first number: ";
    cin >> num1;

    cout << "Enter an operation (+, -, *, /): ";
    cin >> operation;

    cout << "Enter second number: ";
    cin >> num2;

    // Perform calculation based on the selected operation
    switch (operation) {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0) {
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            } else {
                cout << "Error: Division by zero is undefined." << endl;
            }
            break;
        default:
            cout << "Invalid operation. Please enter +, -, *, or /." << endl;
            break;
    }

    return 0;
}
