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

### Word Guesser Simplified

while True:

    word = input("Enter a word: ")
    
    if word == "chupacabra": # the word can be changed to match your preference
    
        print("You've successfully left the loop.")
        
        break

## Ugly Vowel Muncher

user_word = input("Enter a word: ").upper()

vowels = "AEIOU"

print("Filtered Word:")

for letter in user_word:

    if letter not in vowels:
    
        print(letter, end='\n')
    

##  Pretty Vowel Muncher
word_without_vowels = ""

user_word = input("Enter a word: ")

user_word = user_word.upper()

for letter in user_word:

    # Complete the body of the for loop.
    
    if (letter in "AEIOU"):
    
        continue
        
    word_without_vowels += letter


print(word_without_vowels)

# December 2, 2025
## Pyramids

blocks = int(input("Enter the number of blocks: "))

height = 0;

blocksN = 1 # blocks needed for next layer


while blocks >= blocksN:

    blocks-= blocksN
    height += 1
    blocksN += 1

print("The height of the pyramid:", height)

##  Collatz theory

c0 = int(input("Enter a positive integer: "))

steps = 0

while c0 != 1:

    if c0 % 2 == 0:
        c0 = c0 // 2
        
        print(c0)
        
        steps += 1
        
    else:
    
        c0 = 3 * c0 + 1
        
        print(c0)
        
        steps += 1

print("steps = ",steps)

# December 3, 2025
## Beatles

beatles = []

print("Step 1:", beatles)


print("Step 2:", beatles)

beatles.append("John Lennon")

beatles.append("Paul McCartney")

beatles.append("George Harrison")


print("Step 3:", beatles)

members_to_add = ["Stu Sutcliffe", "Pete Best"]

for member in members_to_add:

    user_input = input(f"Add {member} to the band? (yes/no): ")
    
    if user_input.lower() == "yes":
    
        beatles.append(member)


print("Step 4:", beatles)

del beatles[-1]

del beatles[-1]



print("Step 5:", beatles)

beatles.insert(0, "Ringo Starr")

print("The Fab", len(beatles))


# December 16, 2025
## Dupe Remover

my_list = [1, 2, 4, 4, 1, 4, 2, 6, 2, 9]

unique_list = []

for number in my_list:

    if number not in unique_list:
    
        unique_list.append(number)

my_list = unique_list

print("The list with unique elements only:")

print(my_list)
