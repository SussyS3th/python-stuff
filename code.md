# September 23, 2025
## Complex Expression

x = float(input("Enter value for x: "))
print("y =",str( 1 / (x+1 /(x+1/ (x+1))) / x))


# September 30
## End Time Calculator

hour = int(input("Starting time (hours): "))

mins = int(input("Starting time (minutes): "))

dura = int(input("Event duration (minutes): "))

TMS = hour * 60 + mins 

TME = TMS + dura

end_hour = (TME//60) % 24

end_minutes = TME % 60

print(end_hour, end_minutes, sep=":")


# November 5, 2025
## Tax Calculator

income = float(input("Enter the annual income: "))

if income <= 85528:
    tax = 0.18 * income - 556.02
    
else:
    tax = 14839.02 + 0.32 * (income - 85528)

if tax < 0:
    tax = 0

tax = round(tax, 0)



print("The tax is:", tax, "thalers")


# November 12, 2025
## Leap Year Checker

year = int(input("Enter a year: "))

if (year < 1582):
    print("Not within the Gregorian calendar period")
    
elif (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("Leap year")
    
else: print("Common year")


## Number Guess

secret_number = 777 # It can be changed to whatever number

print("Welcome to my game, muggle! Enter an integer number and guess what number I've picked for you. So, what is the secret number?")

guess = 0

while guess != secret_number:

    guess = int(input())
    
    print("Ha ha! You're stuck in my loop!")
    
print("Well done, muggle! You are free now.")

## Mississippi Counter

import time

for i in range(1,6):

    print(i,"Mississippi")
    
    time.sleep(1)
    
print("Ready or not, here I come")


# November 17, 2025
## Word Guesser
word = "chupacabra" # the word can be changed to match your preference

guess = ""

while (guess != word):

    guess = input("enter a word: ")
    
    if (guess == word):
    
        break

print("You've successfully left the loop.")

### example 2

while True:

    word = input("Enter a word: ")
    
    if word == "chupacabra": # the word can be changed to match your preference
    
        print("You've successfully left the loop.")
        
        break

