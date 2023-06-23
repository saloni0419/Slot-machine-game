# Slot-machine-game


This is a JavaScript code implementation of a simple slot machine game. The game allows users to deposit money, place bets on a certain number of lines, spin the slot machine, check for winning combinations, and collect their winnings. The game provides an option to play again until the user decides to stop.

## How to Play

1. Deposit Money: The game starts by asking the user to enter a deposit amount. The user must provide a valid positive numeric value.

2. Number of Lines: Next, the user is prompted to enter the number of lines to bet on. The valid range is from 1 to 3.

3. Place Bet: The user is then asked to enter a bet amount per line. The bet amount must be a valid positive numeric value and cannot exceed the available balance divided by the number of lines.

4. Spin the Slot Machine: The slot machine is spun, and the symbols on the reels are randomly generated. The reels consist of 3 rows and 3 columns.

5. Check for Winning: The game checks each line for winning combinations. If all symbols on a line are the same, the user wins and receives a payout based on the symbol's value and the bet amount.

6. Collect Winnings: The user's balance is updated with the winnings. If there are no winnings, the balance remains the same.

7. Play Again: After each round, the user is given an option to play again. If the user chooses to play again, the game restarts from step 2. If the user declines, the game ends.

## Game Logic

The game logic is implemented using functions and constants:

- `deposit()`: Prompts the user to enter a deposit amount and returns the valid numeric value.

- `getNumberOfLines()`: Prompts the user to enter the number of lines to bet on and returns the valid numeric value within the range of 1 to 3.

- `getBet(balance, lines)`: Prompts the user to enter a bet amount per line and returns the valid numeric value. The bet amount cannot exceed the available balance divided by the number of lines.

- `spin()`: Generates random symbols for the reels by selecting symbols from the predefined symbol pool.

- `transpose(reels)`: Transposes the reels matrix to represent the rows instead of columns, making it easier to check for winning combinations.

- `printRows(rows)`: Prints the symbols on each row of the slot machine.

- `getWinnings(rows, bet, lines)`: Checks each line for winning combinations and calculates the winnings based on the bet amount and symbol values.

- `game()`: Main game function that orchestrates the gameplay. It starts by accepting the user's deposit, and then it continues the game loop until the user chooses to stop or runs out of money.

## Running the Game

To run the game, you need to have Node.js installed on your machine. Copy the provided code into a JavaScript file (e.g., `slot-machine.js`), and then execute the file using Node.js:

```shell
node slot-machine.js
```

Follow the on-screen prompts to play the game. Make sure to enter valid inputs as specified for each step.

Please note that the game doesn't have any graphical user interface (GUI) and is played through the console/terminal.

Enjoy playing the slot machine game!
