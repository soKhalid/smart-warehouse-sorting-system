# Smart Warehouse Sorting System: AI-Powered Automation Solution

<p align="center">
  <img src="docs/system_overview.png" alt="Smart Warehouse Sorting System" width="800"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white" alt="Arduino"/>
  <img src="https://img.shields.io/badge/AI-Computer%20Vision-blue?style=for-the-badge" alt="AI"/>
  <img src="https://img.shields.io/badge/IoT-Blynk-green?style=for-the-badge" alt="IoT"/>
  <img src="https://img.shields.io/badge/Accuracy-95.5%25-brightgreen?style=for-the-badge" alt="Accuracy"/>
</p>

## 🎯 Project Overview

An intelligent warehouse sorting system that integrates artificial intelligence, robotics, and IoT technologies to automate object classification and sorting operations. Developed as a capstone project at **The British University in Dubai**, this system demonstrates how accessible embedded platforms can deliver professional-grade automation capabilities.

### 🏆 **Key Achievements**
- **95.5%** AI classification accuracy
- **93.8%** overall sorting success rate  
- **98.2%** system uptime during extended operation
- **73%** cost reduction vs. manual operations
- **±2.1mm** robotic arm positioning precision

## ✨ Key Features

🤖 **AI-Powered Classification**: HuskyLens camera with innovative 5-pass majority voting algorithm  
🦾 **Precision Robotics**: 6-DOF servo-based arm with industrial-grade accuracy  
📱 **Real-Time IoT Monitoring**: Live dashboard with instant alerts via Blynk  
⚡ **Dual-Board Architecture**: Innovative voltage domain separation for reliable operation  
💰 **Cost-Effective**: Professional performance using accessible components  
🔧 **Modular Design**: Scalable architecture supporting future expansion  

## 🛠️ Technology Stack

| Component | Technology | Purpose | Performance |
|-----------|------------|---------|-------------|
| **Main Controller** | Arduino UNO WiFi Rev2 | System coordination, AI interface | WiFi + 20 I/O pins |
| **Arm Controller** | Arduino UNO R3 | Dedicated robotic arm control | 5V logic, servo control |
| **AI Vision** | HuskyLens | Object classification | 95.5% accuracy |
| **Robotics** | LewanSoul xArm (6-DOF) | Physical sorting | ±2.1mm precision |
| **IoT Platform** | Blynk | Real-time monitoring | 1.2s response time |
| **Motor Control** | NEMA 17 + TB6560 Driver | Precision conveyor | 98.5% positioning |
| **Sensors** | HC-SR04 Ultrasonic | Object detection | ±2mm accuracy |

## 🏗️ System Architecture
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Object        │    │  AI              │    │  Robotic        │
│   Detection     │───▶│  Classification  │───▶│  Sorting        │
│   (Ultrasonic)  │    │  (HuskyLens)     │    │  (xArm 6-DOF)   │
└─────────────────┘    └──────────────────┘    └─────────────────┘
│                       │                       │
▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Stepper       │    │  Dual Arduino    │    │  IoT            │
│   Conveyor      │    │  Architecture    │    │  Monitoring     │
│   Control       │    │  (Main + Arm)    │    │  (Blynk)        │
└─────────────────┘    └──────────────────┘    └─────────────────┘
## 📊 Performance Metrics

| Metric | Target | Achieved | Status |
|--------|--------|----------|--------|
| **Classification Accuracy** | >90% | **95.5%** | ✅ **Exceeds** |
| **Sorting Success Rate** | >85% | **93.8%** | ✅ **Exceeds** |
| **System Uptime** | >90% | **98.2%** | ✅ **Exceeds** |
| **IoT Response Time** | <2 seconds | **1.2 seconds** | ✅ **Meets** |
| **Processing Speed** | Competitive | **4.2 objects/min** | ✅ **Meets** |

## 👥 Team & Contributions

| Team Member | Role | Key Innovations |
|-------------|------|-----------------|
| **🤖 Khalid Alshehhi** | Robotics Specialist | 2-month systematic calibration achieving ±2.1mm precision |
| **🧠 Ahmed Lootah** | AI & IoT Expert | 5-pass majority voting algorithm, 95.5% accuracy |
| **🏗️ Dhaen Alqubaisi** | System Architect | Dual-board architecture, complete system integration |
| **⚡ Yousif Bineshaq** | Electrical Engineer | Power distribution, 98.5% conveyor positioning |
| **📊 Suhail Alawadhi** | Project Leader | Strategic vision, comprehensive testing protocols |
| **💻 Anfal Alhammadi** | Software Developer | Conveyor algorithms, technical documentation |

## 🚀 Quick Start Guide

### Prerequisites
```bash
# Required Software
- Arduino IDE 2.0+
- Blynk IoT App

# Required Libraries
- BlynkSimpleWiFiNINA
- HUSKYLENS
- AccelStepper  
- xArmServoController
- Ultrasonic
```
Installation Steps

Clone the repository

bashgit clone https://github.com/yourusername/smart-warehouse-sorting-system.git
cd smart-warehouse-sorting-system

Hardware Setup

Follow wiring diagram in /hardware/wiring_diagrams/
Ensure proper 12V→5V voltage regulation
Mount all components according to mechanical drawings


Software Configuration

cpp// Update WiFi credentials in src/main_controller/main_arduino_code.ino
char ssid[] = "your_wifi_network";
char pass[] = "your_wifi_password";

// Update Blynk authentication token
#define BLYNK_AUTH_TOKEN "your_blynk_token_here"

Upload Code

Upload src/main_controller/main_arduino_code.ino to Arduino UNO WiFi Rev2
Upload src/arm_controller/arm_arduino_code.ino to Arduino UNO


Configure Blynk App

Create new project with provided template
Add virtual pins: V0 (Electronics), V1 (Furniture), V2 (Makeup)



📈 Results & Testing
Classification Performance

Electronics: 96% accuracy (25 test objects)
Furniture: 94% accuracy (22 test objects)
Makeup: 95% accuracy (20 test objects)

Robotic Arm Performance

Positioning Accuracy: ±2.1mm average
Success Rate: 98.2% across all categories
Cycle Time: 8.0 seconds average

System Reliability

8-Hour Continuous Test: 95.2% success rate
200-Cycle Integration Test: 94.5% overall success
Network Uptime: 98.2% IoT connectivity

🔮 Future Development Roadmap
Immediate Enhancements (0-6 months)

 Startup signal bug fix with pull-down resistors
 30-40% speed optimization through parallel processing
 Environmental robustness with adaptive lighting control

Advanced Features (6-18 months)

 Multi-arm coordination for increased throughput
 Custom neural networks replacing HuskyLens
 Quality assessment capabilities
 5-7 object category expansion

Enterprise Integration (18+ months)

 ERP system connectivity
 Professional industrial packaging
 API development for third-party integration
 Predictive maintenance capabilities

📚 Documentation

📖 Complete Capstone Report - Comprehensive technical documentation
🔧 Hardware Setup Guide - Component list and assembly instructions
💻 Software Documentation - Code structure and algorithms
📊 Test Results - Detailed performance analysis
🎤 Final Presentation - Project overview slides

🎓 Academic Context
Institution: The British University in Dubai
Department: Computer Science & Artificial Intelligence
Course: AI Capstone Project (CSAI405)
Supervisor: Prof. Piyush Maheshwari
Academic Year: 2024-2025
Submission Date: June 25, 2025
🏆 Project Impact
This project demonstrates that sophisticated warehouse automation can be achieved using accessible embedded systems, potentially democratizing automation technology for small-to-medium enterprises and educational institutions worldwide.
Commercial Viability

Target Market: Small warehouses, educational institutions, research facilities
Cost Advantage: 25-100x cheaper than traditional commercial systems
Scalability: Modular design supports incremental expansion

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
🤝 Contributing
We welcome contributions from the community! Please read our Contributing Guidelines before submitting pull requests.
📞 Contact & Support
For questions, collaboration opportunities, or technical support:

📧 Project Team: [Create team email or individual contacts]
🎓 Institution: The British University in Dubai
📋 Issues: Use GitHub Issues for bug reports and feature requests


<p align="center">
  <strong>⭐ Star this repository if you found it helpful! ⭐</strong>
</p>
<p align="center">
  <em>Bridging the gap between educational projects and industrial automation</em>
</p>
```
