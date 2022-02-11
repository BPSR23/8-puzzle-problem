# 8-puzzle-problem

We also know the eight puzzle problem by the name of N puzzle problem or sliding puzzle problem.

N-puzzle that consists of N tiles (N+1 titles with an empty tile) where N can be 8, 15, 24 and so on.

In our example N = 8. (that is square root of  (8+1) = 3 rows and 3 columns).

In the same way, if we have N = 15, 24 in this way, then they have Row and columns as follow (square root of (N+1) rows  and square root of (N+1) columns).

That is if N=15 than number of rows and columns= 4, and if N= 24 number of rows and columns= 5.

So, basically in these types of problems we have given a initial state or initial configuration (Start state) and a Goal state or Goal Configuration.

Here We are solving a problem of 8 puzzle that is a 3x3 matrix.

Initial state                                                                      Goal state

                                                               

Solution:
The puzzle can be solved by moving the tiles one by one in the single empty space and thus achieving the Goal state.

Rules of solving puzzle

Instead of moving the tiles in the empty space we can visualize moving the empty space in place of the tile.

The empty space can only move in four directions (Movement of empty space)

Up 
Down 
Right or
Left
The empty space cannot move diagonally and can take only one step at a time.


All possible move of a Empty tile



o- Position total possible moves are (2), x - position total possible moves are (3) and 

#-position total possible moves are (4)

Let's solve the problem without Heuristic Search that is Uninformed Search or Blind Search ( Breadth First Search and Depth First Search)

Breath First Search to solve Eight puzzle problem



Note: If we solve this problem with depth first search, then it will go to depth instead of exploring layer wise nodes.

Time complexity: In worst case time complexity in BFS is O(b^d) know as order of b raise to power d.  In this particular case it is (3^20). 

b-branch factor

d-depth factor

Let's solve the problem with Heuristic Search that is Informed Search (A* , Best First Search (Greedy Search))

To solve the problem with Heuristic search or informed search we have to calculate Heuristic values of each node to calculate cost function. (f=g+h)

Initial state                                                                      Goal state

                                                               

Note: See the initial state and goal state carefully all values except (4,5 and 8) are at their respective places. so, the heuristic value for first node is 3.(Three values are misplaced to reach the goal). And let's take actual cost (g) according to depth.

