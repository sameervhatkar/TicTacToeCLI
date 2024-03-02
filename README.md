# TicTacToeCLI
Description:

Game Initialization:
  The program starts by initializing a 3x3 tic-tac-toe board represented by a 2D array called board.
  
User Input and Game Control:
  The main game loop (while loop) runs until there are 9 moves or until a winner is declared.
  The loop prompts the user to enter a row, column, and symbol for their move.
  
Symbol Occurrences Tracking:
  Two HashMaps (hmrow and hmcol) are used to track the occurrences of symbols in rows and columns.
  The outer HashMaps (hmrow and hmcol) use row and column indices as keys, respectively.
  The inner HashMaps store the counts of each symbol in the corresponding row or column.
  
Move Processing:
  For each move, the program checks if the symbol already exists in the current row or column using the inner HashMaps.
  If the symbol is found, its count is incremented. If the count reaches 3, the player wins, and the game ends.
  If the symbol is not found, a new entry is added to the inner HashMap with a count of 1.
  
Game Result:
  After each move, the program checks if a player has won in the current row or column.
  If a winner is found, the program prints the winner's symbol and exits the loop.
  If the loop completes without finding a winner, and the flag is still true, it means the game ended in a draw.
  
Input Validation and Incrementing Move Count:
  The program uses putIfAbsent to ensure that the inner HashMaps are initialized for the specified row and column.
  The count variable is incremented after each move to keep track of the total number of moves.
  
Print Result:
  Finally, the program prints the result of the game, indicating whether it ended in a draw.
  
This implementation focuses on tracking symbol occurrences in rows and columns and determining the winner or a draw based on these occurrences. It's a simplified version of a tic-tac-toe game for learning purposes.

Output:
Please enter where you want to make a move and symbol
2 2 X

Please enter where you want to make a move and symbol
2 1 0

Please enter where you want to make a move and symbol
1 1 X

Please enter where you want to make a move and symbol
0 0 0

Please enter where you want to make a move and symbol
2 0 X

Please enter where you want to make a move and symbol
0 2 0

Please enter where you want to make a move and symbol
0 1 X

Please enter where you want to make a move and symbol
1 0 0

Please enter where you want to make a move and symbol
1 2 X

Draw

