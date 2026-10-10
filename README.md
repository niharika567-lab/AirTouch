# AirTouch# AirTouch: Touchless Mouse Control

## Introduction

AirTouch is a computer vision project that allows users to control a computer mouse using hand gestures in front of a webcam. It uses Python, OpenCV, and MediaPipe to detect hand movements and perform mouse actions without touching a mouse.

The system supports cursor movement, left-click, right-click, double-click, drag and drop, scrolling, and pause control. It uses gesture detection and error prevention techniques to make mouse control smooth and reliable.

## Features

- **Hand Tracking:** Detects hand movements in real time using a webcam.
- **Cursor Movement:** Moves the mouse cursor according to the index finger.
- **Left Click:** Brings the thumb and index finger together to perform a left-click.
- **Right Click:** Uses the two-finger peace sign to perform a right-click.
- **Double Click:** Uses three extended fingers to perform a double-click.
- **Drag and Drop:** Uses pinch and fist gestures to select and move items.
- **Scrolling:** Scrolls pages by moving the index finger up or down.
- **Pause Control:** Shows an open palm to pause mouse control.
- **Idle Mode:** Uses a closed fist as a neutral position.
- **Gesture Accuracy:** Uses multiple-frame checking to reduce accidental clicks.
- **Safety Protection:** Prevents mouse actions on the AirTouch camera window.
- **Live Display:** Shows hand tracking, active gestures, and action notifications on the screen.

## Gesture Controls

| Hand Gesture | Mouse Action |
|---|---|
| Index finger extended | Move cursor and scroll |
| Thumb and index finger pinched | Left-click |
| Two fingers extended | Right-click |
| Three fingers extended | Double-click |
| Pinch, then close the hand into a fist | Drag and drop |
| Open palm | Pause control |
| Closed fist | Idle mode |

## Technologies Used

- **Python:** Main programming language.
- **OpenCV:** Captures webcam video and displays the camera window.
- **MediaPipe:** Detects the hand and its 21 landmarks.
- **NumPy:** Performs distance calculations and coordinate processing.
- **PyAutoGUI:** Controls mouse movement, clicks, dragging, and scrolling.

## How It Works

1. The webcam captures live video.
2. OpenCV processes the video frames.
3. MediaPipe detects the hand and its landmarks.
4. The system identifies the fingers and recognizes the gesture.
5. The gesture control system checks the action and prevents accidental clicks.
6. PyAutoGUI performs the required mouse action.
7. The cursor or screen responds to the hand movement.

## Gesture Accuracy and Safety

AirTouch uses several methods to improve accuracy:

- Checks gestures across multiple frames before performing an action.
- Prevents repeated clicks when a gesture is held.
- Uses cooldowns to avoid unwanted repeated actions.
- Prevents accidental actions while changing between gestures.
- Reduces unwanted scrolling caused by small hand movements.
- Blocks clicks and scrolling when the cursor is over the AirTouch camera window.

## Installation

1. Download or clone the project repository.
2. Create a Python virtual environment.
3. Activate the virtual environment.
4. Install the required libraries using `requirements.txt`.
5. Run the `main.py` file to start the application.

## Testing

AirTouch includes automated tests to check gesture detection and prevent conflicts between mouse actions.

The tests verify cursor gesture classification, left-click, right-click, double-click, drag and drop, and protection against repeated or accidental actions.

## Future Enhancements

- Add more customizable hand gestures.
- Allow users to adjust cursor speed and sensitivity.
- Add keyboard shortcut controls.
- Support two-hand control.
- Create different gesture settings for different applications.

## Conclusion

AirTouch provides a simple and touch-free way to control a computer using hand gestures. By combining computer vision, hand tracking, and mouse automation, it offers a useful alternative to a traditional mouse and can improve accessibility and convenience for users.
