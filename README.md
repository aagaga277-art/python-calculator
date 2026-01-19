# python-calculator
Simple Python calculator supporting multiple operations
x1 = float(input("Enter number 1: "))
x2 = float(input("Enter number 2: "))

op = input("Enter operator (+, -, *, /, **): ")

if op == "+":
    result = x1 + x2 

elif op == "-":
    result = x1 - x2

elif op == "*":
    result = x1 * x2

elif op == "/":
    if x2 == 0:
        print("Error: Division by zero")
        exit()
    result = x1 / x2
elif op == "**":
    result = x1 ** x2

else:
    print("Invalid choice")
    exit()

print("The result is:", result)


