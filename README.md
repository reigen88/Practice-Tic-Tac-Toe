# Tic Tac Toe C++
Tic Tac Toe C++
This project implements a simple game "Tic Tac Toe" in C++ for two players. One player puts a cross, and the other puts a zero. The winner is the player who first finds a line (horizontally, parallel, diagonally) of crosses or zeros. There is a draw in the game, if all the cells of the field are occupied, and none of the players has collected a line, then there is a draw.
## Futures 
- Board Display: Shows the current state of the board.
- Player Moves: Player makes his move
- Win/Loss Checks Determines whether a player has won or lost
- Score Tracking: Reads and writes win/loss statistics from/to a file.
- Save Logs Saves all actions that have been performed in the game


The provided code snippet is part of a Tic-Tac-Toe game written in C++. It consists of two main functions: drawBoard and isMoveValid.

drawBoard() Function:

This function prints the current state of the Tic-Tac-Toe board to the console.
It uses nested loops to iterate over the 3x3 board array and prints each cell's value, separated by vertical bars (|).
After printing each row, it adds a horizontal line of dashes (-----------) for visual separation.
This function helps players see the board's current configuration.
isMoveValid(int choice) Function:

This function checks whether a player's move is valid.
It first ensures that the move is within the valid range (1 to 9). If not, it prints an error message and returns false.
If the move is valid, it converts the choice (which is a number from 1 to 9) into row and column indices for the board array.
Specifically, it calculates the row as (choice - 1) / 3 and the column as (choice - 1) % 3.
This function ensures that players can only choose valid positions on the board.
![image](https://github.com/reigen88/Practice-Tic-Tac-Toe/assets/161708406/2a698858-b64e-4a7b-b54d-1c65c4e5474d)




This part of the Tic-Tac-Toe game code handles checking for a win and the main game loop. Here’s a detailed explanation:

![image](https://github.com/reigen88/Practice-Tic-Tac-Toe/assets/161708406/c6905143-01bb-4f74-a5d0-ecc4cb05be1a)

These lines are part of a function that checks if a player has won the game.
It specifically checks for two diagonal win conditions:
From top-left to bottom-right (board[0][0], board[1][1], board[2][2]).
From top-right to bottom-left (board[0][2], board[1][1], board[2][0]).
If either condition is met, it returns true; otherwise, it returns false.
Initializes an empty 3x3 Tic-Tac-Toe board with spaces.
Sets the initial player to 'X'.
Initializes variables for row and column inputs and the turn counter.
Prints a welcome message.
Runs a loop for 9 turns (the maximum number of moves in Tic-Tac-Toe).
Calls drawBoard(board) to display the current state of the board.
Uses a while (true) loop to get valid input from the current player.
Prompts the player to enter a row and column.
Checks if the chosen cell is valid (empty and within bounds).
If the move is invalid, it prints an error message and prompts again.
If valid, breaks out of the loop.
Additional code for placing the move on the board and checking for a win would follow this input validation.



