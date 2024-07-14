# Snake-Game
A simple snake terminal game in  cpp
![image](https://github.com/user-attachments/assets/34b4d29c-f230-48d1-8946-0613851fb33a)

# Snake Game

A simple Snake game implemented in C++ for the terminal. This project is designed to run on Windows using the `conio.h` library for handling input and `windows.h` for sleep functionality.

## Features

- Classic snake gameplay
- Simple controls: W, A, S, D for movement, X to quit
- Randomly placed fruit to eat and grow the snake
- Score tracking

## Requirements

- gcc compiler (MinGW recommended for Windows)

## Getting Started

### Prerequisites

Ensure you have MinGW installed on your system. If not, you can download and install it from [MinGW](http://www.mingw.org/).

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/snake_game.git
   cd snake_game
Compile the code using g++:

sh
Copy code
g++ -o snake_game snake_game.cpp -std=c++11
Run the game:

sh
Copy code
./snake_game
Controls
W: Move up
A: Move left
S: Move down
D: Move right
X: Quit game
Code Overview
The main components of the game include:

Setup(): Initializes the game state.
Draw(): Renders the game state to the terminal.
Input(): Handles user input.
Logic(): Contains the game logic, including movement and collision detection.
EndGame(): Displays the final score and waits for user input before exiting.
Setup
Initializes the game variables and sets the initial position of the snake and fruit.

Draw
Clears the screen and redraws the game board, including the snake and the fruit. Displays the current score.

Input
Reads user input without blocking the game loop, allowing real-time control of the snake.

Logic
Updates the game state based on the current direction of the snake. Handles movement, collision detection, and fruit consumption.

EndGame
Displays the "Game Over" message and final score, and waits for the user to press a key before exiting the game.

