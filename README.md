This Go game mini-program is implemented in Python, mainly utilizing the tkinter and time libraries.
It employs a depth-first search (DFS) algorithm and uses a 0-1 matrix to manage the placement of black and white stones.

Design Concept:
The primary functions that need to be realized for this Go mini-game include: 
drawing the board, placing black and white stones, capturing stones, scoring and settlement, and timing functions. Below is an introduction to the implementation of each of these features.

Drawing the Board:
Using the tkinter library, a window is first created, and then a grid of square orange buttons (19x19) is generated in a loop within the window to form the game board.

Placing Black and White Stones:
Each button is given the functionality to change color upon being clicked. 
When a button is clicked, the corresponding square changes to either black or white. This color change alternates with each click, meaning the effect of the previous click is different from the next. 
This is controlled by a variable count that toggles between -1 and 1, switching its value with each click.

Capturing Stones:
After a move is made (when a button is clicked), the corresponding position in the matrix is updated with a value of -1 or 1 to represent different colored stones. 
Following this update, the program checks if the surrounding stones of the opposite color have "liberties" (empty adjacent points). 
This is determined using a depth-first search (DFS) algorithm, which checks for adjacent empty spaces or stones of the same color. 
If an empty space is found, the group is alive; if adjacent stones of the same color are found, it continues checking those. 
If no liberties are found, the stones are captured, the matrix value is set to 0, and the stone's color is changed back to orange.
