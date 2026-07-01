# Optical_tracking
It is a complete Autonomous Optical Rocket Tracking System. 
Since this is your **first ISRO internship task**, your GitHub README should be clean, professional, and easy for your mentor or teammates to follow.

---

# README.md

````md
# 🚀 Optical Rocket Detection using YOLO

## Overview

This project is developed as part of my internship project on **Optical Tracking**.

The objective of this module is to detect rockets in images using a pretrained YOLO model. The detected rocket is highlighted with bounding boxes, forming the first stage of an autonomous optical tracking system.

This repository currently supports **image-based rocket detection**. Video tracking and advanced tracking modules will be integrated in future phases.

---

## Features

- Rocket detection using a pretrained YOLO model
- Detects rockets in uploaded images
- Displays bounding boxes with confidence scores
- Supports Google Colab execution
- Foundation for future video tracking and optical tracking pipeline

---

## Project Structure

```
.
├── detect.py                 # Main detection script
├── hybrid_detector.py        # YOLO detection module
├── domain_validator.py       # Filters false detections
├── tracker.py                # Tracking module
├── control_system.py         # Camera/gimbal control
├── rocket_yolo.pt            # Trained YOLO model
├── sample_images/            # Test images
└── README.md
```

---

## Requirements

Python 3.10+

Install the required libraries:

```bash
pip install ultralytics
pip install opencv-python
pip install sahi
pip install numpy
pip install matplotlib
```

Or install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/rocket-detection.git
cd rocket-detection
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Open the notebook in **Google Colab** or **Jupyter Notebook**.

Upload an input image when prompted.

The model will detect the rocket and display the output image with bounding boxes.

---

## Workflow

```
Input Image
      │
      ▼
YOLO Detection
      │
      ▼
Domain Validation
      │
      ▼
Bounding Box Generation
      │
      ▼
Output Image
```

---

## Technologies Used

- Python
- YOLO
- OpenCV
- SAHI
- NumPy
- Google Colab

---

## Future Work

- Video-based rocket detection
- Real-time optical tracking
- Kalman Filter integration
- Optical Flow tracking
- Camera pan-tilt-zoom control
- Rocket tracking under challenging conditions such as clouds, smoke, and long-distance launches.

---

## Author

Sanjana M

ISRO Internship Project
Optical Tracking System
````

---

### Also create a `requirements.txt` file:

```txt
ultralytics
opencv-python
sahi
numpy
matplotlib
```

---

### Git commands to push the project

```bash
git init
git add .
git commit -m "Initial commit: Optical Rocket Detection using YOLO"
git branch -M main
git remote add origin <your-github-repository-url>
git push -u origin main
```

This README is appropriate for an internship repository: it explains the project, how to set it up, how to run it, and where it is headed without overstating what has been implemented so far.
