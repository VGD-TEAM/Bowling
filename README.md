# Bowling Game Project

This repository contains the code for a bowling game implemented in Unity. The game features realistic pin behavior, collision detection, and a controllable bowling ball. Players aim to knock down all the pins to complete the level.
# itcho link
https://ibrahim3999.itch.io/bowling
## Features
- **Pin System**: Detects when pins fall and keeps track of the number of fallen pins.
- **Level Management**: Automatically progresses to the next level when all pins are knocked down.
- **Bowling Ball Control**: Players can control the ball using keyboard inputs.
- **Collision Detection**: Handles interactions between pins and the bowling ball, as well as pin-to-pin collisions.

## Code Overview

### GameManager.cs
- Manages the overall game state.
- Tracks fallen pins and checks if the level is complete.
- Loads the next level when all pins are knocked down.

### Pin.cs
- Handles individual pin behavior.
- Notifies the `GameManager` when a pin falls due to a collision.

### PinCollision.cs
- Handles advanced collision logic between pins and the bowling ball.
- Ensures pins only register as fallen once.

### BowlingBallController.cs
- Controls the movement of the bowling ball.
- Uses `Rigidbody` physics for realistic movement.

## How to Play
1. Control the bowling ball using the arrow keys or `WASD` to move.
2. Aim and hit the pins to knock them down.
3. Progress to the next level when all pins are down.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ibrhaim3999/Bowling.git
   ```
2. Open the project in Unity.
3. Ensure all required assets and dependencies are imported.
4. Press the play button in the Unity Editor to start the game.

## File Structure
- **Assets/**: Contains all the Unity assets, scripts, and prefabs.
  - **Scripts/**: Contains the game scripts listed above.
- **Scenes/**: Contains the game levels (e.g., Level1, Level2).

## Tags Used in the Game
- **Pins**: Tag assigned to pin objects for collision detection.
- **BowlingBall**: Tag assigned to the bowling ball object.

## Known Issues
- The pin detection logic might trigger multiple notifications for the same pin in certain scenarios. Future updates will refine this behavior.
- Ensure the game is played on a flat surface for consistent pin physics.

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or bug reports.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For any inquiries or feedback, please contact [your email/contact info].
