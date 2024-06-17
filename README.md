Specific features to consider:
Display the board. After asking us for our names, the program prints out a 3×3 board filled with dashes, signifying empty spots.
Take turns placing noughts and crosses. Each turn it asks either player 1 or player 2 to enter a row and col index which is where they want to place their x and o, and then the board is printed again with the x or o in the right spot.
Skip invalid plays. If the position the player entered is “off the board” or already has an x or o on it, then our program notifies the player, who is prompted to enter another row and col?
State the result. Once the player wins by getting 3 in a row, column, or diagonal, the program prints that player 1 or 2 has won and prints out the final board.
General order of steps to implement:
Create a Tic Tac Toe board and fill it with dashes.
Create a function that draws the board like a square.
Keep track of the player’s turn and what symbol they are using.
Keep asking the user to enter a row and col until they are valid.
Set the right position on the board to the proper symbol.
Create a function that checks if either player has won.
Check draw: check if the game has ended in a tie.
Use a loop to keep the game going.
How do we do each of these steps?
Step 1: Create a 3×3 array to represent the tic tac toe board and fill it with dashes.
We need to make a 2D array of characters, which can be x, o, or -.

Hint: We can use the following line of code to make a 3×3 array of chars: char[][] board = new char[3][3]

Now we have to fill our board with dashes.

Hint: We can use a nested for loop to iterate through each position on our board. Inside both for loops, we can set board[i][j] equal to a dash.

Step 2: Ask the users for their names.
First, we import the Scanner to help us get user input by adding import java.util.Scanner to the top of our program.
Then, we initialize our Scanner variable by making a new ScannerNext, we print out a message asking the user to type in their name using System.out.print().
We store their input in a String called p1.
Do the same for p2.
Step 3: Create a function that draws the board and prints it out like a 3×3 square.
In order for our function to draw the board and print it out, do we need to pass a parameter into the function? Do we need to return anything?
Hint: We need to pass in the board 2D array in order for the function to be able to print it. We don’t need to return anything since the function is simply printing out the board.
Inside our function, we need to print out each position on our board.
Hint: If we do System.out.println(), then each position is on a new line.
Hint: If we do System.out.print(), then all of the positions are on one line.
Hint: We can do System.out.print() in the inner for loop, and do System.out.println() at the end of the outer for loop so that it starts a new line after each row has been printed.
