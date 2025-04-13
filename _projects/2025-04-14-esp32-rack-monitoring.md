---
title: "ESP32 Rack Monitoring System"
date: 2025-04-14
layout: project
description: "A modular sensor setup using ESP32 for rack monitoring, including temperature, humidity, and smoke sensors."
tags: [hardware, IoT, ESP32, sensors]
image: "/assets/images/esp32-rack.jpg"
---

## Project Overview

This project aims to build an ESP32-based rack monitoring system that includes various sensors to monitor the environment of server racks. The system includes temperature, humidity, and smoke sensors, and it can send real-time data to a server for monitoring purposes.

### Components Used
- **ESP32**: The microcontroller that drives the system.
- **DHT22**: Temperature and humidity sensor.
- **MQ-2**: Smoke sensor for fire detection.
- **OLED Display**: Displays real-time sensor data.
- **Buzzer**: Provides an audible alert in case of an emergency.

### Project Features
- **Temperature & Humidity Monitoring**: Measures and logs the environmental conditions in the rack.
- **Smoke Detection**: Monitors smoke levels to detect potential fire hazards.
- **Alert System**: Sends alerts through a buzzer and OLED display when abnormal conditions are detected.
- **Node-RED Integration**: Uses Node-RED to visualize data and trigger notifications.

### Step-by-Step Guide
1. **Setup ESP32**: Install the necessary libraries and configure the ESP32.
2. **Wiring Sensors**: Connect the DHT22 and MQ-2 sensors to the ESP32.
3. **Coding**: Write the Arduino code to read sensor data and send it to a server or display.
4. **Integration with Node-RED**: Use Node-RED to visualize the data in real-time.

### Schematic Diagram
![Rack Schematic](https://example.com/assets/images/rack-schematic.jpg)

### Conclusion
The ESP32-based rack monitoring system provides a low-cost solution to monitor critical parameters in server racks. It helps prevent overheating, detects potential fire hazards, and ensures proper airflow in the environment.

---

For a complete step-by-step guide, please check the [full project documentation](https://example.com/projects/esp32-rack-monitoring).
