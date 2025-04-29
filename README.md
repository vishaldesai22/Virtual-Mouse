# Virtual-Mouse
# 🖐️ Virtual Mouse Controller using Hand Tracking

This project enables you to control your computer mouse using hand gestures captured via a webcam. It uses **MediaPipe** and **OpenCV** for real-time hand tracking and maps gestures to mouse functions such as move, click, scroll, and drag.

## 📁 Project Structure

- `HandTracking.py`: A reusable module for detecting and tracking hand landmarks, determining finger states, and measuring distances.
- `newMouse.py`: The main application that uses the hand tracker to control mouse input through gesture recognition.

---

## 🛠️ Requirements

Install the dependencies using pip:

```bash
pip install opencv-python mediapipe numpy autopy pyautogui

▶️ How to Run
Make sure both HandTracking.py and newMouse.py are in the same directory. Then run:

bash
Copy
Edit
python newMouse.py
A window will open displaying your webcam feed. Move your hand into the frame and use the gestures described below to control your mouse.

✋ Gesture Controls

Gesture	Action
Index finger up	Move cursor
Index + Middle up (close)	Left click
Thumb + Middle up	Right click
Pinky up (others down)	Drag
Thumb up	Scroll down
Index up	Scroll up
📦 Features
Hand detection using MediaPipe

21 landmark-based finger tracking

Smooth and accurate mouse control

Scroll and drag support via gestures

Customizable frame and smoothing parameters

📸 Preview
(Insert a GIF or screenshot here of the virtual mouse in action)

📌 Notes
Ensure good lighting for accurate detection.

The webcam index can be adjusted in the code (cv2.VideoCapture(0)).

Works best on screens with a standard resolution.

🧠 Credits
MediaPipe by Google

AutoPy for mouse control

PyAutoGUI for scrolling

