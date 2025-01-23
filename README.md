# IoT-Based Smart Agriculture System

## Description
This project leverages IoT to monitor temperature, humidity, and soil moisture in agricultural fields using sensors like DHT11 and YL-69. It automates irrigation by turning motors ON/OFF based on soil moisture. Real-time data visualization is achieved via ThingsBoard.

## Features
- Monitors temperature, humidity, and soil moisture.
- Automates irrigation using relay and motor control.
- Publishes and subscribes to data via MQTT protocol.
- Real-time data visualization using ThingsBoard.

## Modules
### Module 1
- ESP8266 WiFi module with DHT11 sensor for temperature and humidity.
- Data is published to the MQTT broker.

### Module 2
- Arduino Uno with YL-69 sensor to measure soil moisture.
- Data is published to the MQTT broker.

### Module 3
- ESP8266 as a subscriber that controls the motor via a relay.

## Components Used
- **ESP8266 ESP-01**
- **DHT11 Sensor**
- **YL-69 Soil Moisture Sensor**
- **Arduino Uno**
- **Relay (2 Channel)**
- **Raspberry Pi (MQTT Broker)**

## Wiring
![Wiring Diagram for Module 1](Schematics/wiring_diagram_module1.png)
![Wiring Diagram for Module 2](Schematics/wiring_diagram_module2.png)
![Wiring Diagram for Module 3](Schematics/wiring_diagram_module3.png)

## Real-Time Visualization
Data is visualized on ThingsBoard. Access the dashboard [here](https://your-thingsboard-dashboard-link).

## Installation
- Clone the repository: `git clone https://github.com/gdsneha/IoT-Smart-Agriculture-System.git`
- Follow the wiring diagrams for each module.
- Configure MQTT settings in `iot_config.h`.
- Upload the respective codes to ESP8266 and Arduino.
- Run the Python scripts for ThingsBoard visualization.

## Contributors
- Sneha G D ([GitHub Profile](https://github.com/gdsneha))
