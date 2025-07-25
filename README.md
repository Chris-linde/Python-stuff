# Python-stuff
#Revolver roulette
import random
Gun_list = [1, 2, 3, 4, 5, 6]
#numbers to be chosen.
Gun_choice = random.choice(Gun_list)
#choosing the numbers by random.
def game_loop():
    Choice = input('Choose a number, (1-6)')
    if int(Choice) == Gun_choice:
        #int( is to convert from a string to an integer.
        print('\nCorrect!')
    else:
        print(f'\nYou died, you chose: \n{Choice}, \nbut the right number was: \n{Gun_choice}')
        #this is an "f" string, you need an f string to display variables in your text.
game_loop()