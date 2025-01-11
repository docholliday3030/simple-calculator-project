# simple-calculator-project
# Calculator Project

#Function to perform subtraction
def subtract(x, y):
    return x - y

#Function to perform division
def divide(x, y):
    if y == 0:
        return "Cannot divide by zero"
    else:
        return x / y

#Function to perform addition
def add(x, y):
    return x + y

#Function to perform multiplication
def multiply(x, y):
    return x * y

#Get input from the user
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operand = input("Enter the operand (+, -, *, /): ")

#Preform calculation based on the operand
if operand == '+':
    result = add(num1, num2)
elif operand == '-':
    result = subtract(num1, num2)
elif operand == '*':
    result = multiply(num1, num2)
elif operand == '/':
    result = divide(num1, num2)
else:
    result = "Invalid operand"

# Print the result
print("Result:", result)
