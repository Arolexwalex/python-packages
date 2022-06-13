# python-packages

import random 

user_action = input ("Enter a choice (rock, paper, scissors): ")
possible_actions = ["rock", "paper", "scissors"]
computer_action = random.choice(possible_actions)
print(f"\nYou chose {user_action}, computer chose {computer_action}. \n")
if user_action == computer_action: 
    print(f"Both players selected {user_action} It's a tie!")
elif user_action == "rock":
    if computer_action == "scissors":
        print("rock smashes scissors! You win!")
    else:
        print("paper covers rock! You lose.")
elif user_action == "paper":
    if computer_action == "rock":
        print("paper covers rock! You win! You win!")
    else:
        print("scissors cuts paper! You lose!")
elif user_action == "scissors":
    if computer_action == "paper":
        print("scissors cut paper! You win!")
    else:
        print("rock smashes scissors! You lose!")
