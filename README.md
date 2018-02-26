# QA

import random

attempts = 0

name = input("What is your name? ")
random = random.randint(1, 20)
print(name + ",","I'm thinking of a number between 1 and 20, What is it?")

while attempts < 6:
    number = int(input("Type your guess: "))
    attempts = attempts + 1
    int(print(attempts,"attemps left")) #This is the code to tell the user how many attempts left
    if number < random:
        print("Too low. Try something higher")
    if number > random:
        print("Too high. Try something lower")
    if number == random:
        break
if number == random:
    if attempts <= 3:
        print("Well done,",name + "! It took you only",attempts,"attempts")
    if attempts >= 4:
        print("Well done,",name + "! It took you",attempts,"attempts. Athough, next time try to get three attempts or lower")
if number != random:
    print("Sorry. All your attempts have been used up. The number I was thinking of was",random)
