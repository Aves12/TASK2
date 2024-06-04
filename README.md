# Question 2: Design a Fixed Player Online Game (Snake & Ladder)

## Assumptions

The game is designed for two players, playing against each other.
The game board consists of 30 cells, with some cells having ladders or snakes.
The players roll a dice to determine how many cells they can move.
The game ends when one player reaches the last cell (cell 30).

## Reason behind assumptions:

A fixed number of players simplifies the game design and implementation.
Turn-based games are easier to implement and manage than real-time games.
A server is necessary to handle game logic and store game state, ensuring a consistent experience for all players.

## APIs Available:

Game API: Provides functionality to create a new game, join an existing game, and make moves.
Player API: Manages player information, such as username, password, and game history.
Game Board API: Provides the game board layout, including ladder and snake positions.

## Game Objects Involved:

Game: Represents the game instance, including the game board, players, and game status.
Player: Represents a player, including their username, password, and game history.
Game Board: Represents the game board, including the layout of cells, ladders, and snakes.
Cell: Represents a single cell on the game board, including its position and any ladder or snake connections.
Ladder: Represents a ladder on the game board, including its start and end cells.
Snake: Represents a snake on the game board, including its start and end cells.
Dice: Represents the dice used to determine player moves.
sion.
Board: Represents the game board and pieces.
