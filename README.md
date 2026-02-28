**Arduino Ultrasonic Radar System
Overview**

This project is an Arduino-based radar system using an ultrasonic sensor mounted on a servo motor. The system operates in both automatic sweep mode and manual joystick control mode, displaying obstacle positions on an OLED screen and transmitting data to a Processing-based GUI.

**Features**

    Automatic sweep scanning (15°–165°)
    
    Manual joystick-controlled scanning
    
    Real-time distance measurement (HC-SR04)
    
    OLED radar visualization (SSD1306)
    
    Obstacle alert using LED indicators
    
    Serial data transmission for PC visualization

**Hardware Components**

    Arduino Nano
    
    HC-SR04 Ultrasonic Sensor
    
    SG90 Servo Motor
    
    SSD1306 128x64 OLED Display
    
    Joystick Module
    
    Red and Green LEDs
    
    Jumper wires and breadboard
    
**Pin Configuration**
    
    Ultrasonic Sensor
    Trig → D7
    Echo → D9
    
    Servo
    Signal → D10
    
    LEDs
    Green → D5
    Red → D3
    
    Joystick
    VRx → A0
    Switch → D12
    
    OLED
    SDA → A4
    SCL → A5

**Working Principle**

The ultrasonic sensor emits a sound pulse and measures the echo return time. Distance is calculated using time-of-flight principles:

Distance = (Time × Speed of Sound) / 2

The servo rotates between 15° and 165° in automatic mode. In manual mode, joystick input maps directly to servo angle. The OLED renders a semicircular radar grid and plots detected obstacles based on angle and scaled distance.

**Applications**

Obstacle detection systems

Basic robotic perception models

Educational radar visualization

Autonomous vehicle concept prototypes

**Future Improvements**

Add filtering for noisy distance readings

Integrate Kalman filtering

Add Bluetooth or WiFi streaming

Replace ultrasonic with LiDAR module

Implement object tracking algorithm

**Author**

Auren
B.Tech Mechanical Engineering (Design & Manufacturing)
