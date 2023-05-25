# G.O.R.A Maze Game

This project is a game simulating a player navigating through a series of maze levels. The main components and functions are as follows:

clear: This function clears the screen each time the game redraws. It uses the 'system' function from the 'os' module and runs the 'cls' command on Windows.

Player class: This class represents the state of the player. It stores the player's x, y position and total score. It has a 'move' function that allows the player to move.

Level class: This class represents each maze level. It stores a maze map, and start and end points.

get_username: This function takes the name of the user, who is the person playing the game.

save_score: This function saves a player's score to a 'scores.json' file. It uses the 'json' module.

print_leaderboard: This function reads the 'scores.json' file and sorts the players by score, with those with the highest scores at the top.

generate_maze: This function generates a maze. It uses a walk algorithm to create the maze, and then returns a text representation of the maze.

generate_levels: This function generates a certain number of maze levels. For each one, it generates a maze and finds the start and end points.

find_start_and_end: This function finds the start and end points of a maze.

main: This function runs the main loop of the game. It gets the player's name, generates the maze levels, and for each one, simulates the player trying to exit the maze. It takes the player's moves as input and tries to move them in the maze. When the player reaches the exit or time runs out, it saves the player's score and prints the leaderboard.

The game takes as input from the user which direction they want to move to exit the maze. The player can use the 'w' (up), 'a' (left), 's' (down), and 'd' (right) keys to try to navigate out of the maze and collect as many points as possible. They have a total of 60 seconds per level. The player receives points for completing each level, and the points are ultimately saved to a file called 'scores.json'. This file is used to create a leaderboard.
