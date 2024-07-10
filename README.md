# -calculator.py
A simple calculator application implemented in Python, featuring basic arithmetic operations (add, subtract, multiply, divide), as well as square, power, and square root functions.
def add(a, b):
    return a + b

def sub(a, b):
    return a - b

def mult(a, b):
    return a * b

def div(a, b):
    if b == 0:
        return "Invalid value for denominator, can't divide by 0!"
    else:
        return a / b

def sqr(a):
    return a ** 2

def pwr(a, b):
    return a ** b

def sqrroot(a):
    return a ** 0.5

def main():
    while True:
        print("Welcome to the Calculator!")
        print("Please select an operation:")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Square")
        print("6. Power")
        print("7. Square Root")
        print("8. Exit")

        try:
            choice = input("Enter your choice (1-8): ")

            if choice == "8":
                print("Exiting the Calculator...")
                break

            num1 = float(input("Enter the first number: "))
            num2 = float(input("Enter the second number: "))

            if choice == "1":
                result = add(num1, num2)
                print(f"Result: {result}")
            elif choice == "2":
                result = sub(num1, num2)
                print(f"Result: {result}")
            elif choice == "3":
                result = mult(num1, num2)
                print(f"Result: {result}")
            elif choice == "4":
                result = div(num1, num2)
                print(f"Result: {result}")
            elif choice == "5":
                result = sqr(num1)
                print(f"Result: {result}")
            elif choice == "6":
                result = pwr(num1, num2)
                print(f"Result: {result}")
            elif choice == "7":
                result = sqrroot(num1)
                print(f"Result: {result}")
            else:
                print("Invalid choice. Please try again.")

        except ValueError:
            print("Invalid input. Please enter a valid number.")
        except EOFError:
            print("Unexpected end of input. Exiting the calculator.")
            break
        except ZeroDivisionError:
            print("Error: Division by zero is not allowed.")

        print()

if __name__ == "__main__":
    main()
