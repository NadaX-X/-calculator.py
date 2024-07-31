# Calculator

This is a simple calculator program written in Python that can perform various arithmetic operations such as addition, 
subtraction, multiplication, division, square, power, and square root.

## Features
- Supports the following operations:
  - Addition
  - Subtraction
  - Multiplication
  - Division
  - Square
  - Power
  - Square Root
- Handles invalid inputs, such as non-numeric values or division by zero, and provides appropriate error messages.
- Allows the user to perform multiple operations in a single session and exit the program when desired.

## Usage

1. Run the calculator.py file in your Python environment.
2. The program will display a menu of available operations.
3. Enter the corresponding number for the operation you want to perform.
4. Follow the prompts to enter the necessary number(s) for the selected operation.
5. The program will display the result of the calculation.
6. You can continue performing calculations or select the "Exit" option to terminate the program.

## Code Structure

The program consists of the following functions:

- add(a, b): Performs addition of two numbers.
- sub(a, b): Performs subtraction of two numbers.
- mult(a, b): Performs multiplication of two numbers.
- div(a, b): Performs division of two numbers, handling the case of division by zero.
- sqr(a): Calculates the square of a number.
- pwr(a, b): Calculates the power of a number.
- sqrroot(a): Calculates the square root of a number.
- main(): Implements the main program loop, displaying the menu, handling user input, and calling the appropriate functions.

The main() function is the entry point of the program, where the user can interact with the calculator.

## Installation and Dependencies

This program does not require any external dependencies. It can be executed using a standard Python environment.

## Contribution

If you find any issues or have suggestions for improvements, feel free to create a new issue or submit a pull request on the [GitHub repository](https://github.com/your-username/calculator).

## License

This project is licensed under the [MIT License](LICENSE).
