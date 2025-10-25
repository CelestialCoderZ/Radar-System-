# ARDUINO RADAR SYSTEM 
A real-time radar system using Arduino, ultrasonic sensor, and servo motor with Processing IDE visualization.

## 🎯 Overview
This project creates a functional radar system that scans the environment using an ultrasonic sensor mounted on a servo motor. The system detects objects in real-time and displays the results on a computer screen using Processing IDE for visualization.

## 🚀 Features

- **Real-time Object Detection** - Scans 15° to 165° range
- **Distance Measurement** - Accurate detection from 2cm to 200cm
- **Visual Radar Display** - Professional radar interface
- **Serial Communication** - Real-time data transmission
- **Object Tracking** - Multiple object detection and display

## 🛠️ Hardware Components

| Component | Quantity | Specification |
|-----------|---------------|---------------|
| Arduino Uno | 1 | Microcontroller |
| HC-SR04 Ultrasonic Sensor | 1 | Distance Measurement |
| SG90 Servo Motor | 1 | 180° rotation |
| Jumper Wires | 7 | Connections |

## 📋 Performance Specifications

| Parameter | Specification |
|-----------|---------------|
| Scanning Angle | 15° to 165° (150° total sweep) |
| Angular Resolution | 1° per step |
| Distance Range | 2cm to 400cm (theoretical) |
| Effective Range | 2cm to 200cm (practical) |
| Scan Speed | 30ms per degree |
| Full Scan Time | ~9 seconds (150° × 30ms × 2 directions)|
| Distance Accuracy | ±3mm (theoretical), ±1cm (practical) |
| Object Size Detection | Minimum 2cm diameter |

## 🔌 Circuit Connection


| ULTRASONIC SENSOR | ARDUINO UNO |
|-----------|---------------|
| VCC | 5V |
| GND | GND |
| TRIG | D10 |
| ECHO | D11 |

| SERVO MOTOR | ARDUINO UNO |
|-----------|---------------|
| VCC | 5V |
| GND | GND |
| SIG | D12 |


## ⚡ Quick Start
    1. Clone the repository:
       git clone https://github.com/yourusername/Radar-System.git
       cd Radar-System

    2. Installation:
      - Download Processing from "processing.org"
      


##  🚀 Usage
    Step 1: Hardware Assembly
     (i)   Connect components as per circuit diagram
     (ii)  Ensure stable power supply
     (iii) Position ultrasonic sensor on servo horn

    Step 2: Upload Arduino Code
      (i)   Open Arduino IDE
      (ii)  Upload the radar code
      (iii) Keep serial monitor closed

    Step 3: Run Visualization
      (i)   Open Processing IDE
      (ii)  Paste visualization code
      (iii) Update serial port:
                           java 
         myPort = new Serial(this,"COM3", 9600); // Windows
                            or
         myPort = new Serial(this, "/dev/ttyUSB0", 9600);
      (iv)  Run the sketch

    Step 4: Monitor Radar
      (i)   Green arcs represent distance circles
      (ii)  Red dots show detected objects
      (iii) Angle lines indicate scanning directions
      (iv)  Real-time data display

## 🖥️ Expected Output
   - Radar Sweep: Green line rotating 15°-165°
   - Object Detection: Red dots at detected positions
   - Distance Circles: 10cm, 20cm, 30cm, 40cm markers
   - Angle Indicators: 30°, 60°, 90°, 120°, 150°

## 🔧Troubleshooting
    Common Issues:
    1. No Serial Data
      - Check Arduino-TX to Computer-RX connection
      - Verify baud rate (9600)
      - Ensure only one program accesses serial port

    2. Servo Not Moving
      - Check power supply (5V)
      - Verify signal pin connection
      - Ensure servo library is included

    3. No Object Detection
      - Check ultrasonic sensor connections
      - Ensure clear line of sight
      - Test sensor with basic example

    4. Processing Sketch Not Working
      - Update serial port name
      - Check Processing Serial library
      - Verify data format from Arduino

    Serial Port Configuration:
      - Windows: COM3, COM4, etc.
      - Linux: /dev/ttyUSB0, /dev/ttyACM0
      - Mac: /dev/tty.usbmodem1411

## 🚀 Future Enhancements
   - Add LCD display for standalone operation
   - Implement buzzer alerts for close objects
   - Add data logging to SD card
   - Create web interface with ESP32
   - Multiple sensor integration
   - Object tracking algorithms 


## 🤝 Contributing

Contributions are welcome! Here are ways you can help:

### 🐛 Reporting Bugs
- Open an issue with detailed description
- Include steps to reproduce
- Add relevant code/screenshots

### 💡 Suggesting Enhancements
- Describe the new feature
- Explain the use case
- Consider implementation approach

### 🔧 Code Contributions
    1. Fork the repository
    2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
    3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
    4. Push to the branch (`git push origin feature/AmazingFeature`)
    5. Open a Pull Request

## 🙏 Acknowledgments
     
- Arduino Community for continuous support
- Processing IDE for visualization capabilities
- Open-source hardware and software contributors


## 📞 Contact Me
If you have any questions, suggestions, or feedback, feel free to reach out:

 - **Name**: Anuprabha Bag
 - **Email**: [anuprabhabag2004ind@gmail.com]
 - **LinkedIn**: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/anuprabha-bag-b98359260/) 
 - **GitHub**: [github.com/yourusername](https://github.com/CelestialCoderZ)  
💡 I’d love to connect and collaborate on exciting projects!

<div align="center">
⭐ If you find this project helpful, please give it a star!
"Seeing the Unseen - Radar Technology in Action" 🛰️

</div>

