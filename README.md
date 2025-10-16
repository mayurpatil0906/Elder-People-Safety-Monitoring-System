# Elder-People-Safety-Monitoring-System
🧓 Elder People Monitoring System
🔒 AI-Powered Real-Time Safety Monitoring for Elderly Care

Elderly individuals often live alone, and their safety is a major concern — they are prone to accidental falls, and sometimes unsafe or threatening situations can occur at home or care centers.
Manual monitoring isn’t always reliable or possible 24/7.

To address this, I developed a smart AI-based monitoring system that continuously observes elderly people in real time, detects falls automatically, and identifies dangerous objects such as knives or guns — sending instant alerts to caregivers or family members.

🎯 Problem Statement

Elderly people living independently face a high risk of accidents, especially falls, which can lead to serious injuries if help doesn’t arrive quickly.
Additionally, potential threats such as weapons or unsafe intrusions can put them in danger.

Traditional monitoring systems depend on manual observation or wearable devices — both of which are inconvenient and prone to failure.

💡 Solution Overview

The Elder People Monitoring System combines Computer Vision and Machine Learning to enable continuous real-time monitoring and automatic alerting.

The system uses a live camera feed analyzed by the YOLOv8 object detection model to recognize people and detect hazardous items such as knives or guns.
A separate fall detection module tracks posture and motion patterns to identify accidental falls.

Whenever a fall or weapon is detected, the system:

Sends instant alerts to caregivers or family members via Pushbullet integration.

Logs the event in the local database with details such as event type and timestamp.

This ensures a fast response, timely assistance, and peace of mind for families and caregivers.

🧠 Languages and Frameworks

Language: Python 3.10

Object Detection: YOLOv8 (Ultralytics)

Image Processing: OpenCV

Backend Framework: Flask

Machine Learning Backend: TensorFlow / PyTorch

Alert Notifications: Pushbullet API Integration

📦 Libraries Used

ultralytics – YOLOv8 model for object and person detection

opencv-python – Handles image capturing and video stream analysis

flask – For building a lightweight web interface and backend API

pushbullet.py – For sending instant notifications to registered devices

numpy, time, os, threading – Core utility libraries

🏗️ System Architecture
⚙️ Architecture Flow

Camera Module – Captures a continuous video feed of the monitored area.

YOLOv8 Detection Module – Detects objects such as people, knives, or guns from live frames.

Fall Detection Module – Analyzes body posture and motion to detect accidental falls.

Alert System – Triggers an immediate notification using Pushbullet when a risky event is detected.

Database – Records all alerts with timestamps for later review or analysis.

Web Dashboard – Built with Flask, displays live camera feed, alerts, and event logs.

📊 Results

Successfully detected falls and dangerous objects in real time.

Reduced monitoring delay through instant alerting.

Achieved efficient frame-by-frame inference using GPU support.

Provided a web interface for live supervision and control.


