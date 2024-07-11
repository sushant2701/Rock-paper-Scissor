# Rock-paper-Scissor using python
import random
user_ch=int(input("Enteryour choice: Type 0 for Rocks, 1 for Paper, 2 for Scissors."))
if user_ch >=3 or user_ch <0:
    print("You entered invaild number , you lose.")
else:
    computer_ch=random.randint(0,2)
    print("Computer Choice")
    print(computer_ch)
    if computer_ch == user_ch:
        print("It's a draw.")
    elif computer_ch == 0 and user_ch == 2:
        print("Computer Wins.")
    elif user_ch == 0 and computer_ch == 2:
        print("You Win.")
    elif computer_ch > user_ch:
        print("Computer Wins.")
    elif user_ch > computer_ch:
        print("You Win.")
