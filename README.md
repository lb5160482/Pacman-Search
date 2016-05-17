# Pacman_Saerch-AI
Artificial Intelligence search algorithm base on Pacman  

Depth-First Search:  
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:  
python pacman.py -l tinyMaze -p SearchAgent  
python pacman.py -l mediumMaze -p SearchAgent  
python pacman.py -l bigMaze -z .5 -p SearchAgent  
python pacman.py -l openMaze -z .5 -p SearchAgent  

Breadth-First Search :  
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:  
python pacman.py -l tinyMaze -p SearchAgent -a fn=bfs  
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs  
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs  
python pacman.py -l openMaze -p SearchAgent -a fn=bfs  

Iterative Deepening Search:  
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:  
python pacman.py -l tinyMaze -p SearchAgent -a fn=ids  
python pacman.py -l mediumMaze -p SearchAgent -a fn=ids -z .5  
python pacman.py -l bigMaze -p SearchAgent -a fn=ids -z .5  
python pacman.py -l openMaze -p SearchAgent -a fn=ids -z .5  

A* Search:  
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:  
python pacman.py -l tinyMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic  
python pacman.py -l mediumMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic  
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic  
python pacman.py -l openMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic  

New Heuristic Function:  
By running the following 2 commands, we can see the solutions for tinyCorners and mediumCorners:  
python pacman.py -l tinyCorners -p AStarCornersAgent -z 0.5  
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5  

Eating all the dots problem with A* with a null heuristic function:  
In this question, we just need to let function foodHeuristic(state, problem) return 0 and test it. In this way, it is a null heuristic.  
python pacman.py -l testSearch -p AStarFoodSearchAgent  
python pacman.py -l trickySearch -p AStarFoodSearchAgent  

