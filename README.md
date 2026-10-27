# Cloud-Connected Security Node using ESP32 and IoT Telemetry

## 📌 Project Overview
The Cloud-Connected Security Node is an IoT-based security monitoring system developed using an ESP32 microcontroller and an HC-SR04 ultrasonic distance sensor. It measures the distance of nearby objects, activates a buzzer when an object comes within a predefined threshold, and sends sensor readings to the Adafruit IO cloud dashboard using MQTT.

## 🎯 Objectives
- Measure object distance using an ultrasonic sensor.
- Generate an audible alert when an object comes within 50 cm.
- Connect the ESP32 to Wi-Fi.
- Publish sensor data to a cloud dashboard using MQTT.
- Monitor distance readings remotely through Adafruit IO.

## 🛠️ Components and Technologies
- ESP32 DevKit
- HC-SR04 Ultrasonic Distance Sensor
- Buzzer
- Wokwi Simulator
- Adafruit IO Cloud Dashboard
- MQTT Protocol
- Arduino C++

## 🔌 Pin Connections

| Component | ESP32 Pin |
|---|---|
| HC-SR04 VCC | VIN |
| HC-SR04 GND | GND |
| HC-SR04 TRIG | GPIO 4 |
| HC-SR04 ECHO | GPIO 18 |
| Buzzer Positive (+) | GPIO 19 |
| Buzzer Negative (-) | GND |

## ⚙️ Working Principle
1. The HC-SR04 sensor measures the distance to a nearby object.
2. The ESP32 processes the distance measurement.
3. If the distance is below 50 cm, the buzzer generates an alert.
4. The ESP32 connects to Wi-Fi and publishes distance readings using MQTT.
5. The Adafruit IO dashboard displays the received sensor data.

## ☁️ Cloud Integration
Adafruit IO is used to receive and display sensor readings through an MQTT feed named `distance`.

## 🧪 Simulation and Testing
The project was simulated using Wokwi. The Serial Monitor displayed distance readings, object status, Wi-Fi connection status, and cloud publishing status.

## 🔐 Security Note
Adafruit IO credentials are private and must not be committed to a public repository. Replace credential placeholders with your own credentials only in your local simulation code.

## 🚀 Future Enhancements
- Add remote notifications for nearby objects.
- Store and analyze historical sensor readings.
- Add configurable distance thresholds.
- Extend the system with additional security sensors.

## 👩‍💻 Project Platform
- Simulation: Wokwi
- Cloud Dashboard: Adafruit IO
- Repository: GitHub
