# 🌱 Smart Irrigation System for Optimal Crop Management

An IoT-based irrigation system using **NodeMCU**, **Firebase**, and **GSM** to automate crop watering based on real-time soil moisture levels. The system supports multiple irrigation modes, remote control via mobile app, and SMS alerts—aimed at reducing water usage and enhancing farm efficiency.

---

## 🚀 Key Features

- 📡 Real-time soil moisture monitoring (4 zones)
- 💧 Water tank level detection using ultrasonic sensor
- 🔄 Manual, Automatic, and Optimal irrigation modes
- ☁️ Firebase Realtime Database for remote access
- 📲 SMS alerts via SIM800L GSM module
- 📟 Local LCD display for live system status
- 📅 Scheduling based on last irrigation date
- 🌦️ Climate tips and fertilizer recommendations
- 📊 ThingSpeak data logging & visualization

---

## ⚙️ Setup Instructions

### 1. Flash the Arduino Code

- Upload `NodeMCU_1_MainController.ino` to the **main NodeMCU**.
- Upload `NodeMCU_2_GSM_LCD_Controller.ino` to the **secondary NodeMCU**.
- Update Wi-Fi, Firebase, and GSM details in the `.ino` files (look for `----------` comments).

### 2. Configure Firebase

- Set up a Firebase project and structure the DB as shown in `/Firebase_Config/firebase_structure.png`.
- Insert your API key and DB URL in both Arduino and mobile app files.

### 3. Import the Mobile App

- Open [MIT App Inventor](https://ai2.appinventor.mit.edu/).
- Import `Smart_Irrigation_System (2).aia`.
- Replace Firebase keys with your own.

### 4. Circuit & Power

- Connect all sensors and modules as per circuit diagram.
- Power up both NodeMCUs (USB/adapter).
- System boots and starts monitoring.

---

## 📦 Components Used

- NodeMCU (x2)
- SIM800L GSM module
- 4 Soil Moisture Sensors
- Ultrasonic sensor (for tank)
- 4-Channel Relay Module
- LCD Display (I2C)
- Firebase, ThingSpeak, MIT App Inventor

---
