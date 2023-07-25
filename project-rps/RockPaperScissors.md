# Software Requirements Specification (SRS) Document for Rock, Paper, Scissors 

## 1. Introduction

Rock Paper Scissors is a game of chance. In this game two players signify rock, paper, or scissors with their hands at
the same time and then reveal them. The winner of the game is determined by the following rules:

- Paper beats rock,
- Rock beats scissors and
- Scissors beat paper.

## 2. Project Scope

This project is a prototype (How will my product look like and work?) for an eventual GUI based RPS game. The scope 
includes the creation of a simple two-player `command-line` Rock, Paper, Scissors game, where the user plays against the 
computer. This game should be coded in Java.

## 3. Functional Requirements

### 3.1 User Interface

1. The game must have a user-friendly text-based interface through the command line.
2. The game must prompt the user to enter their move (i.e., Rock, Paper, Scissors).
3. The game must display the individual moves of the user and the computer.
4. The game must show the result of each round and the current score.
5. The game must display a summary of the total wins, losses, and ties before exiting.
6. The game must allow the user to quit at any time by entering a specific quit command (e.g., "Q" or "quit").
7. The game must save the game statistics to a file before exiting.
    - The file must be in a comma-separated value (CSV) format.
    - The file must contain the following information:
        - The number of wins, losses, and ties for the user.
        - The number of wins, losses, and ties for the computer.
        - The total number of rounds played.
8. The game must display the game statistics from the file when the game is started.

### 3.2 Game Logic

1. The game must randomly select a move for the computer player.
2. The game must determine the winner of each round according to the following rules:
   - If the player selects Paper and Computer Selects Scissor – Computer wins
   - If the player selects Rock and Computer Selects Scissor – Player 1 wins
   - If the player selects Paper and Computer Selects Rock – Player 1 wins
   - And If the player selects Paper and Computer Selects Paper – Draw
   - If the player selects Rock and Computer Selects Rock – Draw
   - If the player selects Scissor and Computer Selects Scissor – Draw
3. High-level flow
![High-level flow](./images/high-level-flow.png)

## 4. Non-Functional Requirements

- The game must be written in Java.
- The game must be able to run on a command line interface.
- The game must be able to handle invalid input from the user.