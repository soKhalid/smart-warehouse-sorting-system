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
