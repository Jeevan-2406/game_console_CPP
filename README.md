# Game Console with C++

This project is a game console application implemented in C++ using the SFML library. It features multiple games that can be selected and played from a main menu.

## Project Structure

### The project consists of the following main components:

1. `main.cpp`: The entry point of the application, containing the `GameConsole` class.
2. `SnakeGame.hpp`: Implementation of the Snake game.
3. `TicTacToe.hpp`: Implementation of the Tic-Tac-Toe game.
4. `RockPaperScissors.hpp`: Implementation of the Rock Paper Scissors game.
5. `ConnectFour.hpp`: Implementation of the Connect Four game.
6. `HighScore.hpp`: A high score system used by the Snake game.
7. `arial.ttf`: Font file used for text rendering.

## Workflow

### 1. Main Menu (GameConsole class)

- The application starts by creating an instance of the `GameConsole` class.
- The main menu is displayed, showing options for different games and an exit option.
- Users can navigate the menu using keyboard arrows or mouse.
- Selecting a game initializes and runs that game.

### 2. Game Initialization

- When a game is selected, its respective class is instantiated (e.g., `SnakeGame`, `TicTacToe`, etc.).
- Each game is initialized with the main window and font as parameters.

### 3. Game Loop

Each game follows a similar structure:

a. Initialization:
   - Set up game-specific variables, UI elements, and initial state.

b. Main Loop:
   - Handle events (user input)
   - Update game state
   - Render graphics

c. Game Over:
   - Display results
   - Option to return to main menu

### 4. Specific Game Workflows

#### Snake Game
- Players control a snake, eating food to grow longer.
- Includes obstacles and difficulty settings.
- Maintains a high score system.

#### Tic-Tac-Toe
- Two-player game on a 3x3 grid.
- Players take turns placing X or O.
- Checks for win conditions or draw.

#### Rock Paper Scissors
- Player vs Computer game.
- Best of 3, 5, or 7 rounds.
- Animated result display.

#### Connect Four
- Two-player game on a 6x7 grid.
- Players drop discs to form a line of four.
- Includes dropping animation and win detection.

### 5. Return to Main Menu

- After a game ends, players can choose to return to the main menu.
- The game-specific instance is destroyed, and control returns to the `GameConsole` class.

## Key Features

- Modular design allowing easy addition of new games.
- Consistent UI elements across games (buttons, text, etc.).
- Use of SFML for graphics and event handling.
- Implementation of game-specific logic and rules.
- High score system for the Snake game.

## Dependencies

- SFML library for graphics and window management.
- C++ compiler supporting C++11 or later.
- `arial.ttf` font file for text rendering.

## Compilation and Running

Ensure SFML is installed and properly linked in your development environment. Compile all `.cpp` files together and run the resulting executable.
 