# Python Arcade Shooter Game

A space-themed arcade shooter game built with Python and the Arcade library. Battle waves of enemies that shoot back while dodging their attacks and managing your ammunition!

## Features

- **Dynamic Enemy AI**: Enemies move in patterns and shoot bullets that track the player
- **Ammo Management**: Limited ammunition system with reload mechanic (press R to reload)
- **Health System**: Visual health bar showing remaining lives
- **Score Tracking**: Track enemies eliminated and high scores
- **Scrolling Background**: Animated space background for immersive gameplay
- **Progressive Difficulty**: More enemies spawn as time progresses
- **Game Over Screen**: Displays time survived, enemies killed, and high score

## Requirements

- Python 3.6+
- Arcade library

## Installation

1. Clone this repository:
```bash
git clone https://github.com/victorialu0515/Python-arcade-shootergame.git
cd Python-arcade-shootergame
```

2. Install the required dependencies:
```bash
pip install arcade
```

## How to Play

Run the game with:
```bash
python "Have Enemies Shoot The Player 8.py"
```

### Controls

- **Mouse Movement**: Control your spaceship position
- **Mouse Click or Spacebar**: Shoot bullets (requires ammo)
- **Arrow Keys**: Alternative movement controls
  - ↑ Up Arrow: Move up
  - ↓ Down Arrow: Move down
  - ← Left Arrow: Move left
  - → Right Arrow: Move right
- **R Key**: Reload ammunition (resets to 10 bullets)

### Objective

- Survive as long as possible by avoiding enemy bullets
- Shoot down enemies to increase your score
- Manage your ammunition wisely - you only have 10 bullets before needing to reload
- You have 10 health points - game ends when all are lost

## Game Mechanics

### Player
- Start with 10 ammo
- Start with 10 health points
- Move speed: 10 units per frame
- Can reload at any time by pressing R

### Enemies
- Spawn randomly across the screen
- Move in a pattern bouncing off screen edges
- Face and track the player
- Shoot bullets aimed at the player every 30 frames
- Various enemy types with different appearances
- Speed: 2 units per frame

### Bullets
- Enemy bullets: Blue lasers that track player position
- Player bullets: Red lasers that shoot upward
- Speed: 4 units per frame
- Bullets disappear when leaving the screen

## Scoring

- Each enemy destroyed: +1 point
- Time survived is tracked in seconds
- High score is saved for the session

## Game Over

The game ends when you take 10 hits from enemy bullets. The game over screen shows:
- Total time survived
- Total enemies killed
- Session high score

Click to restart and try again!

## Notes

The game references some image files (`Instructions page-2.jpg`, `spacebg.jpg`, `doge.jpg copy.jpg`) that should be in the same directory as the Python file for full visual experience. If these files are missing, the game will still run but without custom backgrounds and instruction screens.

## License

This project is open source and available for educational purposes.
