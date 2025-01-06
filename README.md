# Tic Tac Toe Game

A Python-based command-line implementation of the classic Tic Tac Toe game for two players. This project demonstrates core programming concepts such as loops, conditional logic, and function-based design while being an enjoyable interactive experience.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [How to Run](#how-to-run)
5. [Game Rules](#game-rules)
6. [How to Play](#how-to-play)
7. [Code Overview](#code-overview)
8. [Code Structure](#code-structure)
9. [Dependencies](#dependencies)
10. [Example Gameplay](#example-gameplay)
11. [Known Issues](#known-issues)
12. [Future Enhancements](#future-enhancements)
13. [License](#license)

---

## Introduction

Tic Tac Toe is a classic strategy game for two players. The objective is to align three of your marks (either `X` or `O`) in a horizontal, vertical, or diagonal row on a 3x3 grid. This project implements the game in Python with a clean and modular design, making it easy to understand and extend.

---

## Features

- Interactive command-line interface.
- Two-player gameplay.
- Automatic checks for win or tie conditions.
- Dynamic board updates after every move.
- Clear modular code structure, suitable for beginners and learners.

---

## Getting Started

### Prerequisites
To run this project, you need:
- **Python 3.6 or higher** installed on your system.

### Installation
1. Clone the repository or download the project files.
   ```bash
   git clone https://github.com/your-repo/tic-tac-toe.git
   ```
2. Navigate to the project directory.
   ```bash
   cd tic-tac-toe
   ```

---

## How to Run

To start the game:
1. Open a terminal or command prompt.
2. Run the script using Python:
   ```bash
   python tic_tac_toe.py
   ```

---

## Game Rules

1. The game is played on a 3x3 grid.
2. Players take turns placing their marks (`X` or `O`) in an empty spot.
3. The first player to get three of their marks in a horizontal, vertical, or diagonal row wins.
4. If all spots are filled and no player has won, the game ends in a tie.

---

## How to Play

1. The game displays the board with positions labeled from 1 to 9.
2. Players are prompted to input a number corresponding to their desired position.
3. The game validates the input and updates the board accordingly.
4. The game checks for a win or tie after each move.
5. The current player switches until the game ends.

---

## Code Overview

### Key Concepts
- **Dynamic Input Handling:** Ensures players provide valid positions.
- **Game State Management:** Tracks the game's progress, winner, and current player.
- **Logic Separation:** Functions are modular for specific tasks (e.g., checking rows, flipping players).

---

## Code Structure

### Global Variables
- **`board`**: Represents the 3x3 game grid.
- **`game_still_going`**: Boolean flag for the game's active state.
- **`winner`**: Tracks the winner (`X`, `O`, or `None` for a tie).
- **`current_player`**: Indicates whose turn it is (`X` or `O`).

### Functions
1. **`play_game()`**: The main game loop.
2. **`display_board()`**: Prints the current game board.
3. **`handle_turn(player)`**: Processes the player's move.
4. **`check_if_game_over()`**: Checks for win or tie conditions.
5. **`check_for_winner()`**: Identifies if there's a winner.
6. **`check_rows()`, `check_columns()`, `check_diagonals()`**: Validates win conditions for rows, columns, and diagonals.
7. **`check_for_tie()`**: Checks if the board is full without a winner.
8. **`flip_player()`**: Switches the active player.

---

## Dependencies

This project has no external dependencies and runs on a standard Python environment.

---

## Example Gameplay

### Initial Board
```
- | - | -     1 | 2 | 3
- | - | -     4 | 5 | 6
- | - | -     7 | 8 | 9
```

### Sample Session
```
X's turn.
Choose a position from 1-9: 5

- | - | -     1 | 2 | 3
- | X | -     4 | 5 | 6
- | - | -     7 | 8 | 9

O's turn.
Choose a position from 1-9: 1

O | - | -     1 | 2 | 3
- | X | -     4 | 5 | 6
- | - | -     7 | 8 | 9

X's turn.
Choose a position from 1-9: 9

O | - | -     1 | 2 | 3
- | X | -     4 | 5 | 6
- | - | X     7 | 8 | 9
```

---

## Known Issues

- **Input Validation**: Only accepts valid numbers but may loop unnecessarily for invalid input.
- **Scalability**: Limited to a 3x3 grid; doesn't support larger board sizes.

---

## Future Enhancements

1. Add single-player mode with AI:
   - Easy: Random moves.
   - Hard: Minimax algorithm for unbeatable AI.
2. Support custom board sizes (e.g., 4x4, 5x5).
3. Implement a graphical user interface (GUI) using `Tkinter` or `Pygame`.
4. Add a replay option after the game ends.
5. Optimize input validation for better user experience.

---

## License

This project is open-source and available under the [MIT License](LICENSE).

---

Happy Coding! 🎮
