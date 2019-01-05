# rockPaperScissors
# Ask user to type 'rock' 'paper' or 'scissors', then generate a random number 1-3 which will determine what the computer chose

import random

import random

def main():

    again = 'y'

    while again =='y' or again == 'Y':
        
     player = input('Player enters Rock, Paper or Scissors: ')
     print('The player entered   ', (player))

     computer = ['Rock' , 'Paper' , 'Scissors']
     print('The computer picked   ', random.choice(computer))

     number = random.randint(1, 4)
     print('The random number is', number)
    
    if player == 'Rock' and computer == 'Rock':
     print('The winner is Tie')
    elif player == 'Rock' and computer == 'Paper':
     print('The winner is COMPUTER')
     print(' Paper covers Rock')

    

    again = input('Would you like to play again? (y = yes): ')

main()
