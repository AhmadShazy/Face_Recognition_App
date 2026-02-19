🎯 AI Face Recognition System

A Python-based Face Recognition System built using OpenCV’s LBPH algorithm for real-time face detection and identification.
The system supports custom dataset training and configurable recognition thresholds, making it suitable for academic and experimental AI applications.

📌 Overview

This project implements a complete face recognition pipeline:

Face detection using OpenCV

Face recognition using LBPH (Local Binary Patterns Histogram)

Custom dataset training

Threshold-based identity validation

Optional MySQL integration for storing user data

The system is designed for educational and practical implementation of computer vision concepts.

🛠 Technologies Used

Python 3.13

OpenCV (opencv-contrib-python)

NumPy

Pillow

MySQL Connector

📦 Installation

Install required dependencies:

& C:/Python313/python.exe -m pip install pillow numpy opencv-contrib-python mysql-connector-python

📁 Dataset Format

The training ID is extracted from the second dot-separated token in the filename.

Required naming format:

anything.<id>.anything.jpg


Examples:

user.1.sample1.jpg
person.2.001.png


Files not following this pattern are skipped during training.

🎓 Training Recommendations

For improved recognition accuracy:

Use 30–50 images per person

Include variations in:

Lighting

Facial expressions

Angles

Keep faces centered and clearly visible

Avoid strong backlighting or heavy shadows

🎯 Recognition Threshold

The system uses LBPH distance for matching.

Lower distance indicates better match

Default threshold: ≤ 75

Threshold can be adjusted in face_recognition.py

If valid matches are slightly above the threshold, increase it to 80–90 as needed.

▶ Running the Project
& C:/Python313/python.exe "path_to_project/main.py"


Example:

& C:/Python313/python.exe "e:/Your_Project_Path/main.py"

📚 Project Type

Academic AI / Computer Vision Project
Developed as part of coursework to demonstrate practical implementation of face recognition systems.
