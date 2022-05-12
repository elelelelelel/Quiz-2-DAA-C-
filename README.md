#      SNAKE : "APPLE RIGHT AWAY!!!"
.
.
.
##  Member of Group
Nazhifah Elqolby 5025201156 - DAA (C)

Raden Pandu Anggono Rasyid 5025201024 - DAA (C)


## Description
We made Snake Game named "SNAKE : APPLE RIGHT AWAY!!!" by using BFS algorithm. The snake will use BFS algorithm to find the shortest path between its head and the apple (let's call it path_1). If path1 is not available, then go to step 4. Create a virtual snake identical to the original snake and make it follow path_1. After the virtual snake reaches the apple, check if the path between the virtual snake's head and its tail is available (let's call it path_2), if so, then make the original snake follow path_1. If path_1 or path_2 are not available, make the original snake follow its tail.

•	settings.py : contains game settings and global variables like width, height, etc..

•	snake.py : contains Snake and Square classes.

•	play.py : contains code for running the project.


To run the game, you can install python 3 and install these modules: pip install pygame and run play.py file.


## Result
![gameplay](https://user-images.githubusercontent.com/38482276/87240274-cae19380-c420-11ea-8193-bddab2ef379d.gif)


### Reference
Hayderkahrrufa, geeksforgeeks, stackoverflow
