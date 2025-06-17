# 🎭 Real-Time Emotion Detection using YOLOv8 and Supervision

This project demonstrates real-time **emotion detection** from video input using a **YOLOv8** model fine-tuned on a custom emotion detection dataset. It uses the **Supervision** library for drawing bounding boxes and class labels.

---

## 📂 Project Overview

Using a fine-tuned YOLOv8 model, this system detects and classifies human emotions in video frames. The model identifies eight emotional states and annotates them on the video output.

---

## 🔍 Detected Emotions

The model detects the following 8 emotion classes:

| ID | Emotion   |
|----|-----------|
| 0  | Anger     |
| 1  | Content   |
| 2  | Disgust   |
| 3  | Fear      |
| 4  | Happy     |
| 5  | Neutral   |
| 6  | Sad       |
| 7  | Surprise  |

---

## 🚀 Technologies Used

- [YOLOv8](https://github.com/ultralytics/ultralytics) – Real-time object detection model
- [Supervision](https://github.com/roboflow/supervision) – For visualizing detections
- Python

---

## 🛠️ How It Works

1. Load the fine-tuned YOLOv8 model:
   ```python
   model = YOLO("/content/emotion_detection_model.pt")
