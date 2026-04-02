# 🧠 Smart Surveillance System using YOLOv8

## 📌 Overview

This project implements a **Smart Surveillance System** that detects and tracks people in video streams using **YOLOv8**. The system identifies individuals and assigns unique IDs to track their movement across frames.

---

## 🎯 Objectives

* Detect people in images and videos
* Track individuals across frames using unique IDs
* Build an end-to-end computer vision pipeline
* Demonstrate real-time surveillance capability

---

## 🛠️ Technologies Used

* Python
* OpenCV
* YOLOv8 (Ultralytics)
* Google Colab

---

## ⚙️ Methodology

### 1. Object Detection

A pre-trained YOLOv8 model is used to detect people in each frame of the video.

### 2. Object Tracking

ByteTrack algorithm is used to assign unique IDs to detected individuals and track them across frames.

### 3. Video Processing

The system processes video input frame-by-frame and generates output with bounding boxes and tracking IDs.

---

## 📂 Project Structure

```
smart-surveillance/
│── notebook.ipynb
│── input_video.mp4
│── output_video.mp4
│── README.md
```

---

## 🚀 How to Run

1. Install dependencies:

```bash
pip install ultralytics opencv-python
```

2. Run detection and tracking:

```python
from ultralytics import YOLO

model = YOLO("yolov8n.pt")

model.track(
    source="input_video.mp4",
    show=True,
    save=True
)
```

---

## 📊 Results

* Successfully detected multiple people in video frames
* Assigned unique IDs for tracking
* Generated output video with bounding boxes and IDs

---

## ⚠️ Challenges

* Occlusion (people overlapping)
* Motion blur in fast videos
* Lighting variations

---

## 🔮 Future Improvements

* Face recognition integration
* Suspicious activity detection
* Multi-camera tracking system
* Real-time dashboard visualization

---

## 🎬 Demo

The output video demonstrates real-time detection and tracking of individuals with bounding boxes and unique IDs.

---

## 📌 Conclusion

This project demonstrates how deep learning and computer vision can be applied to build intelligent surveillance systems for real-world applications.

---

## 🙌 Author

Sohaib Altaf

---
