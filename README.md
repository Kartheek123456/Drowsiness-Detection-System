##  Drowsiness Detection System
This is a real-time drowsiness alert system that uses a Convolutional Neural Network (CNN) to monitor eye activity through a webcam. When prolonged eye closure is detected, an alarm is triggered to prevent accidents due to drowsiness.

## Features
- Detects closed eyes using a trained CNN model
- Triggers a warning alarm after 3 seconds of continuous eye closure
- Uses Haar Cascades for face and eye detection
- Integrated with live webcam monitoring using OpenCV
- Lightweight and suitable for real-time usage
- Alarm remains active until the eyes are fully open

## How It Works 
1. Live webcam feed captures the user's face.
2. Haar Cascades detect face, left eye, and right eye.
3. Each eye image is processed and passed to a CNN model.
4. If both eyes are classified as "Closed" for a continuous period, an alarm is played.
5. The system resets the alert once eyes are detected as "Open".

## Installation

### Set Up Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate

## Install Requirements**
pip install -r requirements.txt

## Run the App**
python main.py

**Requirements **
Python 3.7+
OpenCV
TensorFlow
Keras
NumPy
Pygame
