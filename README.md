# 🧠 Real-Time Face Mesh & Mask Analysis System

## 📌 Overview
This project is a real-time face analysis system built using computer vision techniques. It detects facial landmarks and analyzes user behavior such as eye blinking, mouth movement, and head direction using live webcam input in Google Colab.

The system uses **MediaPipe FaceMesh** to extract 468 facial landmarks and applies simple yet effective logic to interpret facial actions.

---

## 🚀 Features
- 📷 Capture webcam frames directly in Google Colab  
- 🔍 Detect 468 facial landmarks using FaceMesh  
- 👁️ Blink detection using Eye Aspect Ratio (EAR)  
- 😮 Mouth open/close detection  
- 🧭 Head direction estimation (Left / Right / Forward)  
- 🖥️ Side-by-side visualization (raw image + mesh overlay)  
- 💾 Option to save and download output  

---

## 🛠️ Tech Stack
- Python  
- MediaPipe  
- OpenCV  
- NumPy  
- Pillow  
- Google Colab  

---

## 📊 How It Works

### 🔹 Face Detection & Landmark Extraction
- Uses MediaPipe FaceMesh  
- Detects **468 facial landmarks** in real time  

---

### 🔹 Blink Detection
- Based on distance between eye landmarks  
- If distance is small → eye is considered closed  

---

### 🔹 Mouth Detection
- Measures gap between upper and lower lips  
- Larger gap → mouth is open  

---

### 🔹 Head Direction
- Uses nose position to estimate:
  - Left  
  - Right  
  - Forward  

---

## 🖼️ Output
The system displays:
- Left → Live camera frame  
- Right → Face mesh overlay  


---

## ▶️ How to Run

1. Open the notebook in Google Colab  
2. Install dependencies (first cell)  
3. Run all cells step by step  
4. Click **Capture Frame** to analyze face  

---

## 📦 Dependencies
```bash
pip install mediapipe==0.10.9 opencv-python-headless Pillow
