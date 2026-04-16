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
👉  https://drive.google.com/file/d/1r48AJdCEntRK7WYsC-S6GnDcOJ9-iNiD/view?usp=sharing
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
<img width="1815" height="850" alt="traking" src="https://github.com/user-attachments/assets/2f62c7be-04f9-4a42-afc4-3429bda0008e" />
<img width="1821" height="827" alt="2_12" src="https://github.com/user-attachments/assets/0347a2cc-063d-42d4-8e85-a0d663e5d3b7" />
<img width="1792" height="812" alt="654ed" src="https://github.com/user-attachments/assets/3c76b080-4d4b-4092-85c9-23e81fd49556" />




---

## 📌 Conclusion

This project demonstrates a real-world scalable computer vision pipeline for multi-object tracking.
