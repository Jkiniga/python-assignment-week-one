# python-assignment-week-one
assignment
def main():
    # 1. Read inputs
    try:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
    except ValueError:
        print("Error: please enter valid numbers.")
        return

    op = input("Enter operation (+, -, *, /): ")

    # 2. Compute based on the chosen operation
    if op == "+":
        result = num1 + num2
    elif op == "-":
        result = num1 - num2
    elif op == "*":
        result = num1 * num2
    elif op == "/":
        if num2 == 0:
            print("Error: cannot divide by zero.")
            return
        result = num1 / num2
    else:
        print("Invalid operation. Please choose +, -, *, or /.")
        return

    # 3. Display the result
    print(f"{num1} {op} {num2} = {result}")

if __name__ == "__main__":
    main()
