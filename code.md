# September 23, 2025 - First real coding proiblem i solved in python

x = float(input("Enter value for x: "))
print("y =",str( 1 / (x+1 /(x+1/ (x+1))) / x))


# September 30 - Evaluate the end time of a period of time, given as a number of minutes. The start time is given as a pair of hours (0..23) and minutes (0..59).

hour = int(input("Starting time (hours): "))

mins = int(input("Starting time (minutes): "))

dura = int(input("Event duration (minutes): "))

TMS = hour * 60 + mins 

TME = TMS + dura

end_hour = (TME//60) % 24

end_minutes = TME % 60

print(end_hour, end_minutes, sep=":")


# November 5, 2025 - Tax Calculator

income = float(input("Enter the annual income: "))

if income <= 85528:
    tax = 0.18 * income - 556.02
    
else:
    tax = 14839.02 + 0.32 * (income - 85528)

if tax < 0:
    tax = 0

tax = round(tax, 0)



print("The tax is:", tax, "thalers")


# November 12, 2025 - leap year calc, number guessing game

year = int(input("Enter a year: "))

if (year < 1582):
    print("Not within the Gregorian calendar period")
    
elif (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("Leap year")
    
else: print("Common year")


secret_number = 777 # It can be changed to whatever number

print(
"""
+================================+
| Welcome to my game, muggle!    |
| Enter an integer number        |
| and guess what number I've     |
| picked for you.                |
| So, what is the secret number? |
+================================+
""")

guess = 0

while guess != secret_number:

    guess = int(input())
    
    print("Ha ha! You're stuck in my loop!")
    
print("Well done, muggle! You are free now.")
