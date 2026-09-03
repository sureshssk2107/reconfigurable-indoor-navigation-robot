Reconfigurable Indoor Navigation Robot

Project Overview

The Reconfigurable Indoor Navigation Robot is a low-cost Arduino-based mobile robotic platform that integrates multiple navigation and control strategies into a single robot.

The robot supports four operating modes:

1. Line Following
2. Obstacle Avoiding
3. Line + Obstacle Avoiding
4. Manual Control

The user can select the required operating mode using an IR remote without physically changing the robot's hardware configuration.

Problem Statement

Indoor environments can contain predefined paths as well as unexpected obstacles. A robot designed for only one navigation behaviour may not be suitable when the operating requirement changes.

This project addresses this limitation by providing multiple navigation and control strategies on a single robotic platform.

Proposed Solution

The robot combines IR sensors for line detection, an HC-SR04 ultrasonic sensor for obstacle detection, an HC-05 Bluetooth module for smartphone control, and an IR receiver with remote for mode selection and manual control.

An Arduino UNO acts as the main controller and processes the selected mode and sensor inputs to control the robot's movement through an L298 motor driver.

Operating Modes

1. Line Following

The robot follows a predefined path using two IR sensors. The Arduino UNO processes the sensor readings and controls the motors to maintain the robot's position on the path.

2. Obstacle Avoiding

The HC-SR04 ultrasonic sensor detects obstacles in front of the robot. Based on the detected obstacle, the Arduino UNO controls the motors to change the robot's movement and avoid collisions.

3. Line + Obstacle Avoiding

This mode combines line following and obstacle detection. The robot follows a predefined path while monitoring the environment for obstacles using the ultrasonic sensor.

4. Manual Control

The robot can be manually controlled using an HC-05 Bluetooth module connected to a smartphone or through the IR remote.

Mode Selection

The IR remote is used to select the required operating mode. The IR receiver receives the command and sends it to the Arduino UNO, which activates the corresponding control logic.

Hardware Components

- Arduino UNO
- IR Sensor × 2
- L298 Motor Driver
- HC-05 Bluetooth Module
- IR Receiver Module
- IR Remote
- SG90 Servo Motor
- HC-SR04 Ultrasonic Sensor
- DC Gear Motor × 4
- Robot Car Tyres × 4
- Male-to-Female Jumper Wires
- ON/OFF Switch
- 18650 Battery Holder – 2 Cell
- 18650 Battery Cell 3.7V × 2

Software

- Arduino IDE
- MIT App Inventor

Key Features

- Four operating modes on a single robotic platform
- IR-based mode selection
- Line following using IR sensors
- Obstacle detection using an ultrasonic sensor
- Combined line and obstacle navigation
- Bluetooth smartphone control
- IR remote control
- Arduino-based embedded control
- Low-cost hardware implementation

Applications

- Robotics education
- Indoor robotics experimentation
- Automation prototypes
- Assistive robotics research
- Robotics laboratory projects
- Navigation-system demonstrations

Future Improvements

Future development can include additional environmental sensors, improved sensor integration, IoT connectivity, enhanced obstacle detection and more advanced indoor navigation capabilities.

Project Status

Initial Prototype — Under Development

The robot is being developed and tested across all four operating modes. The repository will be updated with source code, hardware documentation, project photographs and testing results as development progresses.

Repository Contents

- "src/" — Arduino source code
- "hardware/" — Circuit and hardware documentation
- "documentation/" — Project presentation and supporting documents
- "media/" — Photographs and demonstration media

Team

Shakthi Priyan P
Sudharsan P
Sukumar P
Suresh Kumar S

Acknowledgement

This project was developed as part of the RECURSION — Edition II hackathon under the Smart Living, Automation & Assistive Technology track.

The implementation was developed using publicly available technical documentation and programming resources, with external resources and adapted code credited where applicable.
