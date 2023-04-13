# Calculator Program in Python

# Addition
def add(a, b):
    return a + b

# Subtraction
def subtract(a, b):
    return a - b

# Multiplication
def multiply(a, b):
    return a * b

# Division
def divide(a, b):
    if b == 0:
        print("Error: Division by zero is not allowed!")
        return None
    else:
        return a / b

# Main Calculator Loop
while True:
    print("Select an operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Exit")

    choice = input("Enter your choice (1/2/3/4/5): ")

    if choice == '5':
        print("Exiting...")
        break

    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))

    if choice == '1':
        result = add(num1, num2)
        print("Result: ", result)
    elif choice == '2':
        result = subtract(num1, num2)
        print("Result: ", result)
    elif choice == '3':
        result = multiply(num1, num2)
        print("Result: ", result)
    elif choice == '4':
        result = divide(num1, num2)
        if result is not None:
            print("Result: ", result)
