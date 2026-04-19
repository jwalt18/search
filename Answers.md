to run game: /usr/bin/python3 pacman.py -t -p GreedyAgent

Question 1
Spent a while trying to get the game to run, eventually got it to run as text (ASCII) mode. Once I got it to run, I gave the AI the instructions for question 1 as well as the files it should edit and should view and ran it. It solved tinyMaze(cost 10) and mediumMaze(cost 130, nodes 146) with that, but needed additional prompting to also solve bigMaze(cost 210, nodes 390). The order was about what I expected from DFS, and pacman doesn't go to each explored square since it isn't the most optimal stratagy.

Question 2
With BFS implemented and testing just for medium and big maze which while mediumMaze(cost 68, nodes 269) had a lower cost it expanded much more nodes and bigMaze(cost 210, nodes 620) was just worse overall.

Question 3
UCS was implemented and mediumMaze(cost 68, nodes 269) performed the same as BFS. The mediumDottedMaze(cost 1, nodes 186) using the stay east search agent had a low cost as expected although expanded far too many nodes comparitively. The mediumScaryMaze(cost 68719479864, nodes 108) had a high cost as expected due to bias.

Question 4
A* was implemented and in bigMaze A*(cost 210, nodes 549) and UCS(cost 210, nodes 620) A* was better at predicted levels. On openMaze DFS(cost 298, nodes 576), BFS(cost 54, nodes 682), UCS(cost 54, nodes 682), and A*(cost 54, nodes 535). DFS did quite badly, BFS and UCS are identicle and found the seemingly best strategy, and A* was most optimal due to the heuristic.

Question 5
