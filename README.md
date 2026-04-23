# ✋ Gesture-Controlled Robotic Arm 🤖

## 📌 Overview

This project implements a real-time **gesture-controlled robotic arm** using **computer vision** and **embedded systems**. Hand gestures captured through a webcam are processed using **MediaPipe**, then translated into servo motor movements through an **Arduino**.

The system demonstrates **human-computer interaction (HCI)** by enabling intuitive, touchless control of robotic hardware.

---

## 🎯 Problem Statement

Traditional robotic arm control systems often rely on physical interfaces such as joysticks, switches, or buttons. These methods can be restrictive, unintuitive, and less interactive for modern automation needs.

This project aims to:

- Enable **contactless control**
- Improve **ease of use**
- Demonstrate **real-time AI + hardware integration**

---

## 🧠 System Architecture

```text
## 🧠 System Architecture

```text
Gesture Sensor / Glove → Data Acquisition (Flex / IMU / Potentiometers)
        ↓
   Microcontroller (Transmitter)
        ↓ (Processed angles / codes)
    Bluetooth Module (TX)
        ↓  ~~~ Wireless Link (Bluetooth) ~~~  ↓
    Bluetooth Module (RX)
        ↓
   Microcontroller (Receiver / Robot Controller)
        ↓
   Servo & Stepper Motor Drivers → Robotic Arm Joints & Gripper
```
```

---

## ⚙️ Tech Stack

### Software
- Python
- OpenCV
- MediaPipe
- NumPy

### Hardware
- Arduino Uno
- Servo Motors

### Communication
- Serial Communication (USB)

---

## 🔄 Workflow

1. Capture live video feed using a webcam  
2. Detect hand landmarks using MediaPipe  
3. Identify gestures based on landmark positions  
4. Map gestures to predefined servo angles  
5. Send commands via serial communication  
6. Arduino processes commands and moves servos  

---

## 🚀 Features

- Real-time gesture recognition
- Low-latency communication
- Modular design with separate vision and control layers
- Easy integration with Arduino-based robotic systems
- Scalable for advanced robotics applications

---

## 📊 Performance Metrics

> Add measured results after testing.

- **Frame Rate:** ~XX FPS
- **Latency:** ~XX ms
- **Gesture Accuracy:** ~XX%

---

## 🎥 Demo

👉 Add your demo video link here

Example:
```md
[Project Demo](https://your-video-link-here)
```

---

## 📂 Project Structure

```text
Gesture-Controlled-Robotic-Arm/
│── src/              # Python scripts
│── arduino/          # Arduino code
│── docs/             # Images, diagrams
│── README.md
```

---

🔮 Future Improvements

- Machine Learning-based gesture classification
- Wireless control using Bluetooth or WiFi
- Multi-hand gesture support
- Object gripping automation
- Error handling and motion smoothing


🧪 Applications

This project can be extended for use in:

- Assistive robotics
- Industrial automation
- Smart interfaces
- Human-computer interaction research
- Touchless robotic control systems


🧾 Conclusion

This project highlights the integration of **AI, computer vision, and embedded systems** to build an intuitive robotic control system. It serves as a foundation for future work in **automation**, **assistive robotics**, and **smart human-machine interfaces**.

---

👨‍💻 Author

**N Avanish Reddy and Team**

If you found this project useful, consider starring the repository.
