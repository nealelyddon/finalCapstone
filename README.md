Financial Calculator
Introduction
The financial calculator is a Python program that allows users to calculate either the amount of interest they'll earn on an investment or the amount they'll have to pay on a home loan (bond). It provides a user-friendly interface and guides the user through the necessary inputs to perform the calculations.

Key Concepts
The key concepts in this financial calculator include:

Investment: Calculating the amount of interest earned on an investment based on the deposit amount, interest rate, number of years, and the type of interest (simple or compound).
Bond: Calculating the monthly repayment amount for a home loan based on the present value of the house, annual interest rate, and the number of months to repay.
Code Structure
The code is structured as follows:

Import the math module to use mathematical functions.
Display a welcome message and menu options for the user to choose between investment and bond calculations.
Prompt the user to enter their choice and convert it to lowercase for case-insensitive comparison.
Based on the user's choice, perform the corresponding calculations.
If the user chooses investment, prompt for the deposit amount, interest rate, number of years, and type of interest (simple or compound).
Calculate the investment amount based on the user's inputs and print the result.
If the user chooses bond, prompt for the present value of the house, annual interest rate, and number of months to repay.
Calculate the monthly bond repayment amount based on the user's inputs and print the result.
If the user enters an incorrect choice, display an error message.
Code Examples
Here are some code examples to illustrate the functionality of the financial calculator:

Calculating investment with simple interest:

deposit = float(input("Please enter the amount of money that you are depositing: "))
rate = float(input("Please enter the interest rate as a percentage: "))
n = float(input("Please enter the number of years you plan to invest: "))
interest = input("Please enter if you want simple or compound interest - type simple/compound: ").lower()

if interest == "simple":
    answer = round((deposit * (1 + rate/100 * n)), 2)
    print(f"\nYour investment will be worth R{answer} after {n} years.")

Calculating investment with compound interest:
language-python

deposit = float(input("Please enter the amount of money that you are depositing: "))
rate = float(input("Please enter the interest rate as a percentage: "))
n = float(input("Please enter the number of years you plan to invest: "))
interest = input("Please enter if you want simple or compound interest - type simple/compound: ").lower()

if interest == "compound":
    answer = round((deposit * math.pow((1 + rate/100), n)), 2)
    print(f"\nYour investment will be worth R{answer} after {n} years.")
Calculating bond repayment:
language-python
 
present_value = float(input("Please enter the present value of the house: "))
rate = float(input("Please enter the annual interest rate as a percentage: "))
n = float(input("Please enter the number of months you plan to repay: "))

answer = round(((rate / 12 / 100 * present_value) / (1 - math.powrate / 12 / 100), -n))), 2)
print(f"\nYour monthly bond repayment will be R{answer}.")

Conclusion
The financial calculator is a useful tool for individuals who want to calculate the interest earned on an investment or the monthly repayment amount for a home loan. It provides a simple and intuitive interface for users to input the necessary variables and obtain accurate results. By using this calculator, users can make informed financial decisions and plan their investments or loan repayments effectively.



    
