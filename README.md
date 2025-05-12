# Emotion Recognition Using Body Gestures and Facial Expressions

This project is a real-time emotion recognition system that uses **MediaPipe** for extracting body and face landmarks and a machine learning model for classifying emotions based on the extracted keypoints.

## 🔍 Project Overview

The system uses:
- **MediaPipe Holistic** for detecting facial landmarks, body posture, and hand positions.
- A trained **machine learning model** (RandomForest/any ML classifier) for predicting human emotions.
- **OpenCV** for real-time video capture and visualization.

## 🎯 Objective

To classify emotions such as *happy, sad, angry, surprised*, etc., using both **facial expressions** and **body gestures**.

---

## 🛠️ Features

- Real-time detection from webcam
- Keypoint extraction using MediaPipe
- Classification of emotion using trained model (`body_language.pkl`)
- Visualization of face mesh and pose/hand landmarks
- Display predicted emotion with probability

---

## 🧠 Model

The model was trained on keypoints extracted from:
- **33** pose landmarks (with 4 values each: x, y, z, visibility)
- **468** face landmarks (x, y, z, visibility)
- **21** left hand + **21** right hand landmarks (x, y, z)

➡️ **Total features**: `33*4 + 468*4 + 21*3 + 21*3 = 2130`

The model is stored in a pickle file:
```bash
body_language.pkl
