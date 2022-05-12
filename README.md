#      SNAKE : "APPLE RIGHT AWAY!!!"
.
.
.
##  Member of Group
Nazhifah Elqolby 5025201156 - DAA (C)

Raden Pandu Anggono Rasyid 5025201024 - DAA (C)

Dawamul Fikri Aqil 5025201025 - DAA (C)]


## Description
We made Snake Game named "SNAKE : APPLE RIGHT AWAY!!!" by using BFS algorithm. The snake will use BFS algorithm to find the shortest path between its head and the apple (let's call it path_1). If path1 is not available, then go to step 4. Create a virtual snake identical to the original snake and make it follow path_1. After the virtual snake reaches the apple, check if the path between the virtual snake's head and its tail is available (let's call it path_2), if so, then make the original snake follow path_1. If path_1 or path_2 are not available, make the original snake follow its tail.


•	settings.py : contains game settings and global variables like width, height, etc..

•	snake.py : contains Snake and Square classes.

•	play.py : contains code for running the project.


## Algorythm

•	Find shortest path between (start_position, end_position)
![1](https://user-images.githubusercontent.com/94452616/168067962-4766d5a9-5ad9-40f7-b956-8b01cf96e083.jpg)

•	Starting from end node, we will find the parent node of each node 
![2](https://user-images.githubusercontent.com/94452616/168067968-69aa1adb-2eba-420e-9436-ae77b7340a3e.jpg)

•	Creates a copy of snake (same size, same position, etc)
![3](https://user-images.githubusercontent.com/94452616/168067974-21e4d052-ca4f-46db-b648-730e78ea9b0d.jpg)

•	If there is only 1 apple left for snake to win and it’s adjacent to head
![4](https://user-images.githubusercontent.com/94452616/168067982-94975fca-0593-4b89-878a-d90a4feca241.jpg)

•	Let the virtual snake check if path to apple is available
![5](https://user-images.githubusercontent.com/94452616/168067991-a35e4361-c358-46bb-a953-89ae587ddd03.jpg)

•	This will be the path to virtual snake tail after it follows path_1
![6](https://user-images.githubusercontent.com/94452616/168068154-80b4fc3c-a040-42f6-aa07-4097d916326c.jpg)

•	If there is a path between v_snake and it’s tail, choose BFS path to apple (fastest and shortest path)

![7](https://user-images.githubusercontent.com/94452616/168068005-a34f4b76-d355-49e8-be73-318a31472173.jpg)

•	If path_1 or path_2 not available, these 3 conditions:

  1. Make sure that the longest path to tail is available
![8](https://user-images.githubusercontent.com/94452616/168068022-0af8100f-8c0f-47fb-b773-280ffabd8c6f.png)
  
  2.	If score is even, choose longest_path_to_tail() to follow the tail,
![9](https://user-images.githubusercontent.com/94452616/168068074-ccb18faa-4b63-42a1-9b67-d6b0506b0260.png)

   if odd use any_safe_move()
![10](https://user-images.githubusercontent.com/94452616/168074545-4c854cf4-7294-49df-ad4c-2c4cb4d12723.png)

   if path to tail is available, choose shortest path to tail
![12](https://user-images.githubusercontent.com/94452616/168074560-2327e2d5-e0eb-4676-a37c-9bc5c38fdb8e.png)

  3.	Change the follow tail method if the snake gets stuck in a loop. Snake couldn’t find a path and will probably die
![11](https://user-images.githubusercontent.com/94452616/168068097-de35466f-2a53-4c37-b254-a6ef8aa24b3a.png)  

## Result
![gameplay](https://user-images.githubusercontent.com/38482276/87240274-cae19380-c420-11ea-8193-bddab2ef379d.gif)

To run the game, you can install python 3 and install these modules: pip install pygame and run play.py file.

### Reference
Hayderkahrrufa, geeksforgeeks, stackoverflow
