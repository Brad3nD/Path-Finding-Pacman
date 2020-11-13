# Path-Finding-Pacman
Using BFS, DFS, A*, and UCS to find a path for pacman on various maps and in certain problems.

Acknowledgement: The base code is borrowed from the Introduction of AI course of the University of California, Berkeley.

Create a virtual environment using python2.7
Commands to test out each function:

DFS
python pacman.py -l tinyMaze -p SearchAgent -a fn=dfs
python pacman.py -l mediumMaze -p SearchAgent -a fn=dfs
python pacman.py -l bigMaze -p SearchAgent -a fn=dfs

BFS
python pacman.py -l tinyMaze -p SearchAgent -a fn=bfs
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs

UCS
python pacman.py -l tinyMaze -p SearchAgent -a fn=ucs
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
python pacman.py -l bigMaze -p SearchAgent -a fn=ucs

A*
python pacman.py -l tinyMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
python pacman.py -l mediumMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
python pacman.py -l bigMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic

Finding all Corners Problem
python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem

Corners Heuristic
python pacman.py -l mediumCorners -p SearchAgent -a \
 fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic

Food Heuristic
python pacman.py -l trickySearch -p SearchAgent \
 -a fn=astar,prob=FoodSearchProblem,heuristic=foodHeuristic

Closest Dot Search
python pacman.py -l bigSearch -p ClosestDotSearchAgent -z .5 
