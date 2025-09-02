## Lane Line Detection 🚗🛣️
-----------------------------
## 📌 Project Overview
-----------------------------
This project implements Lane Line Detection using image processing techniques in Python.
The goal is to detect lane lines in road images or video frames using OpenCV and NumPy.
It applies filtering, edge detection, and region masking to highlight lane boundaries for self-driving car applications.

## 📂 Dataset
-------------------------------
- The project uses test images (e.g., solidWhiteRight.jpg) located in a folder like: /content/test_image/
- You can replace this with your own road/lane images.

## ⚙️ Requirements
--------------------------------
Make sure you have the following installed:
- python 3.x
- numpy
- pandas
- matplotlib
- opencv-python


## Install dependencies with:
pip install numpy pandas matplotlib opencv-python

## 🛠️ Methodology
--------------------------------------
The pipeline follows these main steps:

1. Import Libraries
- NumPy, Pandas, Matplotlib, and OpenCV.

2. Read Input Image
- Load road/lane images using matplotlib.image.

3. Preprocessing
- Convert the image to grayscale.
- Apply Gaussian Blur to reduce noise.

4. Edge Detection
- Use the Canny Edge Detector to find edges.

5. Region of Interest
- Mask the area of the image where lanes are expected (triangular region ahead of car).

6. Hough Transform
- Detect straight lines corresponding to lanes.

7. Overlay Results
- Draw the detected lane lines on the original image.
