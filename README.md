def calculator():
 num1 = float(input("Enter the first number: ")) 
 num2 = float(input("Enter the second number: ")) 
 operation = input("Enter operation (+, -, *, /): ")

if operation == '+':
        result = num1 + num2
     elif operation == '-':
        result = num1 - num2
    elif operation == '*':
        result = num1 * num2
    elif operation == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
            return
        result = num1 / num2
    else:
        print("Invalid operation. Please enter one of +, -, *, /")
        return
    
    print(f"The result is: {result}")
except ValueError:
    print("Invalid input. Please enter numeric values.")

calculator()
