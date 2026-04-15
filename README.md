# PredictiveCarSafety
An AI-powered safety system designed to predict potential road hazards and collision risks using real-time video processing. This project was developed and tested within a Google Colab environment.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/b70688cb-946e-4a20-8376-1d6583d86a87" />

## Project Overview
This project implements a computer vision pipeline that analyzes vehicle dashcam footage to enhance driver safety. By identifying objects and calculating spatial relationships, the system provides a predictive layer to prevent accidents before they occur.

### Key Features
Object Detection: Real-time identification of vehicles, pedestrians, and traffic signs.

Distance Estimation: Calculates the relative distance of objects in the frame.

Predictive Alert Logic: Triggers safety warnings based on "Time-to-Collision" (TTC) metrics.

Visual Overlays: Dynamic UI that highlights high-risk zones for the driver.

### Tech Stack
Environment: Google Colab

Language: Python

Libraries: OpenCV (Image processing), TensorFlow/PyTorch (Model Inference), NumPy (Calculations), Matplotlib (Visualization).

### Methodology
Frame Extraction: Processing raw video input at 30 FPS.

Detection Layer: Utilizing a pre-trained model (e.g., YOLO or SSD) to extract bounding boxes.

Heuristic Risk Assessment: Analyzing the rate of change in bounding box size to estimate closing speed.

Output Generation: Exporting a processed video with safety annotations.
