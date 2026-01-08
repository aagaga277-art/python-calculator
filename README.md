# python-calculator
Simple Python calculator supporting multiple operations
x1 = float(input("Enter number 1: "))
x2 = float(input("Enter number 2: "))
x3 = float(input("Enter number 3: "))
x4 = float(input("Enter number 4: "))

op = input("Enter operator (+, -, *, /, **): ")

if op == "+":
    result = x1 + x2 + x3 + x4

elif op == "-":
    result = x1 - x2 - x3 - x4

elif op == "*":
    result = x1 * x2 * x3 * x4

elif op == "/":
    if x2 == 0 or x3 == 0 or x4 == 0:
        print("Error: Division by zero")
        exit()
    result = x1 / x2 / x3 / x4

elif op == "**":
    result = x1 ** x2 ** x3 ** x4

else:
    print("Invalid choice")
    exit()

print("The result is:", result)
