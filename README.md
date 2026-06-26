# Pixel Runner

A 2D side-scrolling runner game built with Python and [Pygame](https://www.pygame.org/). Dodge snails and flying enemies, survive as long as possible, and beat your high score.

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pygame](https://img.shields.io/badge/Engine-Pygame-green)

## Gameplay

- Press **Space** to start the game
- Press **Space** or click the player to jump
- Avoid the snails and flying enemies
- Your score increases the longer you survive
- Colliding with an obstacle ends the run and shows your final score

## Features

- Sprite-based player animation (walk cycle and jump)
- Procedurally spawned obstacles (snails and flies) using `pygame.sprite.Group`
- Gravity and jump physics
- Real-time score tracking based on survival time
- Background music and jump sound effects
- Intro and game-over screens

## Built With

- **Python 3**
- **Pygame** – game loop, sprites, collision detection, audio

## Getting Started

### Prerequisites

- Python 3.10+
- pip

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/Gotetisid/Runner-Game.git
   cd Runner-Game
   ```

2. Install dependencies
   ```bash
   pip install pygame
   ```

3. Run the game
   ```bash
   python runner.py
   ```

## Project Structure

```
Runner-Game/
├── runner.py            # Game loop, player and obstacle classes, core logic
├── graphics/            # Sprite images (player, snail, fly, background)
├── audio/               # Sound effects and background music
└── font/                # Pixel font used for score and menu text
```

## What I Learned

This was my first project using a real game engine rather than a GUI framework. Building it helped me get hands-on with:

- Structuring a continuous game loop and managing game state (intro screen, active gameplay, game-over)
- Using `pygame.sprite.Sprite` and `Group` classes to manage and update multiple game objects efficiently
- Implementing simple physics (gravity, jump velocity) and collision detection
- Working with timed events (`pygame.USEREVENT`) to control animation and obstacle spawning independently of the frame rate
- Managing game assets (images, audio, fonts) and loading them efficiently

## License

This project is open source and available for anyone to use or modify.
