<<<<<<< HEAD
# Wireless Volume Control by Hand Detection

A real-time gesture-based volume control system using computer vision. Control your system volume by simply moving your index finger and thumb in front of a webcam — no physical contact required.

---

## What This Does

Detects hand landmarks in real time using MediaPipe, tracks the distance between the index finger and thumb, and maps that distance to system volume. A visual volume bar provides instant feedback on screen.

---

## How It Works

1. Webcam captures live video feed
2. MediaPipe detects hand landmarks (21 keypoints)
3. Distance between thumb (landmark 4) and index finger (landmark 8) is calculated
4. Distance is mapped to system volume range using `numpy.interp`
5. Volume is set in real time via `pycaw` (Windows audio API)
6. Visual feedback shown as volume bar and percentage on screen

---

## Files

| File | Description |
|------|-------------|
| `HandTrackingModule.py` | Hand detection and landmark tracking class |
| `VolumeHandControl.py` | Main volume control application |
| `requirements.txt` | Python dependencies |

---

## How to Run

```bash
pip install -r requirements.txt
python VolumeHandControl.py
```

Point your hand at the webcam and move your thumb and index finger apart to increase volume, together to decrease.

---

## Requirements

- Python 3.8+
- Webcam
- Windows OS (pycaw is Windows-only)
- Libraries: OpenCV, MediaPipe, pycaw, NumPy

---

## Tech Stack

Python · OpenCV · MediaPipe · pycaw · NumPy · Computer Vision · Gesture Recognition

---

## Author
Sai Naveena Kode — CSE Mini Project, GRIET, 2022-2023

