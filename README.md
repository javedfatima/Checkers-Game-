CHECKERS GAME 

DESCRIPTION:

Build a 2-player checkers game. The game supports standard Checkers rules including piece 
movement, jumping/capturing, and king promotion. It also includes functionality to save and 
load game state using a text file. 

FEATURES: 

• 8x8 game board display 
• Turn-based player control (red vs black) 
• Jump captures and validates simple moves 
• Automatically promotes pieces to king 
• Game state is saved after every valid move 
• A saved file can be reopened 

SETUP 

Dependencies: 
• A C++ compiler 
• An IDE like visual studio 2022 

HOW TO RUN THIS PROJECT: 

• Download the project files 
• Compile the code and run the executable program. 

HOW TO PLAY: 
1. The game starts with a black player 
2. Valid moves include:  
• Diagonal step to an empty square
• Jumping over an opponent's piece (capture) 
4. Pieces are promoted to kings when they reach the opponent's last row. 

SAVE/ LOAD GAME: 
Game state is saved in checkers_save.txt. On launch, the program attempts to load the last 
saved state. If the save file doesn't exist, a new game is initialized. 

CODE OVERVIEW: 
Functions use: 
• initializeBoard(): Sets up the board with red and black pieces. 
• displayBoard(): Prints the current state of the board. 
• movePiece(int, int, int, int): Executes the move, handles captures, and 
promotions. 
• saveGame() / loadGame(): Handles persistent storage of the game state. 
• isValidMove(int, int, int, int): Validates player moves based on Checkers rules. 
• hasWon(char player): Determines if the current player has won. 
• canJump(int, int): Checks if a piece can perform a jump. 
