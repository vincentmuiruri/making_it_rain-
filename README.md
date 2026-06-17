# Making It Rain 🌧️

A simple animated rain effect built with Pygame. Blue streaks fall continuously down a black screen, recycling from the top once they reach the bottom — like a basic rain or Matrix-style particle effect.

## Requirements

- Python 3.x
- Pygame

Install Pygame if you don't already have it:

```bash
pip install pygame
```

## Running the Program

```bash
python rain.py
```

A 500x700 window will open showing the rain animation. Close the window to stop the program.

## How It Works

- 150 raindrops are created at start, each with a random starting position, fall speed (4-10 px/frame), and streak length (10-20 px).
- Every frame, each raindrop is drawn as a short blue line and moved downward by its speed.
- When a raindrop falls past the bottom of the screen, it resets to a random x position and reappears just above the top, so the rain never runs out and looks continuous.
- The animation runs at 60 frames per second.

## Customization Ideas

- Change `WIDTH` and `HEIGHT` to resize the window.
- Adjust the `range(150)` value to add or remove raindrops.
- Tweak the `speed` and `length` ranges for slower/faster or shorter/longer rain.
- Change the color tuple `(0, 0, 255)` in `pg.draw.line()` to make the rain a different color.
