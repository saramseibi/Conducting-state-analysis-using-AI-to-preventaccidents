# Eye Blink and Drowsiness Detection

This project uses **OpenCV**, **Mediapipe**, and **Python** to detect **eye blinks**, **mouth movement**, and **eye gaze direction** in real time. It can help monitor drowsiness by tracking blink frequency and giving an **audio alert** when the user seems to be falling asleep.

---

## 🚀 Features
- **Real-time face mesh detection** using Mediapipe  
- **Eye blink detection** with blink counter  
- **Drowsiness detection** → triggers voice alert when eyes remain closed too long  
- **Eye gaze tracking** (left, right, center)  
- **Mouth ratio tracking** (for yawning detection – can be extended)  
- **Audio alert system** using `pyttsx3`  
- **FPS counter** for performance monitoring  

---

## 🛠️ Tech Stack
- [Python](https://www.python.org/)  
- [OpenCV](https://opencv.org/)  
- [Mediapipe](https://developers.google.com/mediapipe)  
- [NumPy](https://numpy.org/)  
- [pyttsx3](https://pypi.org/project/pyttsx3/)  

---

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/saramseibi/Conducting-state-analysis-using-AI-to-preventaccidents.git
   cd eye-blink-detection
   ```
2.Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3.Required libraries:
   ```bash
   opencv-python
   mediapipe
   numpy
   pyttsx3
   ```
## 📊 How It Works
-Mediapipe provides 468 facial landmarks.

-Eye aspect ratio (EAR) is calculated using Euclidean distances between eye landmarks.

-If eyes remain closed for more than a set threshold → system triggers "Wake up!" alert.

-Blink count is tracked for performance/statistics.

-Eye regions are cropped to estimate eye position (left, right, center).

---
