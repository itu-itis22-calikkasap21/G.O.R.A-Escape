

# G.O.R.A Maze Game

This project is a text-based maze game where the player (`P`) has to navigate through a maze, collect points (`@`), and reach the exit (`E`) within a certain time limit. If the player hits a wall (`#`), they lose points and are returned to their original position. The game consists of multiple levels and a leaderboard, which displays the top scores.

## Key Features

1. **Maze Generation**: Random mazes are generated for each level using a depth-first search algorithm.

2. **Player Movement**: The player can move up, down, left, and right within the maze using the `w`, `s`, `a`, and `d` keys, respectively.

3. **Scoring System**: Players receive points for collecting items within the maze. Hitting a wall results in a penalty.

4. **Multi-Level Gameplay**: The game consists of multiple levels, each with a unique maze and a 60-second time limit.

5. **Leaderboard**: The leaderboard keeps track of the scores for each player. The score is cumulative over the levels and is saved to a JSON file.

## Code Structure

### Libraries

The game uses standard Python libraries such as `time`, `random`, `json`, and `os`.

### Player Class

The `Player` class represents the player within the maze. The player has a position (x, y) and a score. The `move` method allows the player to move in a specified direction.

### Level Class

The `Level` class represents a level within the game. Each level has a maze, start point, and end point.

### Functions

The game includes several functions to manage the game process:

- `clear`: Clears the terminal screen.
- `get_username`: Asks the user for their username and displays the game instructions.
- `save_score`: Saves the player's score to a JSON file.
- `print_leaderboard`: Prints the leaderboard, reading the scores from the JSON file.
- `generate_maze`: Generates a random maze.
- `generate_levels`: Generates multiple random levels.
- `find_start_and_end`: Finds the start and end points of a maze.
- `main`: Contains the main game loop.

### Running the Game

To run the game, call the `main` function. The function will generate the levels, create a player, and manage the gameplay and scoring.

## How to Play

When you start the game, you are asked to enter your username. Once you've entered your username, you can start playing the game. Use the `w`, `s`, `a`, and `d` keys to move the player up, down, left, and right, respectively. Try to collect as many points as possible and reach the exit within the time limit to maximize your score. Be careful not to hit the walls, as you will lose points and return to your starting position. Good luck!

## Future Enhancements

While this game is fully functional, there are a few potential enhancements that could make it even better:

- Adding more varied maze generation algorithms.
- Including different types of obstacles or power-ups within the maze.
- Implementing an improved leaderboard that includes dates and times of the scores.
