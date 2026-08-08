# 🚆 Integrated Track Monitoring System for Indian Railways 

An IoT-based intelligent railway track monitoring system designed for
real-time detection and monitoring of potential track abnormalities.

## 🏆 Achievement

🥈 Secured 2nd Prize at LUNARA 2K26,
an 8-hour hackathon organized by the Department of Computer Science
and Engineering, Bannari Amman Institute of Technology.

📅 Date: 10 April 2026

## 💡 Key Features

- Real-time railway track monitoring
- ESP32-based sensor acquisition
- Vibration monitoring
- Ultrasonic distance measurement
- ToF-based distance measurement
- Camera-based track inspection
- Image processing and edge detection
- Flask-based real-time dashboard
- Live sensor data visualization
- Alert generation

## ⚙️ Technologies

### Hardware
- ESP32
- Vibration Sensor
- Ultrasonic Sensor
- ToF Sensor
- Camera Module
- Gear Motors
- L298N Motor Driver

### Software
- Arduino IDE
- Embedded C / C++
- Python
- Flask
- OpenCV
- HTML
- CSS
- JavaScript

## 🔄 System Flow

Sensors → ESP32 → Wi-Fi → Flask Backend → Dashboard

Camera → Image Processing → Edge Detection → Analysis → Dashboard

## 🧠 Image Processing

The captured railway track image is processed using OpenCV.
Grayscale conversion, Gaussian filtering and Canny edge detection
are used to highlight structural edges that can indicate potential
track abnormalities.

## 📊 Dashboard

The dashboard displays:

- Sensor readings
- Vibration level
- Distance measurements
- Track status
- Camera image
- Processed image
- AI/Image-processing result
- Battery status
- Robot status

## 🚀 Future Scope

- Deep-learning-based crack detection
- YOLO-based defect detection
- Cloud data storage
- Predictive maintenance
- GPS-based defect mapping
- Mobile notifications
- Industrial-grade sensors
