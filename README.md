# 2048 Game Implementation in C++

## Project Name: 2048 Game Implementation in C++

### Overview:
This project is an implementation of the popular single-player sliding tile puzzle game "2048". The objective of the game is to slide numbered tiles on a grid to combine them and create a tile with the number 2048. The project uses C++ for the core logic and the console for user interaction.

### Key Features:

#### Grid Initialization:
- The game initializes with a 4x4 grid with two tiles, containing numbers 2 and 4, placed at random positions.

#### Tile Movement:
- The game supports four types of movements: up, down, left, and right.
- Tiles slide as far as possible in the chosen direction until they encounter another tile or the edge of the grid.
- If two tiles with the same number collide while moving, they merge into a tile with the sum of their numbers.

#### New Tile Addition:
- After each move, a new tile with a value of either 2 or 4 appears at a random empty position on the grid.

#### Game Interface:
- The game provides a simple console interface to display the current state of the grid.
- It includes visual separation between tiles and clearly shows the numbers on each tile.

#### Game Controls:
- The player uses the arrow keys to move the tiles up, down, left, or right.
- Pressing the 'Esc' key allows the player to exit the game at any time.

#### Game Over Condition:
- The game checks for available moves after every turn. If no moves are possible and the grid is full, the game displays a "Game Over" message.

#### Tile Merging Logic:
- The merging logic ensures that a tile can only merge once per move, preventing multiple merges in a single move sequence.

### Code Explanation:

#### Movement Functions:
- `void upmove(int a[4][4])`
- `void downmove(int a[4][4])`
- `void leftmove(int a[4][4])`
- `void rightmove(int a[4][4])`
- Each of these functions handles the movement and merging of tiles in the specified direction.

#### Grid Display Function:
- `void disp(int a[4][4])`
- This function displays the current state of the grid in a visually appealing manner in the console.

#### Tile Addition Function:
- `void addblock(int a[4][4])`
- This function adds a new tile with a value of 2 or 4 at a random empty position on the grid.

#### Game State Check Functions:
- `int check(int tmp[4][4], int a[4][4])`
- `int checkover(int a[4][4])`
- These functions check if the grid has changed after a move and if there are any possible moves left, respectively.

#### Main Function:
- The main function initializes the grid, handles user input for tile movements, updates the grid state, and checks for the game-over condition.

### Execution:
- The game starts with an introduction screen, prompting the player to press any key to begin.
- The grid is displayed, and the player can make moves using the arrow keys.
- After each move, the grid updates, and a new tile is added.
- The game continues until no more moves are possible, at which point a "Game Over" message is displayed.

This project provides a simple yet functional implementation of the 2048 game, demonstrating basic game development principles and C++ programming skills.
