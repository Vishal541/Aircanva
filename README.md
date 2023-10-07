# Air Canvas Project

## Introduction

The Air Canvas project is a computer vision-based implementation using OpenCV that allows you to draw in the air by simply waving a colored marker. This project is designed to capture the motion of a colored marker using a camera and draw anything on a digital canvas. The colored object at the tip of your finger serves as the marker.

We will be using OpenCV's computer vision techniques to build this project. While the preferred language for this project is Python due to its extensive libraries and user-friendly syntax, the basic concepts can be implemented in any OpenCV-supported programming language.

The key technique used in this project is color detection and tracking. The colored marker is detected, and a mask is created to isolate it. This mask undergoes further processing through morphological operations, including erosion and dilation. Erosion reduces impurities in the mask, while dilation restores the eroded main mask.

## Algorithm

Here's a step-by-step breakdown of the algorithm used in the Air Canvas project:

1. Start by capturing frames from the camera and convert them to the HSV color space. HSV is preferred for color detection.

2. Prepare the canvas frame and add the necessary ink buttons to it.

3. Adjust the trackbar values to find the mask of the colored marker.

4. Preprocess the mask using morphological operations such as erosion and dilation.

5. Detect contours in the processed mask, find the center coordinates of the largest contour, and store them in an array for successive frames. These arrays will be used for drawing points on the canvas.

6. Finally, draw the points stored in the array on the frames and canvas.

## Requirements

To run the Air Canvas project, you will need the following:

- Python 3
- NumPy
- OpenCV installed on your system

## Creator

This Air Canvas project was created by Vishal. If you have any questions or would like to learn more about this project, you can reach out to the creator for further information and assistance.
