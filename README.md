# Eye Controlled Mouse 🖱️👁️

Control your computer mouse using your eye movements and blink detection! This project uses **OpenCV**, **MediaPipe**, and **PyAutoGUI** to track facial landmarks and simulate mouse actions.

---

## 🚀 Features

* Move mouse cursor using eye position
* Perform mouse click by blinking
* Real-time face and eye tracking
* Simple and lightweight implementation

---

## 🛠️ Technologies Used

* Python
* OpenCV (`cv2`)
* MediaPipe
* PyAutoGUI

---

## 📦 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/eye-controlled-mouse.git
   cd eye-controlled-mouse
   ```

2. Install required dependencies:

   ```bash
   pip install opencv-python mediapipe pyautogui
   ```

---

## ▶️ Usage

Run the script:

```bash
python main.py
```

---

## 🎮 How It Works

* The webcam captures your face in real time.
* MediaPipe detects facial landmarks.
* Specific eye landmarks (474–478) control cursor movement.
* A blink is detected using vertical distance between eye landmarks.
* When a blink is detected, a mouse click is triggered.

---

## ⚙️ Controls

| Action      | Input Method     |
| ----------- | ---------------- |
| Move Cursor | Eye Movement     |
| Click       | Blink (left eye) |

---

## ⚠️ Notes

* Ensure good lighting for accurate tracking.
* Avoid excessive head movement.
* Webcam quality affects performance.
* Blink sensitivity may need adjustment depending on your face and distance from camera.

---

## 🧠 Future Improvements

* Right-click support
* Scroll functionality
* Calibration system
* Multi-eye gesture controls

---

## 📄 License

This project is open-source and available under the MIT License.

---

## 🙌 Acknowledgements

* MediaPipe for facial landmark detection
* OpenCV for image processing
* PyAutoGUI for mouse automation

---

## 💡 Tip

If the cursor feels too sensitive or inaccurate, try adjusting:

```python
if (left[0].y - left[1].y) < 0.008:
```

Increase or decrease the threshold for better blink detection.

---

Enjoy controlling your computer with just your eyes! 👁️✨
