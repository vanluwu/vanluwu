# Turtle Runaway Game Explanation

This Python program implements a "Turtle Runaway" game using the `turtle` and `tkinter` libraries. In this game, one turtle (the chaser) is controlled by the player, while another turtle (the runner) is controlled by the computer (AI). The goal is for the chaser to catch the runner within a time limit.

## Code Structure

### 1. `RunawayGame` Class
This is the main class that handles the game logic, such as initializing the game, tracking the score, and determining if the runner has been caught.

#### Attributes:
- **`canvas`**: The drawing area where the turtles move.
- **`runner`**: The turtle that tries to run away (controlled by AI).
- **`chaser`**: The turtle that tries to catch the runner (controlled by the player).
- **`catch_radius2`**: The square of the distance within which the chaser catches the runner.
- **`start_time`**: Records the time when the game starts.
- **`score`**: Tracks the score of the player.
- **`time_limit`**: Time limit for the game (default is 30 seconds).
- **`game_active`**: Boolean flag to indicate if the game is running.

#### Methods:
- **`__init__(self, canvas, runner, chaser, catch_radius=50, time_limit=30)`**: Initializes the game objects, sets up turtles' appearance, and prepares the score and time tracking.
- **`is_catched(self)`**: Checks if the chaser is within a certain distance from the runner.
- **`start(self, init_dist=400, ai_timer_msec=100)`**: Starts the game, placing the turtles at opposite sides and setting a timer for the AI's movements.
- **`step(self)`**: A looped function that updates the positions of the turtles, checks if the game is over, and updates the score.
- **`end_game(self)`**: Ends the game when the runner is caught or time runs out, displaying the final score.
- **`update_score(self)`**: Updates the score based on the elapsed time. The score decreases as time progresses.

### 2. `ManualMover` Class
This class represents the turtle controlled by the player. The player moves the turtle using the keyboard's arrow keys (`Up`, `Down`, `Left`, `Right`).

#### Attributes:
- **`step_move`**: The number of pixels the turtle moves forward or backward.
- **`step_turn`**: The degree by which the turtle turns left or right.

#### Methods:
- **`run_ai(self, opp_pos, opp_heading)`**: A placeholder method since the player manually controls the turtle (no AI logic needed).

### 3. `RandomMover` Class
This class represents the turtle controlled by the AI. The AI moves randomly, either moving forward or turning left or right.

#### Methods:
- **`run_ai(self, opp_pos, opp_heading)`**: Implements basic AI logic where the turtle randomly decides to move forward, turn left, or turn right.

### 4. Main Program
The program starts by creating a `tkinter` window (`root`) and a `Canvas` widget for the game area. The `TurtleScreen` is initialized to display the turtles. The runner is controlled by the `RandomMover` class (AI), and the chaser is controlled by the `ManualMover` class (player).

The game is started by creating an instance of the `RunawayGame` class and calling the `start()` method. The game loop continues until the runner is caught or time runs out.

### Controls:
- **Up Arrow**: Move forward.
- **Down Arrow**: Move backward.
- **Left Arrow**: Turn left.
- **Right Arrow**: Turn right.

## Gameplay Rules
- The player controls the chaser turtle, while the runner turtle is controlled by AI.
- The runner moves faster than the chaser to increase the game's difficulty.
- The highest possible score is 300 points.
- The faster the player catches the runner, the higher the score.
- If the player fails to catch the runner within 30 seconds, they lose the game.

## How the Game Works
- The runner turtle moves randomly using a simple AI logic.
- The chaser turtle is controlled by the player using the arrow keys.
- The player must try to catch the runner within the specified time limit (30 seconds).
- The score is calculated based on how quickly the player catches the runner, starting from a maximum score of 300 and decreasing over time.

## End of Game
- The game ends when either the runner is caught or the time limit is reached.
- The final score and elapsed time are displayed on the canvas.

## Libraries Used
- **`turtle`**: Provides the graphics and movement for the turtles.
- **`tkinter`**: Used to create the graphical window and handle keyboard events.
