# Human Pose Detection using OpenCV and MediaPipe

## 📸 Project Overview

This project implements a real-time **human pose detection system** by leveraging **OpenCV** for video capture and **Google’s MediaPipe Pose** solution for landmark detection.  
It captures live feed from a webcam, detects key points on the human body (such as shoulders, elbows, knees, hips, etc.), and visualizes the human skeleton dynamically by connecting these landmarks.

Human pose estimation is a fundamental technology that drives a wide range of modern applications, from fitness tracking apps and rehabilitation monitoring to gesture-based controls, augmented reality, gaming, and sports performance analytics.

---

## 🌟 Why This Project?

- **Growing Relevance**: With the rise of AI in health, fitness, entertainment, and sports, the ability to accurately and efficiently detect human poses in real-time is becoming crucial.
- **Lightweight & Fast**: Built using MediaPipe’s highly optimized pose models, this project runs in real time on a basic laptop webcam without the need for expensive hardware like GPUs.
- **Practical Application Ready**: The project lays a strong foundation that can easily be extended for customized fitness apps, motion capture for animation, injury rehabilitation tracking, posture correction systems, and more.
- **Educational Value**: It serves as a great hands-on project for anyone looking to get into computer vision, machine learning, or AI-based human interaction systems.

---

## 🚀 How It Works

- The webcam feed is continuously captured using **OpenCV**.
- Each frame is processed through **MediaPipe Pose**, which detects **33 different human body landmarks**.
- The detected landmarks are drawn and connected to form a real-time skeleton overlay.
- The output is displayed back to the user with dynamic updating at real-time speed.

---

## 🛠️ Tech Stack

- **Python**
- **OpenCV** (`cv2`)
- **MediaPipe** (`mediapipe`)
- **NumPy** (`numpy`)

<br/>

## 🚀 Installation and Setup

Follow these steps to get the project up and running locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/pose-detection-opencv-mediapipe.git
   cd pose-detection-opencv-mediapipe
   ```

2. **Install Required Packages**:
   ```bash
   pip install mediapipe opencv-python numpy
   ```

3. **Run the Script**:
   ```bash
   python main.py
   ```
   (Or if you're using the notebook, simply run all the cells.)

4. **Allow Webcam Access** when prompted. Press **`q`** to quit the video feed.

<br/>

## 🧠 How It Works

- The webcam feed is captured using **OpenCV**.
- Each frame is converted from BGR to RGB (MediaPipe expects RGB input).
- MediaPipe's **Pose** model processes the image to detect human landmarks.
- The keypoints are drawn onto the frame using **MediaPipe’s drawing utilities**.
- The frame is converted back to BGR and displayed with OpenCV’s `imshow()` function.
- Pressing `q` exits the video window and stops the webcam feed.

<br/>

## 📈 Potential Use Cases

- Fitness apps that track body posture during exercises.
- Gesture-based control systems.
- Animation and AR applications.
- Health monitoring and rehabilitation.
- Sports performance analysis.

<br/>

## 📂 Project Structure

```
.
├── main.ipynb         # Main Notebook for Pose Detection
├── README.md          # Documentation
└── requirements.txt   # (Optional) List of dependencies
```

<br/>

## ⚙️ Requirements

- Python 3.7+
- OpenCV
- MediaPipe
- NumPy

You can also create a `requirements.txt` file:

```
mediapipe
opencv-python
numpy
```

and install all dependencies at once:

```bash
pip install -r requirements.txt
```

<br/>

## 📜 License

This project is licensed under the [MIT License](LICENSE).

<br/>

# 🙌 Acknowledgements

- [MediaPipe Pose](https://google.github.io/mediapipe/solutions/pose) by Google.
- [OpenCV](https://opencv.org/) library for real-time computer vision.

