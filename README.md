# Air-Canvas


Air Canvas is an interactive application that allows users to draw on a virtual canvas using a colored marker or any object with a distinctive color. The application utilizes computer vision techniques to detect the colored object and track its movement, enabling the user to draw in the air. This project is a fun way to explore the basics of image processing and computer vision using Python and OpenCV.


## Features

- Draw on a virtual canvas using a colored marker.
- Change drawing colors with a simple gesture.
- Clear the canvas with a specific gesture.
- Adjustable HSV color range for precise marker detection.
- Real-time drawing on the canvas displayed in a separate window.

## Requirements

- Python 3 {3.11.4 is used here specifically}
- OpenCV
- Numpy
- Deque

## Working
The Air Canvas code is an interactive drawing application that allows users to draw in the air using a colored marker tracked by a webcam. Using OpenCV, the program creates trackbars to adjust the HSV (Hue, Saturation, Value) values, defining the marker's color range. It employs four deque objects to store drawing points for blue, green, red, and yellow markers. The on-screen interface lets users select these colors or clear the canvas.

The canvas starts as a white window with color selection and clear buttons. The webcam captures frames, flips them, and converts them to HSV color space. A mask is created to detect the marker within the specified HSV range, followed by morphological operations to clean up the mask. Contours are identified to locate the marker's position. If the marker is detected within the button area, it triggers the corresponding action (color change or clear). Otherwise, the marker's position is recorded, and lines are drawn on the frame and canvas based on the selected color. The application runs in a loop, updating the drawings in real-time until the user exits by pressing 'q'.
