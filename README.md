# FPV Night Patrolling Quadcopter Drone

<p align="center">
  <strong>A Drone-Based System for Night-Time Monitoring and Patrolling</strong>
</p>

<p align="center">
  <img src="images/drone_day_view.jpg" alt="Night Patrolling Drone" width="600">
</p>

---

## 📌 About the Project

The **FPV Night Patrolling Quadcopter Drone** is a drone-based project developed for **night-time monitoring, patrolling, and aerial surveillance applications**.

The system combines a quadcopter platform with a flight controller, Raspberry Pi, GPS, sensors, camera, wireless communication, and night-vision capabilities.

The project demonstrates the integration of:

**Drone Technology + Embedded Systems + Raspberry Pi + GPS + Sensors + Computer Vision**

---

## 🎯 Objectives

- To develop a quadcopter for night-time monitoring.
- To capture images and videos during low-light conditions.
- To integrate a Raspberry Pi for image processing.
- To use GPS for positioning and navigation.
- To use sensors for monitoring flight-related parameters.
- To explore object detection using computer vision and AI.
- To provide a platform for future autonomous patrolling applications.

---

## ⭐ Key Features

- Quadcopter-based aerial platform
- APM 2.8 flight controller
- Raspberry Pi 3
- GPS-based positioning
- Ultrasonic sensing
- Camera-based monitoring
- Night-vision support
- Wireless communication
- Computer vision and object detection
- Ground-station monitoring

---

## ⚙️ System Architecture

```text
                    ┌─────────────────┐
                    │   LiPo Battery  │
                    └────────┬────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Power Distribution  │
                  └──────────┬──────────┘
                             │
             ┌───────────────┼────────────────┐
             │               │                │
             ▼               ▼                ▼
        ┌─────────┐    ┌────────────┐   ┌──────────────┐
        │   ESCs  │    │  APM 2.8   │   │ Raspberry Pi │
        └────┬────┘    │ Controller │   │      3       │
             │         └──────┬─────┘   └──────┬───────┘
             ▼                │                │
       ┌───────────┐          │       ┌────────┼────────┐
       │  Motors   │          │       │        │        │
       │    ×4     │          │       ▼        ▼        ▼
       └───────────┘          │    Camera     GPS    Ultrasonic
                              │       │
                              │       ▼
                              │  Image Processing
                              │       │
                              │       ▼
                              │  Object Detection
                              │       │
                              └───────┼───────────┐
                                      ▼           │
                              ┌──────────────┐    │
                              │ Communication│◄───┘
                              └──────┬───────┘
                                     │
                                     ▼
                              ┌──────────────┐
                              │Ground Station│
                              └──────────────┘
```

---

## 🔧 Hardware Components

| Component | Purpose |
|---|---|
| Quadcopter Frame | Mechanical structure |
| APM 2.8 | Flight control and stabilization |
| Brushless Motors ×4 | Generate thrust |
| ESCs | Control motor speed |
| Propellers | Generate lift |
| 11.1V LiPo Battery | Main power source |
| Raspberry Pi 3 | Processing and communication |
| GPS Module | Position and navigation |
| Camera | Image and video capture |
| Ultrasonic Sensor | Distance measurement |
| LEDs / IR Illumination | Improve night visibility |
| Telemetry Module | Flight-data communication |

---

## 💻 Software & Technologies

| Technology | Purpose |
|---|---|
| ArduPilot | Flight-control software |
| Mission Planner | Ground-station and mission planning |
| Raspberry Pi OS | Raspberry Pi operating system |
| Python | Programming |
| OpenCV | Image processing |
| TensorFlow / TensorFlow Lite | Object detection |
| MAVLink | Flight-controller communication |

---

## 🔄 Working Principle

### 1. Power Supply

The LiPo battery supplies power to the drone's flight-control and electronic systems.

### 2. Flight Control

The **APM 2.8 flight controller** controls the quadcopter's stability and movement.

It manages:

- Roll
- Pitch
- Yaw
- Throttle
- Flight stabilization

### 3. Motor Control

The ESCs control the speed of the four brushless motors according to commands from the flight controller.

### 4. GPS Navigation

The GPS module provides positioning information for navigation and monitoring.

### 5. Sensor Monitoring

Ultrasonic sensors can be used for distance measurement and altitude-related monitoring.

### 6. Night Monitoring

The camera captures the surrounding environment. LEDs or infrared illumination can improve visibility in low-light conditions.

### 7. Image Processing

The Raspberry Pi receives camera data and can perform image processing using Python and OpenCV.

### 8. Object Detection

AI models such as TensorFlow or TensorFlow Lite can be used to detect objects from camera frames.

### 9. Communication

Telemetry and wireless communication allow flight information and other data to be monitored from the ground station.

---

## 🌙 Night Vision System

```text
       Low-Light Environment
                │
                ▼
        IR / LED Illumination
                │
                ▼
           Camera Input
                │
                ▼
          Raspberry Pi
                │
                ▼
        Image Processing
                │
                ▼
         Object Detection
                │
                ▼
         Ground Monitoring
```

---

## 🤖 Object Detection Pipeline

```text
Camera
  │
  ▼
Image Capture
  │
  ▼
Pre-processing
  │
  ▼
OpenCV / TensorFlow Lite
  │
  ▼
Object Detection
  │
  ▼
Detection Result
  │
  ▼
Ground Monitoring
```

---

## 📡 Communication System

```text
              DRONE
                │
       ┌────────┴────────┐
       │                 │
       ▼                 ▼
   APM 2.8          Raspberry Pi
       │                 │
       │            Wi-Fi / 4G
       │                 │
       └────────┬────────┘
                ▼
         Ground Station
                │
                ▼
             Operator
```

---

## 📷 Project Images

### Drone – Day View

<p align="center">
  <img src="images/drone_day_view.jpg" alt="Drone Day View" width="700">
</p>

### Drone – Night View

<p align="center">
  <img src="images/drone_night_view.jpg" alt="Drone Night View" width="700">
</p>

---

## 🎥 Project Demonstration

### Demonstration Video 1

[▶️ View Drone Demonstration Video 1](videos/drone_demo_video.mp4)

### Demonstration Video 2

[▶️ View Drone Demonstration Video 2](videos/drone_demo_video2.mp4)

---

## 📁 Repository Structure

```text
night-patrolling-drone/
│
├── README.md
│
├── images/
│   ├── drone_day_view.jpg
│   └── drone_night_view.jpg
│
└── videos/
    ├── drone_demo_video.mp4
    └── drone_demo_video2.mp4
```

---

## 🧪 Testing

The project can be tested using the following:

- Power supply test
- Motor and ESC test
- GPS test
- Sensor test
- Camera test
- Night-vision test
- Wireless communication test
- Flight stability test
- Object detection test

---

## 🚀 Applications

The system can be adapted for:

- Night-time aerial monitoring
- Campus monitoring
- Industrial-area monitoring
- Infrastructure inspection
- Wildlife observation
- Disaster-response support
- Authorized security monitoring
- Remote-area observation

---

## 🔮 Future Scope

Future improvements can include:

- Autonomous patrolling
- Advanced obstacle avoidance
- Improved object detection
- Thermal imaging
- Better GPS accuracy
- Longer flight duration
- Automatic object tracking
- Advanced computer vision
- Multi-drone coordination

---

## ⚠️ Safety & Responsible Use

This project is intended for **educational, research, and authorized monitoring applications**.

The drone should always be operated according to applicable drone regulations and safety requirements. It should not be used for unauthorized surveillance or activities that violate privacy or aviation regulations.

---

## 📚 Research Paper

A research paper related to this project is available below:

**[View Research Paper](https://www.doi.org/10.5281/zenodo.15250212)**

---

## 👨‍💻 Project Information

**Project:** FPV Night Patrolling Quadcopter Drone

**Department:** Electronics and Telecommunication Engineering

**Academic Year:** 2024–2025

---

## 📜 Conclusion

The **FPV Night Patrolling Quadcopter Drone** demonstrates the integration of drone technology, embedded systems, Raspberry Pi, GPS, sensors, wireless communication, night monitoring, and computer vision.

The project provides a foundation for developing more advanced aerial monitoring and autonomous drone systems in the future.

---

<p align="center">
  <strong>🚁 FPV NIGHT PATROLLING QUADCOPTER DRONE</strong>
</p>
