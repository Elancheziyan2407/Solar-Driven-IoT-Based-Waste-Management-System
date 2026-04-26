  # 🌞 Solar-Driven IoT-Based Waste Management System (ESP32)

## 📌 Overview

The **Solar-Driven IoT-Based Waste Management System** is a smart solution designed to improve waste collection efficiency using renewable energy and real-time monitoring. The system uses an **ESP32 microcontroller**, sensors, and cloud integration to monitor dustbin status, battery performance, and environmental conditions.

This project aims to reduce manual intervention, optimize waste collection routes, and promote sustainable energy usage through solar power.

---

## 🎯 Objectives

* Enable real-time monitoring of waste levels
* Automate dustbin lid operation
* Utilize solar energy for sustainable operation
* Monitor battery health (voltage & current)
* Send data to cloud for remote access and analysis

---

## ⚙️ System Features

* 📡 IoT-based real-time monitoring using ThingSpeak
* 🌞 Solar-powered system with lithium-ion battery backup
* 🗑️ Automatic lid opening using servo motor
* 📶 GSM module for communication
* 📊 Waste level detection using ultrasonic sensor
* 💧 Moisture detection for wet/dry waste indication
* 🔋 Battery monitoring (voltage & current display on LCD)

---

## 🧩 Components Used

* ESP32 Microcontroller
* GSM Module
* Ultrasonic Sensor
* Moisture Sensor
* Servo Motor
* LCD Display
* Lithium-Ion Battery
* Solar Panel
* Voltage/Current Sensor (e.g., INA219)
* Connecting wires, resistors, etc.

---

## 🏗️ System Architecture

1. Sensors collect data (waste level, moisture)
2. ESP32 processes the data
3. Servo motor controls lid opening
4. Battery parameters are monitored and displayed on LCD
5. Data is sent to ThingSpeak via GSM/WiFi
6. Users can monitor system remotely

---

## 🔌 Circuit Diagram

📷 Refer to: `docs/circuit_diagram.png`

---

## 🔄 Workflow

1. Ultrasonic sensor measures waste level
2. Moisture sensor detects wet/dry waste
3. If user approaches → servo motor opens lid
4. Solar panel charges battery continuously
5. Battery voltage & current shown on LCD
6. Data uploaded to ThingSpeak cloud
7. Authorities can monitor bin status remotely

---

## ☁️ Cloud Integration (ThingSpeak)

* Platform: ThingSpeak
* Data Uploaded:

  * Waste Level (%)
  * Moisture Status
  * Battery Voltage
  * Battery Current

📊 Graphs can be viewed in real-time via ThingSpeak dashboard.

---

## 🧪 Testing

Testing modules included:

* Sensor accuracy testing
* GSM communication testing
* Battery monitoring validation
* Servo motor response testing

Refer: `tests/`

---

## 📊 Sample Data

Sample datasets available in:

```
data/
```

---

## 📷 Project Images

| Prototype                          | Setup                      | Results                              |
| ---------------------------------- | -------------------------- | ------------------------------------ |
| ![Prototype](images/prototype.jpg) | ![Setup](images/setup.jpg) | ![Results](images/results_graph.png) |

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```
git clone https://github.com/your-username/solar-iot-smart-waste-management-esp32.git
cd solar-iot-smart-waste-management-esp32
```

### 2. Upload Firmware

* Open `firmware/main/main.ino` in Arduino IDE
* Install required libraries:

  * WiFi
  * ThingSpeak
  * Servo
  * LiquidCrystal
* Select ESP32 board
* Upload code

### 3. Configure Settings

Update in `config.h`:

* WiFi credentials
* ThingSpeak API key
* GSM settings

---

## 📈 Results

* Real-time monitoring achieved
* Efficient waste level detection
* Stable solar charging observed
* Reduced manual inspection effort

---

## 🔮 Future Enhancements

* Mobile application for monitoring
* AI-based waste prediction
* GPS tracking for smart collection routing
* Integration with smart city systems

---

