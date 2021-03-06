puzzle solver
==============

Java application used to solve the 8-puzzle. It uses A* search algorithm. The Manhattan Distance is its search heuristic.

The layouts of starting board and goal board are decided in the main method. Simply change the numbers in the initialized matrix that represents the starting board. Do note that numbers 0 - 8 must exist in the board and each number can only occur once. 0 is considered an empty tile
and moves on the board always originate from the position of this tile. Also note that permutating the goal layout might lead to a search that goes on for infinity. I think that "unsolvable" goal layouts give this behaviour, but haven't been able to prove it yet.

The whole idea of 8-puzzle is to go from this board:

[8,0,6]<br>
[5,4,7]<br>
[2,3,1]

to:

[0,1,2]<br>
[3,4,5]<br>
[6,7,8]

moving one tile at a time. Diagonal operations are not permitted.

How to run it
------------

Run the make file by writing 'make' in the terminal. you will see how the board permutates and what move was
performed.
