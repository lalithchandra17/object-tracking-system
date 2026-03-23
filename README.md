# 🚗 Autonomous Green Object Tracking Robot

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv">
  <img src="https://img.shields.io/badge/RaspberryPi-Embedded-red?style=for-the-badge&logo=raspberrypi">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

## 📌 Overview

This project is an **Autonomous Object Tracking Robot** built using **Raspberry Pi, OpenCV, and embedded systems**.

It detects a **green-colored object in real-time**, calculates its distance using an ultrasonic sensor, and **autonomously adjusts movement** to maintain an optimal range.

This project showcases the integration of:

* 🤖 Robotics
* 👁️ Computer Vision
* ⚡ Real-time Control Systems

---

## 🎥 Demo (Add Your Output Here)

```
👉 Add images or videos of your robot here
Example:
![Demo](demo.gif)
```

---

## ✨ Features

✔️ Real-time object detection using OpenCV
✔️ Green color tracking using HSV filtering
✔️ Distance measurement using ultrasonic sensor
✔️ Autonomous movement (Forward / Backward / Stop)
✔️ PWM-based motor speed control
✔️ Buzzer alert system
✔️ Continuous real-time feedback loop

---

## 🧠 How It Works

1. 📷 Camera captures live video feed
2. 🎨 Frame converted to HSV color space
3. 🟢 Green object detected using thresholding
4. 📏 Distance calculated using ultrasonic sensor
5. 🤖 Decision logic:

   * Too close → Move backward
   * Too far → Move forward
   * Optimal distance → Stop
6. 🔊 Buzzer activates during motion

---

## 📏 Distance Logic

| Distance Range | Action        |
| -------------- | ------------- |
| < 4.2 cm       | Move Forward  |
| > 10.9 cm      | Move Backward |
| 4.2 – 10.9 cm  | Stop          |

---

## 🛠️ Tech Stack

### 🔌 Hardware

* Raspberry Pi
* L298N Motor Driver
* Ultrasonic Sensor (HC-SR04)
* Pi Camera (Picamera2)
* DC Motors
* Buzzer

### 💻 Software

* Python
* OpenCV
* NumPy
* RPi.GPIO
* Picamera2

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/object-tracking-robot.git
cd object-tracking-robot
```

### 2️⃣ Install Dependencies

```bash
pip install opencv-python numpy
```

### 3️⃣ Enable Camera

```bash
sudo raspi-config
```

* Enable Camera
* Reboot Raspberry Pi

### 4️⃣ Run Project

```bash
python main.py
```

---

## 🔌 GPIO Pin Configuration

| Component       | GPIO Pin |
| --------------- | -------- |
| Motor A IN1     | 20       |
| Motor A IN2     | 16       |
| Motor A ENA     | 21       |
| Motor B IN3     | 27       |
| Motor B IN4     | 22       |
| Motor B ENB     | 17       |
| Ultrasonic TRIG | 23       |
| Ultrasonic ECHO | 24       |
| Buzzer          | 10       |

---

## 📁 Project Structure

```
object-tracking-robot/
│── main.py
│── README.md
│── requirements.txt
```

---

## 📊 Output

* Detects green object in real-time
* Prints distance in terminal
* Moves robot dynamically
* Stops automatically in optimal range
* Activates buzzer during movement

---

## 🚀 Future Improvements

* 🔥 YOLO-based object detection
* 🧠 AI-based tracking instead of color filtering
* 📱 Mobile app integration
* 🗺️ Obstacle avoidance system
* ☁️ IoT-based remote monitoring

---

## 🧪 Applications

* Autonomous robots
* Smart surveillance systems
* Warehouse automation
* Robotics research projects

---

## 📜 License

This project is licensed under the MIT License

---

## 👨‍💻 Author

**Lalith Chandra**

---

## ⭐ Show Your Support

If you like this project, give it a ⭐ on GitHub!

---
