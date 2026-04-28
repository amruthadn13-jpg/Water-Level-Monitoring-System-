# 💧 Water Level Monitoring System (ESP32 + Ultrasonic Sensor)

## 📌 Overview

This project is a **Water Level Monitoring System** built using **ESP32**, **Ultrasonic Sensor**, **LED indicators**, and a **Buzzer**.

It measures the distance between the sensor and water surface to determine whether the tank level is **Low, Medium, or High**, and provides visual and sound alerts accordingly.

---

## ⚙️ Features

* Ultrasonic-based water level detection
* Three-level indication (Low, Medium, High)
* LED indicators for each level
* Buzzer alert for high level
* Serial output for monitoring

---

## 🧠 Project Description

The system uses an **ultrasonic sensor** to calculate the distance of water from the sensor and determines the water level based on predefined thresholds.

---

### 🔹 Distance Measurement

* The trigger pin sends ultrasonic waves

* The echo pin receives the reflected signal

* The time taken is measured and converted into distance

* **Smaller distance → Higher water level**

* **Larger distance → Lower water level**

---

### 🔹 Water Level Logic

The water level is categorized into three stages:

* **Low Level (distance > 20 cm)**

  * Low LED turns ON
  * Buzzer OFF

* **Medium Level (distance < 10 cm)**

  * Medium LED turns ON
  * Buzzer OFF

* **High Level (between 10–20 cm)**

  * High LED turns ON
  * Buzzer ON (alert for near overflow)

---

### 🔹 LED Indication

Each LED represents a specific water level:

* Low → Low LED
* Medium → Medium LED
* High → High LED

---

### 🔹 Buzzer Alert

* The buzzer is activated when the water level is **high**
* Acts as a warning for overflow condition

---

### 🔹 Serial Monitoring

The system continuously prints:

* Measured distance (in cm)
* Water level status

This helps in real-time monitoring and debugging.

---

## 🔄 Working Flow

1. ESP32 triggers ultrasonic sensor
2. Sensor measures distance
3. Distance is converted to water level
4. Corresponding LED is activated
5. If water level is high:

   * Buzzer turns ON
6. Status is displayed on Serial Monitor

---

## 🧠 Learning Outcomes

* Interfacing ultrasonic sensors with ESP32
* Distance calculation using pulse timing
* Implementing conditional logic
* Using multiple output devices (LED + buzzer)
* Real-time monitoring using serial communication

---

## 🚀 Future Enhancements

* Automatic motor control (water pump ON/OFF)
* IoT monitoring via mobile/web
* LCD/OLED display integration
* SMS/Telegram alerts
* Smart home integration

---

## 👩‍💻 Author

**Amrutha D N**
