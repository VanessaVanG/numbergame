import random

computer_number =random.randint(1,9)
while True:
    try:
        human_number= int(input("Enter a number between 1 and 9 for the computer to guess. Don't worry. The computer won't know. "))
    except ValueError:
        print("Sorry. It has to be a number.")
    else: 
      if computer_number==human_number:
        print("""Is your number {}?
Hahaha! It is! Bow down to your computer overlords!""".format(computer_number))
        break
      else: 
        print(""" Is your number {}? 

No. That's not it. The computer will try again.""".format(computer_number))
