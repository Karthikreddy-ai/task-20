import random
def check_voting_eligibility():
    age = int(input("Enter your age: "))
    if age >= 18:
        print("You are eligible to vote.")
    else:
        print("You are not eligible to vote.")
def grade_to_letter(percentage):
    if 90 <= percentage <= 100:
        return "A"
    elif 80 <= percentage < 90:
        return "B"
    elif 70 <= percentage < 80:
        return "C"
    elif 60 <= percentage < 70:
        return "D"
    elif 0 <= percentage < 60:
        return "F"
    else:
        return "Invalid percentage"
def simple_calculator():
    print("\n--- Simple Calculator ---")
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    operation = input("Choose operation (+, -, *, /): ")

    if operation == "+":
        print("Result:", num1 + num2)
    elif operation == "-":
        print("Result:", num1 - num2)
    elif operation == "*":
        print("Result:", num1 * num2)
    elif operation == "/":
        if num2 != 0:
            print("Result:", num1 / num2)
        else:
            print("Error: Division by zero!")
    else:
        print("Invalid operation.")
def odd_even_guess():
    number = random.randint(1, 100)
    print(f"\nGenerated number: {number}")
    if number % 2 == 0:
        print("The number is even.")
    else:
        print("The number is odd.")
print("\n--- Testing Conditional Statements ---")
print("Grade 95%:", grade_to_letter(95))
print("Grade 82%:", grade_to_letter(82))
print("Grade 73%:", grade_to_letter(73))
print("Grade 65%:", grade_to_letter(65))
print("Grade 50%:", grade_to_letter(50))
print("Grade -5%:", grade_to_letter(-5))  
odd_even_guess()
