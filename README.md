The provided Python code is a simple number guessing game where the player attempts to guess a randomly generated target number between 1 and 100.<br>
import random as r: This line imports the 'random' module and aliases it as 'r', allowing the use of random number generation functions.<br>

target = r.randint(1, 100): Generates a random integer between 1 and 100 (inclusive) and assigns it to the variable 'target'. This is the number the player needs to guess.<br>

while True:: Initiates an infinite loop, as 'True' is always true, creating an indefinite game until the player chooses to quit.<br>

userchoice = input("Guess the target or Quit : "): Prompts the user to enter their guess or type 'Quit' to exit the game. The input is stored in the variable 'userchoice'.<br>

if(userchoice == "Quit"): break: Checks if the user wants to quit by comparing their input to the string "Quit". If true, the loop breaks, and the game ends.<br>

userchoice = int(userchoice): Converts the user's input (assumed to be a number) from a string to an integer, preparing it for comparison with the target number.<br>

if(userchoice == target): print("Success: Correct Guess!!"); break: Checks if the user's guess matches the target number. If true, it prints a success message, and the loop breaks, ending the game.<br>

elif(userchoice < target): print("Your number was too small. Take a bigger guess.."): Executes if the user's guess is smaller than the target. It provides feedback to the user, encouraging them to guess a larger number.<br>

else: print("Your number was too big. Take a smaller guess.."): Executes if the user's guess is larger than the target. It provides feedback to the user, encouraging them to guess a smaller number.<br>

print("-----GAME-OVER-----"): Outside the loop, this line is reached when the game is over, either due to a correct guess or the user choosing to quit. It prints a "GAME-OVER" message to indicate the end of the game.<br>
