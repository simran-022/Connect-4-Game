INTRODUCTION:

Connect Four is a classic two-player strategy game that has been enjoyed by people of all ages since its introduction in the 1970s. 
The game is played on a vertical grid of seven columns and six rows, and the objective is to connect four of your colored disks in a row, either vertically, horizontally, or diagonally, before your opponent does the same.The game requires players to carefully plan their moves, as they must try to connect their disks while 
also blocking their opponent's attempts to do the same.
Connect Four is a game of skill that requires players to think ahead and make strategic decisions. It is also a game that can be enjoyed by players of all skill levels, from beginners to experts. 
The simplicity of the game makes it easy to learn, but the strategic depth ensures that players can continue to improve and develop their skills over time.
The game has also been the subject of research in computer science and artificial intelligence, as it provides an interesting challenge for the development of algorithms and machine learning models. Overall, Connect Four is a timeless classic that continues to captivate players and challenge them to outwit their opponents.

PROBLEM STATEMENT:

Write a program that allows a user to play against the computer in Connect Four. The program should provide a graphical user interface and use an algorithm to determine the computer's moves and make informed decisions based on the current state of the game.

GAME RULES:

1. Connect Four is a two players game which takes place on a 7x6 rectangular board placed vertically between them.
2. One player has 21 Yellow discs and the other 21 Red discs.
3. Each player can drop a disc at the top of the board in one of the seven columns; the disc falls down and fills the lower unoccupied square.
4. Of course a player cannot drop a disc in a certain column if it's already full (i.e. it already contains six discs).
5. Even if there's no rule about who begins first, we assume, as in chess, that the yellow side makes the first move.
6. We also use the chess notation to represent a square on the board. That is, we number rows from 1 to 7 starting from the bottom and the columns from A to G 
starting from the leftmost.
7. The objective of the game is to connect four discs vertically, horizontally or diagonally.
8. If the board is filled and no one has aligned four discs then the game is drawn (i.e. after 42 moves if no one wins).

ALGORITHMS USED:

1. Mini-max algorithm:
It is a recursive or backtracking algorithm which is used in decision-making and game theory. It provides an optimal move for the player assuming that the opponent is also playing optimally. Both players of the game are opponents of each other, where MAX (Player 1) will select the maximized value and MIN (Player 2) will select the minimized value.

2. Alpha-beta pruning:
It is a modified version of the minimax algorithm. It is an optimization technique for the minimax algorithm.

Alpha: The best (highest-value) choice we have found so far at any point along the path of Maximizer. The initial value of alpha is -∞. 

Beta: The best (lowest-value) choice we have found so far at any point along the path of Minimizer. The initial value of beta is +∞.

Main condition required for alpha-beta pruning: α>=β.

The Alpha-beta pruning to a standard minimax algorithm returns the same move as the standard algorithm does, but it removes all the nodes which are not really affecting the final decision but making the algorithm slow. Hence by pruning these nodes, it makes the algorithm fast. The Max player will only update the value of alpha and the Min player will only update the value of beta.

