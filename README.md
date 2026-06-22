# AI-Powered Smart Doorbell Security System

## Overview

The AI-Powered Smart Doorbell Security System is an IoT-based home security solution designed to enhance visitor monitoring and access control. The system uses an ESP32-CAM module to capture visitor images, authenticate authorized family members, and automatically control door access.

When a visitor presses the doorbell, the camera captures an image and performs authentication. Authorized visitors are granted access, while unauthorized visitors trigger an alarm and notification mechanism.

---

## Features

* Real-time visitor image capture using ESP32-CAM
* Image-based authentication of authorized family members
* Automatic door unlocking for verified users
* Intrusion detection for unauthorized visitors
* Buzzer-based alarm system
* Wireless notification support through Wi-Fi
* Visitor event logging and monitoring
* Low-cost IoT-based security solution

---

## System Architecture

Visitor → Doorbell Button → ESP32-CAM → Image Authentication

### Authorized Visitor

* Door Unlock
* Event Logged
* Notification Sent

### Unauthorized Visitor

* Alarm Triggered
* Notification Sent
* Event Logged

---

## Hardware Components

| Component          | Quantity    |
| ------------------ | ----------- |
| ESP32-CAM Module   | 1           |
| Relay Module       | 1           |
| Solenoid Door Lock | 1           |
| Buzzer             | 1           |
| Push Button        | 1           |
| Jumper Wires       | As Required |
| 5V Power Supply    | 1           |

---

## Software Requirements

* Arduino IDE
* ESP32 Board Package
* WiFi Library
* HTTPClient Library
* ESP32 Camera Library

---

## Pin Configuration

| Component       | ESP32-CAM Pin |
| --------------- | ------------- |
| Doorbell Button | GPIO12        |
| Relay Module    | GPIO13        |
| Buzzer          | GPIO14        |

---

## Working Principle

1. Visitor presses the doorbell button.
2. ESP32-CAM captures the visitor image.
3. The authentication module compares the visitor image with stored authorized profiles.
4. If the visitor is recognized:

   * Door lock is activated.
   * Access is granted.
   * Notification is sent.
5. If the visitor is not recognized:

   * Alarm buzzer is activated.
   * Unauthorized access alert is generated.
   * Notification is sent to the user.
6. Visitor details are logged for future reference.

---

## Project Workflow

1. Initialize camera and Wi-Fi connection.
2. Wait for doorbell press event.
3. Capture visitor image.
4. Perform authentication.
5. Grant or deny access.
6. Generate logs and notifications.

---

## Applications

* Smart Homes
* Residential Security Systems
* Apartment Access Control
* Visitor Monitoring Systems
* IoT-Based Security Solutions

---

## Future Enhancements

* Real face recognition using AI models
* Mobile application integration
* Cloud database storage
* Face mask detection
* Voice communication support
* Live video streaming
* OTP-based visitor verification

---

## Technologies Used

* Embedded Systems
* Internet of Things (IoT)
* ESP32-CAM
* Arduino IDE
* Wi-Fi Communication
* Image Processing
* Smart Security Systems

---

##
