# <h1 align="center">😎GESTURE TUNE (SMART VOLUME CONTROL SYSTEM) 😎</h1>


.
## ⭐Project Overview:
GestureTune is an interactive program that lets users control their system’s volume using hand gestures. By tracking the positions of your index finger and thumb, this tool detects gestures and automatically raises or lowers the volume based on finger distance.

## ⭐How It Works:
1. The system accesses your webcam to capture real-time video.
2. It uses MediaPipe to recognize and track the hand movements, particularly focusing on the index finger and thumb.
3. If the distance between your index finger and thumb is greater than a specific threshold (50 pixels), the system increases the volume.
4. If the distance is less than or equal to 50 pixels, the system decreases the volume.
5. This continuous loop allows users to control volume seamlessly, without needing to press any physical keys.

## ⭐Technologies Used:
1. Python: Programming language for implementing the code.
2. OpenCV: For capturing and processing video input from the webcam.
3. MediaPipe: For real-time hand-tracking and detecting hand landmarks.
4. PyAutoGUI: To simulate the "volume up" and "volume down" key presses.

## ⭐Getting Started:

### 1. Prerequisites:
Make sure you have Python and the following packages installed:
pip install opencv-python
pip install mediapipe
pip install pyautogui

### 2. Running the Program:
To start the program, simply run:
python smart_volume_control.py

The program will open a window showing the live webcam feed with drawn landmarks on your hand. Move your thumb and index finger to adjust the volume.

### 3. Exiting the Program:
To stop the program, press the Esc key.

## ⭐Code Structure:
1. Video Capture: Uses OpenCV to capture real-time video from the webcam.
2. Hand Detection: MediaPipe detects hand landmarks and locates the index finger and thumb.
3. Distance Calculation: Calculates the distance between the index finger and thumb. Depending on this distance, it triggers a volume increase or decrease.
4. UI Feedback: Visual indicators (circles) are drawn on the index finger and thumb to show the tracked landmarks and a line connecting them.

⭐Planned Improvements:
1.  Volume Sensitivity: Add options to fine-tune the distance threshold for different volume levels.
2. On-Screen Volume Indicator: Display the current volume level on the screen for better feedback.
3. Gesture Customization: Enable users to define custom gestures for mute/unmute or specific volume levels.
4. Multi-Hand Support: Allow the use of both hands to control additional features.
