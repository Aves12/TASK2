# Question 2: Design a Fixed Player Online Game (Chess)

## Assumptions
Game Type: The game is turn-based and involves two players.
Reason: Chess is inherently a two-player game.
Real-time Interaction: The game needs to handle real-time moves between players.
Reason: To maintain the flow and integrity of the game.
State Persistence: The game state must be saved to handle disconnections.
Reason: Players may disconnect and need to resume the game.

## Reason behind assumptions:

A fixed number of players simplifies the game design and implementation.
Turn-based games are easier to implement and manage than real-time games.
A server is necessary to handle game logic and store game state, ensuring a consistent experience for all players.
## System Design
Game Server: Handles game state, player moves, and communications.
Framework: Flask or Django with WebSockets
Database: Stores player information, game state, and history.
Database: PostgreSQL
APIs:
POST /start_game: Initiates a new game.
POST /move: Submits a player's move.
GET /game_state: Retrieves the current state of the game.

## Game Objects:
Player: Represents a player in the game.
Game: Represents the game session.
Board: Represents the game board and pieces.
