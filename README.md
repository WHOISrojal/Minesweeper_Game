# Minesweeper Game
This project is a Java implementation of the classic Minesweeper game. The game features a 16x16 grid with 40 mines hidden within. The goal is to uncover all cells that do not contain mines, using logical deduction based on the numbers revealed by uncovered cells.

## Project Structure
The project consists of two main classes:

1. Board.java
Purpose: Handles the game logic, including mine placement, cell uncovering, and game state management.
Key Features:
- Game Initialization: Sets up the board, including randomly placing mines and calculating adjacent mine counts for each cell.
- Cell Interaction: Implements logic for uncovering cells, marking cells, and determining the outcome of the game (win/loss).
- Rendering: Draws the game board and updates the visuals based on the player's actions.
- Mouse Input: Handles mouse events for interacting with the game, such as uncovering cells or marking them with flags.
  
2. Minesweeper.java
Purpose: Acts as the main entry point for the game, setting up the user interface and launching the game.
Key Features:
- UI Setup: Initializes the JFrame, adds the game board, and sets up the status bar to display the number of remaining mines or game messages (win/loss).
- Game Launch: Uses EventQueue to start the game on the event-dispatching thread.
  
## How to Play
1. Left-Click: Uncover a cell. If the cell contains a mine, the game is lost. If it doesn't, a number will be revealed indicating how many mines are adjacent to that cell.
2. Right-Click: Mark a cell as containing a mine. This helps in keeping track of where you believe mines are located.
3. Winning the Game: Uncover all cells that do not contain mines.
4. Losing the Game: Uncover a cell that contains a mine

## Installation
To run the Minesweeper game, you'll need to have Java installed on your machine. Follow these steps:

1. Clone the Repository:
```
git clone https://github.com/WHOISrojal/Minesweeper_Game.git
cd minesweeper
```

2. Compile the Source Files:
```
javac -d bin src/com/zetcode/*.java
```

3. Run the Game:
```
java -cp bin com.zetcode.Minesweeper
```

## Resources
The game uses a set of images (icons) for rendering the board and game elements. These images are stored in the src/resources/ directory and are loaded during the game's initialization.


Src Code: All Credits to 
> http://zetcode.com/javagames/minesweeper/


