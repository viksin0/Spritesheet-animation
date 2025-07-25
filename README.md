# Sprite Sheet Animation Demo

A web-based sprite sheet animation player built with HTML, CSS, and JavaScript. This project demonstrates how to create smooth character animations using sprite sheets.

## Features

- **Interactive Animation Player**: Play, pause, and stop sprite animations
- **Multiple Animations**: Choose from 10 different character animations:
  - Idle
  - Run
  - Walk
  - Jump
  - Attack (3 variations)
  - Hurt
  - Dead
  - Shield
- **Speed Control**: Adjustable animation speed (50ms to 500ms per frame)
- **Frame Counter**: Real-time display of current frame and total frames
- **Responsive Design**: Dark theme with smooth transitions and hover effects

## Demo

Open `index.html` in your web browser to see the sprite sheet animation in action!

## Project Structure

```
├── index.html          # Main HTML file with animation interface
├── style.css           # All CSS styles for the demo and sprite positioning
├── spritesheet.png     # Character sprite sheet image
├── spritesheet.css     # Original sprite class definitions (legacy)
└── README.md           # Project documentation
```

## How It Works

1. **Sprite Sheet**: The character animations are stored in a single `spritesheet.png` file with each frame positioned in a grid
2. **CSS Background Positioning**: Each animation frame is displayed by adjusting the `background-position` CSS property
3. **JavaScript Animation**: A timer-based system cycles through frames to create smooth animations
4. **Frame Calculation**: The system calculates frame positions based on:
   - Frame width (128px) and height (128px)
   - Row position in the sprite sheet
   - Number of frames per animation

## Usage

1. Clone or download this repository
2. Open `index.html` in a web browser
3. Select an animation from the dropdown menu
4. Click "Play Animation" to start the animation
5. Adjust the speed slider to change animation speed
6. Use "Stop" to reset to the first frame

## Technical Details

- **Frame Size**: 128x128 pixels
- **Display Scale**: 1.5x for better visibility
- **Animation Speed**: Configurable from 50ms to 500ms per frame
- **Browser Compatibility**: Works in all modern browsers

## Customization

To add new animations or modify existing ones:

1. Update the `animations` object in the JavaScript code
2. Define the number of frames, row position, and starting X position
3. Ensure your sprite sheet follows the same 128x128 frame size

## License

This project is open source and available under the MIT License.
