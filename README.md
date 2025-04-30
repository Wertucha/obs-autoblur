# OBS AutoBlur — Real-Time Blurring of Sensitive Words or Images

A proof-of-concept script that automatically detects and blurs specific words or images (e.g. "google") in real-time while streaming or recording. Intended for use with OBS Studio.

---

## ✨ Features

- Detects target words in screen content using OCR (Tesseract).
- Blurs detected areas using OpenCV Gaussian blur.
- Automatically controls OBS recording via WebSocket API.
- Great for livestream moderation, privacy, and compliance.

---

## 🧪 Demo Use Case

Blur the word `"google"` in any visible area of your screen while recording or livestreaming using OBS.

---

## 📷 How It Works

- Uses `pyautogui` to capture screen frames.
- Uses `pytesseract` to extract text.
- Blurs target word areas in real-time.
- Uses `obsws-python` to start/stop OBS recording.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- OBS Studio with WebSocket plugin enabled
- Dependencies:
  ```bash
  pip install opencv-python pytesseract pyautogui obsws-python
