# Object Counter by Color (OpenCV)

This Python script uses OpenCV and NumPy to detect and count objects of three different colors (blue, green, and red) in real time using your webcam. The program displays the number of detected objects for each color directly on the video feed, and highlights each detected object with contours and labels.

# Features

Real-time object detection for blue, green, and red colors.
Live object counting: The counter updates only for objects currently visible on the screen.
Contours and centers: Draws the contour and center of each detected object.
Color labels: Each detected object is labeled with its color.
Combined mask view: Shows a window with the combined mask of all detected colors.

# How to Use

Install dependencies (if you haven't already):

pip install opencv-python numpy

Run the script:

python contador_de_Objetos.py

Show objects of blue, green, or red color in front of your webcam. The program will:

Draw a contour and label for each detected object.
Display the current count of each color at the top left of the video window.
Exit the program by pressing the q key.

# Controls

q: Quit the program.

# Notes

The HSV color ranges for blue, green, and red are set in the script. You may need to adjust these values for your lighting conditions or camera.
Only objects with an area greater than 500 pixels are counted (to avoid noise).
The red color is only detected in the lower hue range (0-10). For better red detection, you can add a second range for high hue values (170-179).
Example Output
The main window (Frame) shows the camera feed with contours, centers, and color labels.
The Mask window shows the combined binary mask for all detected colors.
The top left of the frame displays the current count for each color, for example:

Red objects: 1
Green objects: 0
Blue objects: 2
