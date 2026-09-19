# Arduino Radar Detection System

An Arduino-based radar detection system that uses an **HC-SR04 ultrasonic sensor** and a **servo motor** to detect objects, measure their distance, and visualize their position across different scanning angles.

This project was developed as a **BSc group project** to demonstrate the practical use of Arduino, ultrasonic sensing, servo control, and real-time visualization.

## Project Overview

The system works by rotating an ultrasonic sensor using a servo motor and measuring the distance of objects detected in front of it.

As the servo scans through different angles, the Arduino continuously collects distance measurements. These measurements can then be visualized as a radar-like display, showing the detected object's approximate angle and distance.

### Main Workflow

```text
Ultrasonic Sensor
       ↓
Distance Measurement
       ↓
Arduino Processing
       ↓
Servo Motor Scanning
       ↓
Serial Data
       ↓
Radar Visualization
       ↓
Detected Object + Distance + Angle
```

## Features

* Real-time object detection
* Distance measurement using an HC-SR04 ultrasonic sensor
* Servo-controlled scanning
* Detection across different angles
* Radar-style visualization
* Serial communication between the Arduino and visualization software
* Approximate detection accuracy of 95% based on project testing

## Hardware Requirements

* Arduino board
* HC-SR04 ultrasonic sensor
* Servo motor
* Jumper wires
* Breadboard
* USB cable
* Computer for visualization

## Software Requirements

* Arduino IDE
* Arduino programming environment
* Python / Processing-based visualization environment
* Serial communication interface

## How It Works

### 1. Servo Motor Scanning

The servo motor rotates the ultrasonic sensor through a range of angles.

At each angle, the sensor takes a distance measurement.

### 2. Ultrasonic Distance Measurement

The HC-SR04 sensor sends an ultrasonic pulse and measures the time taken for the reflected signal to return.

The Arduino uses this time to estimate the distance between the sensor and the detected object.

### 3. Arduino Processing

The Arduino combines:

* Current servo angle
* Measured distance

and sends the information through serial communication.

### 4. Radar Visualization

The received data is used by the visualization program to represent detected objects on a radar-style interface.

This allows the user to visually understand:

* Where an object is located
* Its approximate distance
* The angle at which it was detected

## Example

If an object is detected at approximately:

```text
Angle: 90°
Distance: 30 cm
```

the visualization represents the object at the corresponding position on the radar display.

## Project Structure

The repository contains the project documentation and demonstration materials:

```text
RADAR-WITH-AURDINO-DETECTION/
│
├── 1783571883188.jpg
├── RADAR WITH AURDINO DETECTION .pdf
├── VID-20250522-WA0019.mp4
└── README.md
```

## Results

The project successfully demonstrated real-time object detection and distance measurement using an Arduino, HC-SR04 ultrasonic sensor, and servo motor.

The project documentation reports approximately **95% detection accuracy** under the tested conditions.

Actual performance can vary depending on factors such as:

* Object surface
* Object distance
* Sensor orientation
* Environmental conditions
* Servo positioning
* Ultrasonic reflections

## Applications

The basic concept can be applied to:

* Object detection systems
* Robotics
* Obstacle detection
* Autonomous vehicle prototypes
* Security and monitoring prototypes
* Embedded systems learning
* Sensor-based automation

## Limitations

The system has some practical limitations:

* Ultrasonic sensors have a limited detection range.
* Accuracy can vary depending on the object's surface and shape.
* Multiple objects can make detection more difficult.
* The system is intended as an educational/prototype radar system rather than a replacement for professional radar technology.
* The visualization depends on reliable serial communication between the Arduino and computer.

## Future Improvements

Possible improvements include:

* Adding multiple sensors
* Improving the visualization interface
* Adding object tracking
* Recording detection data
* Adding a web-based monitoring dashboard
* Improving sensor positioning and scanning speed
* Integrating the system with a robotic platform
* Adding alerts when objects enter a defined detection zone

## Project Type

**BSc Group Project**

This project was developed as a collaborative academic project to explore Arduino-based sensing, embedded systems, servo control, and real-time data visualization.

## Demo and Documentation

The repository contains:

* Project documentation in PDF format
* Project images
* A demonstration video

See the files above for additional project details and demonstration material.

## License

This project is intended for educational and academic purposes.
