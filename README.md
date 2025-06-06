# 🎭 Emotion Detection via Facial Expressions & Body Gestures

A real-time emotion recognition system using **MediaPipe** and **Machine Learning**, capable of detecting and classifying human emotions based on **facial expressions**, **hand gestures**, and **body posture**.

---

## 📌 Project Overview

This project combines:
- **MediaPipe Holistic** for extracting body, face, and hand landmarks
- A **trained ML model** for emotion classification
- **OpenCV** for real-time webcam processing and display

---

## 🎯 Goals

- Detect facial and body landmarks in real time
- Extract 2,130 keypoint features per frame
- Predict human emotions like *happy*, *sad*, *angry*, *surprised*, etc.
- Visualize both prediction and facial/pose mesh

---

## 🧠 Model Details

The model uses:
- **Pose Landmarks**: 33 points × 4 features = 132
- **Face Landmarks**: 468 points × 4 features = 1,872
- **Left & Right Hand**: 21 × 3 × 2 = 126  
➡️ **Total**: **2,130 features**

Trained model is stored in `body_language.pkl`.

---

## 📸 Results

Here are some sample outputs from the emotion recognition system:

![Prediction Output](results/img1.jpg)
![Prediction Output](results/img2.jpg)
![Prediction Output](results/img3.jpg)
![Prediction Output](results/img4.jpg)
![Prediction Output](results/img5.jpg)
![Prediction Output](results/img6.jpg)
![Prediction Output](results/img7.jpg)
![Prediction Output](results/img8.jpg)
![Data Flow Diagram](results/dfd.jpg)




## 🛠️ Requirements

Make sure you have **Python 3.7+**. Install dependencies using:

```bash
pip install -r requirements.txt



