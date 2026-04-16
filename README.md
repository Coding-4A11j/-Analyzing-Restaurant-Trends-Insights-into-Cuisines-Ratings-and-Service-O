# Multi-Object Detection and Persistent ID Tracking

## 📌 Overview

This project implements an end-to-end computer vision pipeline for detecting and tracking multiple subjects in sports/event videos. Each detected subject is assigned a unique and persistent ID across the video.

---

## 🎯 Objective

* Detect all relevant subjects (persons)
* Assign unique IDs to each subject
* Maintain ID consistency across frames
* Handle occlusion, motion blur, and camera movement

---

## 🛠️ Tech Stack

* Python
* OpenCV
* YOLOv8 (Ultralytics)
* ByteTrack

---

## 📂 Input Video

Public video source:
👉 [PASTE YOUR VIDEO LINK HERE]

---

## ▶️ How to Run

1. Install dependencies:

```id="z1slnd"
pip install ultralytics opencv-python numpy
```

2. Run the notebook or script:

```id="wt0fz1"
python main.py
```

3. Upload your input video and execute all cells.

---

## ⚙️ Pipeline

Video → Frame Extraction → YOLOv8 Detection → ByteTrack Tracking → ID Assignment → Annotated Output Video

---

## 🧠 Model & Tracker

* YOLOv8: real-time object detection
* ByteTrack: robust multi-object tracking

---

## 📊 Features Implemented

* Bounding box detection
* Persistent ID tracking
* Trajectory visualization
* Player counting
* Basic speed estimation

---

## ⚠️ Assumptions

* Only "person" class is tracked
* Moderate crowd density
* Standard lighting conditions

---

## ❌ Limitations

* ID switching in heavy occlusion
* No Re-ID (appearance matching)
* Pixel-based speed (not real-world)

---

## 🚀 Future Improvements

* DeepSORT with Re-ID
* Heatmap generation
* Team classification
* Bird’s-eye view tracking

---

## 📸 Results

Screenshots available in /screenshots folder.

---

## 📌 Conclusion

This project demonstrates a real-world scalable computer vision pipeline for multi-object tracking.
