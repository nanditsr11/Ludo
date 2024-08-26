## Classes:

gridObj: Represents each cell on the board with attributes like background color, list of players (tokens), whether it's a safe spot, and coordinates.
Token: Represents a player's token, with attributes for ID, color, state, coordinates, size, and original coordinates.

## Initialization:

Board Setup: Game_grid is a 15x15 grid initialized with gridObj objects.
Color and Coordinate Matrices: Define the layout and appearance of the board.
Safe Locations: safeLocs and safeMatrix indicate safe zones where tokens cannot be captured.
Player Initialization: Tokens are placed in their starting positions.

## Game Mechanics:

Movement: The move function calculates new positions based on dice rolls and the current player.
Collision Handling: The checkCollision function resets tokens to their starting positions if they collide with an opponent's token.
Token Drawing: The drawGrid function handles the rendering of the board and tokens.

## Main Game Loop:

Handles mouse events, dice rolls, token movement, and player turn transitions.
