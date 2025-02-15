# Air-Canvas

Air Canvas is an interactive application that allows users to draw on a virtual canvas using a colored marker or object with distinctive color. The app uses OpenCV for real-time color detection, enabling users to create drawings in mid-air.

## Features
- Draw using a colored marker tracked via webcam.
- Switch colors or clear the canvas with gestures.
- Adjustable HSV range for precise color detection.
- Real-time drawing displayed in a separate window.

## Requirements
- Python 3.11.4
- OpenCV
- Numpy
- Deque (from collections)

## Working
The webcam captures frames, tracks a specific color in HSV space, and detects movements for drawing. Users can select colors or clear the canvas through specific gestures, and the drawing is continuously updated on the canvas. Press 'q' to exit.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/SoubhLance/Air-Canvas.git
2. Install dependencies:
   ```bash
   pip install opencv-python numpy


## Usage
```bash
python air_canvas.py
```
## Contribution
Feel free to contribute by submitting issues or suggesting features!

## License
```css
This README provides a clear overview and instructions for the project. Feel free to adjust it as necessary!
```


