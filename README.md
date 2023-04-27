# HU-Navigator
A Python Program that uses Dijkstra Algorithm to compute the shortest distance between university classrooms. 
1) Run the first cell – it makes the graph for each level.
2) Run the second cell – it creates the level-wise nested dictionary.
3) Run the third cell consisting of the Dijkstra algorithm. It takes 3 parameters: single level dictionary, start_point, destination. First while loops calculates the cost and updates the dictionary. Second while loop creates a string of nodes. The code following that breaks the string up into a proper list so it can be worked with. 
4) Run landmarks function. It takes one parameter (a node) and return the landmark associated with it. 
5) Run print_path. It takes two parameters: a list containing the nodes of shortest path, flag. Flag will be either multi or same level. If it is same, no node will be printed as (“Take the” node). If it is multi-level, you have to take the stairs or lifts so the first node will be printed as (“Take the” node). Final_route is a list that prevents repetition. 
6) Run shortest_path. It takes 3 parameters: start_point, destination, level_wise. If start_point and destination are on the same level, the first condition runs and path is returned. Otherwise, the nearest connecting nodes (stairs, lifts etc.) from start point are found. Then Dijkstra is called on each of these connecting nodes till destination. The path with the shortest distance is passed on to print_paths.
