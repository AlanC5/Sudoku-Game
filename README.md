# Sudoku-Game
Initializes a sudoku board and allows for rearrangement of column or rows, but maintains all necessary rules to be a completed Sudoku puzzle  

Commands include 'show', 'swap', 'verify', 'erase', or 'quit'.

*show*: Displays the current state of the board

*swap*: Randomly swaps a row or column. If the chosen column or board will interfere with a completed sudoku board, then the respective section will be switched. A section includes 3 rows or 3 columns. For example, A,B,C and S,T,U are sections. 

*verify*: Check if the board adhere to all the requirements of a completed sudoku board. The outcome will change onces the 'erase' command is applied.

*erase*: Randomly erases a number on the board and replaces it with a '-'

*quit*: Quit the program


# Example
```
Welcome to Sudoku Initializer!
> No
Error: Please enter 'show', 'swap', 'verify', 'erase', or 'quit'. Thank you!
> show
   A B C D E F G H I 
P  1 4 7 5 8 2 9 3 6 
Q  2 5 8 6 9 3 1 4 7 
R  3 6 9 7 1 4 2 5 8 
S  4 7 1 8 2 5 3 6 9 
T  5 8 2 9 3 6 4 7 1 
U  6 9 3 1 4 7 5 8 2 
V  7 1 4 2 5 8 6 9 3 
W  8 2 5 3 6 9 7 1 4 
X  9 3 6 4 7 1 8 2 5 

> swap
Trying to swap columns H and F...
- Rows D and G were swapped...
- Rows E and H were swapped...
- Rows F and I were swapped...
> show
   A B C D E F G H I 
P  1 4 7 9 3 6 5 8 2 
Q  2 5 8 1 4 7 6 9 3 
R  3 6 9 2 5 8 7 1 4 
S  4 7 1 3 6 9 8 2 5 
T  5 8 2 4 7 1 9 3 6 
U  6 9 3 5 8 2 1 4 7 
V  7 1 4 6 9 3 2 5 8 
W  8 2 5 7 1 4 3 6 9 
X  9 3 6 8 2 5 4 7 1 

> swap
Trying to swap rows T and X...
- Rows S and V were swapped...
- Rows T and W were swapped...
- Rows U and X were swapped...
> show
   A B C D E F G H I 
P  1 4 7 9 3 6 5 8 2 
Q  2 5 8 1 4 7 6 9 3 
R  3 6 9 2 5 8 7 1 4 
S  7 1 4 6 9 3 2 5 8 
T  8 2 5 7 1 4 3 6 9 
U  9 3 6 8 2 5 4 7 1 
V  4 7 1 3 6 9 8 2 5 
W  5 8 2 4 7 1 9 3 6 
X  6 9 3 5 8 2 1 4 7 

> swap
Trying to swap rows Q and X...
- Rows P and v were swapped...
- Rows Q and w were swapped...
- Rows R and x were swapped...
> show
   A B C D E F G H I 
P  4 7 1 3 6 9 8 2 5 
Q  5 8 2 4 7 1 9 3 6 
R  6 9 3 5 8 2 1 4 7 
S  7 1 4 6 9 3 2 5 8 
T  8 2 5 7 1 4 3 6 9 
U  9 3 6 8 2 5 4 7 1 
V  1 4 7 9 3 6 5 8 2 
W  2 5 8 1 4 7 6 9 3 
X  3 6 9 2 5 8 7 1 4 

> swap
Trying to swap rows X and V...
- Rows X and V were swapped...
> show
   A B C D E F G H I 
P  4 7 1 3 6 9 8 2 5 
Q  5 8 2 4 7 1 9 3 6 
R  6 9 3 5 8 2 1 4 7 
S  7 1 4 6 9 3 2 5 8 
T  8 2 5 7 1 4 3 6 9 
U  9 3 6 8 2 5 4 7 1 
V  3 6 9 2 5 8 7 1 4 
W  2 5 8 1 4 7 6 9 3 
X  1 4 7 9 3 6 5 8 2 

> verify
- All columns, rows, and components are OK...
> erase
Erasing row X column A
> verify  
- Found inconsistency in row X...
- Found inconsistency in column A...
- Found inconsistency in component starting at row V and column A...
> erase
Erasing row R column H
> verify
- Found inconsistency in row R...
- Found inconsistency in row X...
- Found inconsistency in column A...
- Found inconsistency in column H...
- Found inconsistency in component starting at row V and column A...
- Found inconsistency in component starting at row P and column G...
> swap
Trying to swap columns H and B...
- Rows A and G were swapped...
- Rows B and H were swapped...
- Rows C and I were swapped...
> show  
   A B C D E F G H I 
P  8 2 5 3 6 9 4 7 1 
Q  9 3 6 4 7 1 5 8 2 
R  1 - 7 5 8 2 6 9 3 
S  2 5 8 6 9 3 7 1 4 
T  3 6 9 7 1 4 8 2 5 
U  4 7 1 8 2 5 9 3 6 
V  7 1 4 2 5 8 3 6 9 
W  6 9 3 1 4 7 2 5 8 
X  5 8 2 9 3 6 - 4 7 

> verify
- Found inconsistency in row R...
- Found inconsistency in row X...
- Found inconsistency in column B...
- Found inconsistency in column G...
- Found inconsistency in component starting at row P and column A...
- Found inconsistency in component starting at row V and column G...
> quit
```
