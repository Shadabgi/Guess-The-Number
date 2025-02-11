# Guess-The-Number
import random

Target = random.randint(1,100)

while True :
    userchoice = (input("Guess The Target or Quit(Q) :"))
    if(userchoice == "Q"):
        break
    userchoice = int(userchoice)
    if(userchoice == Target):
        print("Success : Correct Guess!!!")
        break
    elif(userchoice < Target):
        print("Your Number is Too Small.Take a Bigger Guess...")
    else:
        print("Your Number is Too Big.Take a Smaller Guess...")

print("___GAME OVER___")
