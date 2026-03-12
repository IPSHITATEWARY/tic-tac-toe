#🎮 Tic-Tac-Toe Console Game (Java)

A simple two-player Tic-Tac-Toe game built using Core Java.
The game runs in the console and demonstrates the use of arrays, loops, condition checking, and user input handling.

📌 Project Overview

This project implements the classic Tic-Tac-Toe game where two players take turns marking spaces on a 3×3 grid.
The game logic is built using a 2D char array, and methods are used to manage the board, validate input, and determine the winner.

The objective is simple:
Get three marks in a row (horizontal, vertical, or diagonal) before your opponent.

🛠 Tech Stack
Technology	Purpose
Java (Core)	Main programming language
Scanner (java.util)	Taking user input
2D Array (char[][])	Representing the game board
Console Output	Displaying the board and game messages
🧠 Data Structure Used
char[][] board = new char[3][3];

The 3×3 character array stores the current state of the game board.

Example board:

X | O | X
---------
O | X |  
---------
  | O | X
🔄 Game Flow

The program follows a turn-based loop:

Initialize Board

Create a 3×3 board and fill it with empty spaces.

Display Board

Print the board layout in the console.

Player Turn

Current player (X or O) enters row and column.

Input Validation

Check if the move is within bounds and the cell is empty.

Update Board

Place the player’s marker in the selected cell.

Check Game Status

Check for win or draw.

Switch Player

If the game is not over, the next player takes a turn.

🧩 Key Components
1️⃣ Game Engine

Controls the main game loop and manages player turns.

Example:

char currentPlayer = 'X';

Handles:

Player switching

Input handling

Game termination

2️⃣ Board Display Method

Responsible for printing the board neatly.

Example method:

printBoard(char[][] board)

Concept:

Iterate through the 2D array

Print characters with separators like | and -

Example output:

X | O | X
---------
O | X | O
---------
  |   | X
3️⃣ Win Checker (Core Logic)

Determines if a player has won the game.

Method example:

checkWin(char[][] board, char marker)

The method checks 8 winning conditions:

Rows
board[i][0] == board[i][1] == board[i][2]
Columns
board[0][j] == board[1][j] == board[2][j]
Diagonals
board[0][0] → board[1][1] → board[2][2]
board[0][2] → board[1][1] → board[2][0]

▶️ How to Run

Clone the repository

git clone https://github.com/IPSHITATEWARY/tic-tac-toe.git

Navigate to the project folder

cd tic-tac-toe

Compile the Java file

javac TicTacToe.java

Run the program

java TicTacToe
🎯 Learning Outcomes

This project demonstrates:

2D Array Manipulation

User Input Handling

Game Logic Implementation

Control Flow & Loops

Basic Object-Oriented Programming Concepts

📌 Future Improvements

Possible upgrades:

Add single player mode (AI opponent)

Implement a GUI version using Java Swing

Add score tracking

Improve input validation

👩‍💻 Author

Ipshita Tewary

GitHub:
👉 https://github.com/IPSHITATEWARY
