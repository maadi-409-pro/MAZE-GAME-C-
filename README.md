# MAZE-GAME-C-
A simple console-based maze game in C++ where players navigate a character (@) to the goal (()) using arrow keys, avoiding obstacles and boundaries.


Libraries Used:

<iostream>: For input/output operations.
<windows.h>: To control the console screen (e.g., cursor position).
<conio.h>: For non-blocking keyboard input (_kbhit and _getch).

Constants and Structs:

Width and Height: Define the maze dimensions.
Position: A struct to store x and y coordinates of objects (player and destination).

FUNCTIONS:
gotoxy(int x, int y): Moves the cursor to a specific position in the console.
screen(): Draws the maze boundary using #.
maze(): Creates the maze with obstacles using *.
drawPositions(Position playerPos, Position destPos): Draws the player (@) and destination (()).
checkCollision(Position newPos): Prevents movement into walls or outside the maze.
checkWin(Position playerPos, Position destPos): Checks if the player has reached the destination.

Game Loop:

Continuously listens for keyboard input using _kbhit() and _getch().
Updates the player position based on arrow key input.
Redraws the player only if the new position is valid (no collision).
Checks for the win condition after each move.

CONTROLS:

Arrow Keys: Move the player (@) through the maze.

------------------------------------------------------------------------------------------------------------------------------------------


