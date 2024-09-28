**Overview**

First to 15 is a console-based two-player game where the goal is to be the first to achieve a sum of 15 across any row, column, or diagonal on a 3x3 grid. The game can be played in two modes: Player vs. Player (PvP) or Player vs. Computer (PvC). The game integrates basic C programming concepts such as arrays, random number generation, and control structures.

**How to Play**

Game Modes
Player vs. Player (PvP): Two human players take turns selecting positions on the grid and choosing numbers between 1 and 9. Each number can only be used once during the game.
Player vs. Computer (PvC): The player competes against the computer. The player makes a move, and the computer responds with its own move, both selecting positions on the grid and numbers from 1 to 9.
Game Objective
The objective is to be the first player to reach a total of 15 across any row, column, or diagonal on the board.
Players take turns choosing a position on the 3x3 board (labeled A-I) and a number between 1 and 9 that hasn't already been chosen.
Winning Criteria
A player wins if they achieve a sum of 15 with their chosen numbers in a row, column, or diagonal.
If all positions on the board are filled without either player achieving a sum of 15, the game ends in a draw.

**Game Components**

Main Functions
int main(): The entry point of the game. Displays the main menu and allows the player to choose between PvP, PvC, or exit the game.

int pvp(): Handles the Player vs. Player game logic. Players take turns selecting positions and numbers until a winner is determined or the game is a draw.

int pvc(): Handles the Player vs. Computer game logic. The player and computer alternate turns, with the computer making random valid moves.

void theboard(): Updates and displays the current state of the game board, showing the positions chosen by each player and their corresponding numbers.

void thepositionboard(): Displays the grid with the available positions (A-I) that players can choose from.
void checkcount(): Ensures that the selected number hasn't been used before. If it has, the player is prompted to choose another number.

int checkifsomeonewon(): Checks if any player has won by achieving a sum of 15 across a row, column, or diagonal.

void picker(): Generates the computer's move by randomly selecting an available position and an unused number.

int choosingletters(): Allows the player to choose a position on the board by entering a letter (A-I).
void replacement(): Updates the board with the player's chosen position and number.

void winner(): Displays the result of the game, indicating if there is a winner or if the game ends in a draw.

Key Variables

int pos[10]: Stores the numbers chosen by the players.

int playerno[10]: Stores the player number (1 or 2) corresponding to the positions on the board.

char boardchoice[10]: Holds the letters A-I representing positions on the board.

int testarr[10]: Used to track numbers already chosen by the players.

int testarrforcomp[10]: Ensures that the computer does not repeat a number or position.

char numchar[20]: Stores the player's input for the number selection.

**Installation and Setup**

Requirements: Ensure you have a C compiler installed, such as GCC.

Compiling the Code: 
Compile the code using a C compiler with the following command:

sh
Copy code
gcc -o first_to_15_game first_to_15_game.c -lm

Running the Game: 
Run the compiled program:

sh
Copy code
./first_to_15_game

**Credits**

This game was developed as a practice project to explore basic game logic implementation in C. It demonstrates the use of functions, arrays, and basic game design principles.

Enjoy the game, and may the best player win!
