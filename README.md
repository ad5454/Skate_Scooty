# Autonomous Scooter Project - "Skate Scooty"

An autonomous two-wheeled scooter designed for urban mobility solutions, with capabilities for real-time navigation, lane detection, object recognition, and more. This project explores a differential drive bot prototype for testing algorithms, eventually scaling to a full-scale autonomous scooter powered by Jetson Nano.

## Project Overview

The goal of this project is to build an autonomous scooter with advanced mapping, navigation, and control features. Starting with a small-scale bot, the project aims to understand and refine autonomous algorithms for future application in a full-scale, two-wheeled scooter.

### Key Components

- **Hardware**:
  - Jetson Nano for computational processing
  - Lidar and Camera for navigation and perception
  - Custom Battery Management System (BMS)
  - Servo Motors for precise control

- **Software**:
  - ROS (Robot Operating System) for robotic middleware
  - TensorFlow for computer vision and object detection
  - Integration of a virtual environment to test in both simulated and real-world conditions

- **Control**:
  - Logitech F710 gamepad for teleoperation, with Axis 2 mapped for steering and Axis 3 for forward motion
  - Python script to map steering angles and speed, with the Arduino controlling steering (`s`), motor speed (`m`), and braking (`b`)

## Features

- **Real-Time Mapping & Navigation**:
  - Autonomous navigation and obstacle avoidance based on Lidar and Camera data

- **Computer Vision**:
  - Lane line detection, traffic sign classification, and object recognition for enhanced situational awareness

- **Docking & Parking**:
  - Advanced docking station detection and automatic parking capabilities

- **Teleoperation**:
  - Joystick-based control for manual navigation with real-time feedback

## Getting Started

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/autonomous-scooter.git
    cd autonomous-scooter
    ```

2. **Install Dependencies**:
    Ensure you have ROS and TensorFlow installed. You may also need other Python packages as listed in `requirements.txt`.
    ```bash
    pip install -r requirements.txt
    ```

3. **Hardware Setup**:
    - Assemble the components as per the hardware guide.
    - Connect the Jetson Nano to the Lidar, Camera, and Servo Motors.

4. **Run the Scripts**:
    - Use the teleoperation script for manual control:
        ```bash
        python teleop_control.py
        ```
    - For autonomous mode, ensure Lidar and Camera feeds are connected and run:
        ```bash
        python autonomous_navigation.py
        ```

## Project Structure

- `src/`: Contains the core codebase for teleoperation, autonomous navigation, and perception modules.
- `docs/`: Includes project documentation, setup guides, and hardware assembly instructions.
- `requirements.txt`: Python dependencies for the project.

## Future Scope

This project envisions additional capabilities:
- Enhanced lane detection and object classification for urban navigation
- Docking and parking systems with improved real-time detection
- Battery management optimizations to increase operational efficiency

## Contributing

Contributions are welcome! Please fork the repository and make a pull request with your changes. For major changes, open an issue first to discuss what you'd like to implement.
