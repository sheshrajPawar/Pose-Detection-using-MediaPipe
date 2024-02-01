# Pose-Detection-using-MediaPipe
This repository contains a Python script for pose detection using the MediaPipe library. Pose detection involves identifying key points on a person's body, such as the nose, shoulders, elbows, and knees. The script processes static images and provides real-time pose detection through a webcam.

# 1. Introduction:
The GitHub repository hosts a Python script for pose detection using the MediaPipe library. Pose detection involves recognizing and tracking key points on the human body, providing insights into body posture and movements.

# 2. Dependencies:
The code relies on OpenCV (cv2), MediaPipe (mediapipe), and NumPy (numpy).
OpenCV is used for image processing, MediaPipe facilitates pose detection, and NumPy is employed for array manipulation.

# 3. Static Image Processing:
a. Image Loading:
The script begins by loading a set of static images specified in the IMAGE_FILES list.
b. Pose Detection:
Utilizes the mp_pose.Pose class in static image mode, with model complexity set to 2 for increased accuracy.
Segmentation is enabled to distinguish the detected pose from the background.
c. Nose Coordinates:
The code prints the coordinates of the nose landmark on each processed image.
d. Annotation and Segmentation:
Generates annotated images with drawn pose landmarks.
Enhances segmentation by adding a background of a specified color (gray).
e. Result Saving:
Annotated images are saved in the /tmp/ directory for further analysis and visualization.

# 4. Webcam Input:
a. Webcam Initialization:
The script sets up the default camera using OpenCV's cv2.VideoCapture.
b. Real-time Pose Detection:
Utilizes the mp_pose.Pose class to continuously process video frames from the webcam.
Annotates the live camera feed with pose landmarks in real-time.
c. Display and Exit:
Displays the annotated frames in a window named "MediaPipe Pose."
The application runs until the 'Esc' key is pressed, allowing for a smooth exit from the webcam mode.

# 5. Usage Instructions:
Users can easily integrate the script into their projects for applications such as fitness tracking, gesture recognition, or augmented reality.

# 6. Results and Screenshots:
Annotated images from static image processing and screenshots from webcam-based pose detection are available in the /tmp/ directory.

# 7. License:
The project is open-source and licensed under the MIT License.
