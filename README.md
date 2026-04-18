# Learning With AI

## Overview
This repository documents how AI tools were used to support the development of a lizard habitat monitoring system. The focus was on learning both the **software** and **hardware** aspects required to collect, process, and interpret environmental and behavioral data.

AI was used as a tool for:
- Writing and debugging code  
- Understanding hardware setup and communication  
- Troubleshooting issues during development  
- Accelerating learning in unfamiliar areas  

---

## Software Domain

### What I Learned
Through this project, I learned how to:
- Read and process **sensor data (temperature and humidity)**  
- Structure Arduino programs for continuous data collection  
- Format and transmit data between devices (UART communication)  
- Generate meaningful outputs (e.g., email reports)  
- Debug issues in embedded systems code  

### Why This Was Necessary
The system depends on accurately interpreting environmental data and combining it with behavioral data from the camera. Without proper data handling, the system would not be able to identify meaningful patterns or generate useful reports.

### How AI Helped
AI played a major role in software development by:
- Helping structure Arduino code for both the ESP32-C6 and ESP32-CAM  
- Assisting with implementing **frame differencing** for motion detection  
- Debugging issues in Wi-Fi connectivity and email functionality  
- Explaining how to use libraries such as:
  - `Adafruit_AHTX0`
  - `ESP_Mail_Client`
  - `esp_camera`  
- Rebuilding lost code for the ESP32-CAM and ensuring it matched expected output formats  

### Key Takeaway
AI significantly accelerated development, but required validation. I learned to test outputs carefully and not rely on AI blindly.

---

## Hardware Domain

### What I Learned
Through this project, I learned how to:
- Wire and integrate multiple components:
  - ESP32-C6  
  - ESP32-CAM  
  - AHT10 sensor  
- Use a breadboard for prototyping  
- Establish **UART communication** between two microcontrollers  
- Properly power and configure embedded devices  
- Flash code onto the ESP32-CAM using a USB-to-TTL adapter  

### Why This Was Necessary
The system relies on multiple devices working together:
- The ESP32-CAM detects motion and position  
- The ESP32-C6 processes sensor data and sends reports  

Without proper hardware setup and communication, the system would not function.

### How AI Helped
AI assisted with:
- Understanding wiring and hardware connections  
- Explaining how to safely connect components and avoid issues (e.g., risky pins like IO12)  
- Guiding the flashing process for the ESP32-CAM, which is more complex than standard boards  
- Helping debug communication issues between the two boards  
- Suggesting design improvements (e.g., removing the unnecessary Arduino Nano)  

### Key Takeaway
AI was especially useful for hardware learning, but required cross-checking with real-world testing since hardware issues are not always obvious from code alone.

---

## Challenges and Limitations of AI

- AI sometimes produced **confident but incorrect information**  
- Small mistakes in code (e.g., naming errors) required debugging  
- Hardware issues still required **manual testing and iteration**  

### Strategy Moving Forward
- Use AI for **specific, targeted questions**  
- Validate results through testing  
- Use external resources (documentation, videos) when needed  

---

## Conclusion

AI was a valuable tool throughout this project, helping bridge gaps in both software and hardware knowledge. It allowed faster iteration and problem-solving, but success depended on actively verifying and understanding the solutions provided.

This project demonstrates how AI can be effectively used as a **learning and development assistant**, rather than a replacement for critical thinking.
