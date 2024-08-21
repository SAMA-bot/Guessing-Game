# Guess the Number Game

This is a simple Python game where the user tries to guess a randomly generated number between 0 and 100. The game provides the following features:

1. **Random Number Generation**: The game generates a random number between 0 and 100 for the user to guess.

2. **User Guessing**: The user is prompted to enter a guess. If the input is not a valid integer, an error message is displayed, and the user is asked to try again.

3. **Feedback on Guesses**: After each guess, the game provides feedback to the user, indicating whether the guess is higher or lower than the target number.

4. **Attempt Limit**: The game allows a maximum of 7 attempts to guess the number correctly. If the user exceeds this limit, the game ends, and the correct number is revealed.

5. **Restart Option**: After the game ends, the user is asked if they want to play again. If the user chooses "yes", the game restarts.

6. **Clear Output**: The `clear_output()` function from the `IPython.display` module is used to clear the output after each guess, providing a clean and organized game experience.

To play the game, simply run the provided code. The game will start, and the user can begin guessing the number.

Here's a step-by-step breakdown of how the game works:

1. The game starts by importing the necessary modules: `randint` from the `random` module and `clear_output` from the `IPython.display` module.
2. The `MAX_ATTEMPTS` constant is set to 7, representing the maximum number of guesses allowed.
3. The `play_game()` function is defined, which contains the main game logic.
4. Inside the `play_game()` function:
   - A random number is generated using `randint(0, 100)` and stored in the `number` variable.
   - A `guessed` flag is initialized to `False`, and a `guesses` counter is set to 0.
   - A `while` loop is used to handle the guessing process. The loop continues until the user guesses correctly or the maximum number of attempts is reached.
   - Inside the loop:
     - The user is prompted to enter a guess using `int(input())`. If the input is not a valid integer, an error message is displayed, and the loop continues.
     - The `guesses` counter is incremented, and the output is cleared using `clear_output()`.
     - The user's guess is compared to the target number. If the guess is correct, a success message is displayed, and the `guessed` flag is set to `True`. If the guess is higher or lower, appropriate feedback is provided.
   - If the user runs out of attempts without guessing correctly, the correct number is revealed.
5. After the game ends, the user is asked if they want to play again. If the user chooses "yes", the `play_game()` function is called again to restart the game.
