# A-simple-dice-game-

## Overview
This program simulates a simple dice game for 2 to 4 players. Each player takes turns rolling a six-sided die, aiming to be the first to reach a total score of 50 points. Players can keep rolling during their turn to accumulate points but risk losing all points for that turn if they roll a 1.

## How to Run the Game
1. Ensure you have Python installed on your machine.
2. Save the code in a file, for example, `dice_game.py`.
3. Run the script using a Python interpreter:
   ```
   python dice_game.py
   ```

## Gameplay Instructions
1. **Start the Game**:
   - The game will prompt you to enter the number of players (between 2 and 4).

2. **Player Turns**:
   - Players take turns to roll a die.
   - At the start of each player's turn, their current total score is displayed.
   - The player can choose to roll the die by entering 'y'. Any other input will end their turn.
   - If the player rolls a 1, their turn ends immediately, and they score no points for that turn.
   - If the player rolls a 2-6, the rolled value is added to their current score for that turn.
   - The player can continue to roll as many times as they want during their turn to accumulate points, but the risk is that rolling a 1 will nullify all points accumulated during that turn.

3. **End of Turn**:
   - At the end of the turn, the player's score for that turn is added to their total score.
   - The game then proceeds to the next player.

4. **Winning the Game**:
   - The game continues until one player reaches or exceeds a total score of 50 points.
   - The player with the highest score at the end of the game is declared the winner.

## Code Explanation
- `roll()`: Function to simulate rolling a six-sided die, returning a random integer between 1 and 6.
- The main loop prompts for the number of players and validates the input.
- `player_scores`: A list to keep track of each player's total score.
- The game loop runs until one player's score reaches or exceeds 50 points.
- Within the game loop, each player takes their turn, rolling the die and accumulating points.
- The winner is determined and announced when the game ends.

## Example Output
```
Enter the number of players (2 - 4): 3

Player number 1 turn has just started!
Your total score is: 0 

Would you like to roll (y)? y
You rolled a: 5
Your score is: 5
Would you like to roll (y)? y
You rolled a: 3
Your score is: 8
Would you like to roll (y)? n
Your total score is: 8

Player number 2 turn has just started!
Your total score is: 0 
...
Player number 1 is the winner with a score of: 50
```

## Dependencies
- Python 3.x
- `random` module (standard library)

Enjoy the game and good luck!
