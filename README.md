# Autonomous Drone Project

![Drone Image](Assets/My_Main_project_demo.gif)

## 📋 Project Overview

This project involves the design and implementation of an autonomous quadcopter drone with GPS tracking capabilities and obstacle avoidance systems. The drone is programmed to autonomously navigate between waypoints using GPS coordinates while detecting and avoiding obstacles in its path.

### 🔑 Key Features

- **Autonomous Navigation**: GPS-guided waypoint navigation
- **Obstacle Avoidance**: Real-time detection and avoidance of obstacles
- **Object Detection**: TensorFlow-based object recognition system
- **Modular Design**: Easily reprogrammable for various applications
- **Safety Features**: Rugged design to withstand collisions and moderate wind conditions
- **Manual Override**: Switch between autonomous and manual control

## 🛠️ Hardware Components

- **Frame**: S500 Quadcopter Frame (Glass Fiber with Polyamide-Nylon arms)
- **Flight Controller**: APM with External Compass
- **Processing Unit**: Raspberry Pi 3
- **Motors**: Brushless DC Motors
- **ESCs**: 30A Electronic Speed Controllers
- **Power**: LiPo Battery (4S 14.8V)
- **Sensors**:
  - GPS Module
  - Ultrasonic Sensors for obstacle detection
  - Accelerometer/Gyroscope
  - Magnetometer (Compass)
  - Barometer
- **Communication**: 2.4GHz RC Transmitter and Receiver

## 💻 Software Stack

- **Flight Control**: Mission Planner for programming APM
- **Object Detection**: TensorFlow Object Detection API
- **Operating System**: Raspberry Pi OS
- **Programming Languages**: Python for image processing and obstacle avoidance algorithms

## 🔄 System Architecture

```
┌─────────────────┐     ┌────────────────┐     ┌────────────────┐
│ RC Transmitter  │◄────┤ APM Flight     │◄────┤ Raspberry Pi   │
│ (Manual Control)│     │ Controller     │     │ (Processing)   │
└─────────────────┘     └───────┬────────┘     └────────┬───────┘
                                │                       │
                        ┌───────┴────────┐     ┌────────┴───────┐
                        │ Motors & ESCs  │     │ Sensors        │
                        │                │     │ - GPS          │
                        └────────────────┘     │ - Ultrasonic   │
                                               │ - Camera       │
                                               └────────────────┘
```

## 🚀 Applications

The modular design enables the drone to be utilized in various scenarios:

- **Delivery**: Small package transportation
- **Surveillance**: Area monitoring and security
- **Agriculture**: Crop inspection and monitoring
- **Search and Rescue**: Assist in locating missing persons
- **Mapping**: Aerial surveying and 3D mapping

## 🔧 Setup and Configuration

1. **Hardware Assembly**:
   - Assemble the frame
   - Mount motors and connect ESCs
   - Install APM flight controller
   - Connect receiver to APM input pins
   - Mount GPS module
   - Install Raspberry Pi and connect to APM

2. **Software Setup**:
   - Install Mission Planner and configure APM
   - Set up flight modes and calibrate sensors
   - Configure communication between Raspberry Pi and APM
   - Install obstacle avoidance algorithm
   - Set up object detection system

3. **Calibration**:
   - Compass calibration
   - Accelerometer calibration
   - Radio calibration
   - Motor direction verification

## 📊 Performance Metrics

- **Flight Time**: ~15-20 minutes (depending on payload)
- **Maximum Speed**: 35 km/h
- **Range**: 1-2 km (with RC control)
- **GPS Accuracy**: Within 5m
- **Obstacle Detection Range**: Up to 4m

## 🔍 Future Work

- Implement multi-UAV coordination and motion planning
- Enhance visual algorithms for better object recognition
- Improve battery efficiency for extended flight time
- Develop advanced autonomous navigation capabilities
- Add machine learning for adaptive flight patterns

## 📚 References

- TensorFlow Object Detection API
- ArduPilot Documentation
- Raspberry Pi Documentation
- IEEE Papers on Autonomous Drone Systems
- NASA UTM (Unmanned Aircraft System Traffic Management)

## 📄 License

[MIT License](LICENSE)

