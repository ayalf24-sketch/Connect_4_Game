**Connect Four (Python)**

I created a Python implementation of Connect Four that features a customizable board, human and AI players, and support for multiple win conditions. This project was completed as part of a freshman-level course project.

**Features**
-Customizable Board: Create a board with any height and width. Display the board in a clean, console-friendly format.
-Gameplay Mechanics: Place checkers ('X' or 'O') in columns. Check for horizontal, vertical, and diagonal wins. Detect ties when the board is full. Reset the board to start a new game.

-Player Types: Human Player: Input moves manually. Random AI Player: Chooses valid moves randomly. Intelligent AI Player: Uses a lookahead algorithm with configurable depth and tiebreak strategies (LEFT, RIGHT, RANDOM).

-Game Flow: Alternating turns between two players. Automatic win and tie detection. Tracks the number of moves made by each player.

**Modules**
Board (Board):

Handles board state, adding/removing checkers, and win/tie detection.

Player (Player):

Base class for players. Tracks checker type and number of moves.

Game Logic (connect_four):

Manages game loop and turn processing for human and AI players.

AI Player (AIPlayer):

Subclass of Player that evaluates board positions using a lookahead strategy to select optimal moves.

**Implementation Notes**

The board is represented as a 2D list of strings.

Horizontal, vertical, and diagonal win checks are implemented as separate methods in Board.

AI uses a recursive lookahead strategy to evaluate moves up to a specified depth.

The next_move method ensures moves are valid before adding checkers to the board.

