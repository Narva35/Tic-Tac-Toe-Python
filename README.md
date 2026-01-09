# 🎮 Tic-Tac-Toe Python Game

A command-line implementation of the classic Tic-Tac-Toe game in Python, featuring player vs computer gameplay with intelligent AI moves.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Game Rules](#game-rules)
- [Technical Implementation](#technical-implementation)
- [Installation](#installation)
- [How to Play](#how-to-play)
- [Code Structure](#code-structure)
- [Functions Documentation](#functions-documentation)
- [Future Improvements](#future-improvements)

## 🎯 Overview

This project is a Python implementation of the traditional Tic-Tac-Toe game (also known as Noughts and Crosses). The game is played on a 3x3 grid where the player competes against a computer opponent. The player uses 'O' markers while the computer uses 'X' markers.

## ✨ Features

- **Interactive Console Interface**: Clean and intuitive command-line display
- **Player vs Computer**: Single-player mode against an AI opponent
- **Smart AI Moves**: Computer makes strategic decisions
- **Input Validation**: Prevents invalid moves and ensures game integrity
- **Win Detection**: Automatic detection of winning conditions
- **Draw Detection**: Identifies when the game ends in a tie

## 📖 Game Rules

1. The game is played on a 3x3 grid
2. Player uses 'O' and Computer uses 'X'
3. Players take turns placing their marks on empty squares
4. The first player to get 3 of their marks in a row (horizontally, vertically, or diagonally) wins
5. If all 9 squares are filled and no player has won, the game is a draw

## 🔧 Technical Implementation

### Board Representation

The game board is represented as a 3x3 list in Python:
```python
board = [[1, 2, 3],
         [4, 5, 6],
         [7, 8, 9]]
```

### Key Algorithms

- **Win Detection**: Checks all possible winning combinations (rows, columns, diagonals)
- **Move Validation**: Ensures moves are made only on available squares
- **AI Logic**: Computer selects moves from available positions

## 💻 Installation

### Prerequisites

- Python 3.x installed on your system

### Setup

1. Clone the repository:
```bash
git clone https://github.com/Narva35/Tic-Tac-Toe-Python.git
```

2. Navigate to the project directory:
```bash
cd Tic-Tac-Toe-Python
```

3. Run the game:
```bash
python "Projeto Final.py"
```

## 🎮 How to Play

1. Run the Python script
2. The game board will be displayed with numbers 1-9
3. Enter a number (1-9) to place your 'O' in that position
4. The computer will automatically make its move with 'X'
5. Continue until someone wins or the board is full
6. The game will announce the winner or declare a draw

### Example Gameplay

```
+-------+-------+-------+
|       |       |       |
|   1   |   2   |   3   |
|       |       |       |
+-------+-------+-------+
|       |       |       |
|   4   |   5   |   6   |
|       |       |       |
+-------+-------+-------+
|       |       |       |
|   7   |   8   |   9   |
|       |       |       |
+-------+-------+-------+

Enter your move: 5
```

## 📁 Code Structure

The project consists of a single Python file with the following main components:

### Core Functions

1. **`displayboard(board)`**: Renders the game board in the console
2. **`entermove(board)`**: Handles player input and validates moves
3. **`makelistoffreefields(board)`**: Generates a list of available positions
4. **`victoryfor(board, sign)`**: Checks if a player has won
5. **`drawmove(board)`**: Executes the computer's move

### Game Flow

```
Initialize Board → Display Board → Player Move → Check Win/Draw → 
Computer Move → Check Win/Draw → Repeat
```

## 📚 Functions Documentation

### `displayboard(board)`
**Purpose**: Displays the current state of the game board
- **Input**: 2D list representing the board
- **Output**: Formatted board display in console
- **Format**: Clean ASCII art representation with borders

### `entermove(board)`
**Purpose**: Processes player input and places 'O' on the board
- **Input**: Current board state
- **Validation**: Checks if the move is valid (1-9 and square is free)
- **Update**: Places 'O' on the selected square

### `makelistoffreefields(board)`
**Purpose**: Identifies all available positions on the board
- **Input**: Current board state
- **Output**: List of tuples containing coordinates of empty squares
- **Usage**: Used by AI to determine possible moves

### `victoryfor(board, sign)`
**Purpose**: Determines if a player has achieved a winning condition
- **Input**: Board state and player symbol ('O' or 'X')
- **Output**: Boolean indicating win status
- **Checks**: All rows, columns, and diagonals for three-in-a-row

### `drawmove(board)`
**Purpose**: Executes the computer's move
- **Input**: Current board state
- **Logic**: Selects from available positions
- **Update**: Places 'X' on the chosen square

## 🚀 Future Improvements

Potential enhancements for the project:

- [ ] **Difficulty Levels**: Easy, Medium, Hard AI opponents
- [ ] **Minimax Algorithm**: Implement unbeatable AI using minimax with alpha-beta pruning
- [ ] **GUI Interface**: Add graphical interface using Tkinter or Pygame
- [ ] **Multiplayer Mode**: Add player vs player option
- [ ] **Score Tracking**: Keep track of wins, losses, and draws across multiple games
- [ ] **Save/Load Game**: Ability to save game state and continue later
- [ ] **Customizable Board Size**: Support for larger grids (4x4, 5x5)
- [ ] **Online Multiplayer**: Network play capabilities
- [ ] **Statistics Dashboard**: Track gameplay statistics and performance
- [ ] **Undo/Redo Moves**: Allow players to reverse moves

## 🛠️ Technologies Used

- **Language**: Python 3.x
- **Libraries**: Standard Python libraries only (random)
- **Paradigm**: Procedural programming

## 📝 License

This project is open source and available for educational purposes.

## 👤 Author

**Ekumby Travessa**
- GitHub: [@Narva35](https://github.com/Narva35)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## ⭐ Show your support

Give a ⭐️ if you like this project!

---

**Note**: This project was created as a learning exercise to demonstrate fundamental programming concepts including:
- Functions and modular code design
- List manipulation and 2D arrays
- Game logic and win condition algorithms
- Input validation and error handling
- Basic AI implementation
