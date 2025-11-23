# 🌡️ Digital Thermometer with Humidity Monitoring (Arduino)

A simple IoT project for environmental monitoring, developed using the Arduino platform. The system reads temperature and humidity in real-time and displays the data on both an LCD screen and the Serial console.

## 📝 Description
This project uses a **DHT11** sensor for data acquisition and a **1602 LCD with I2C interface** for displaying results. The code includes software calibration features for the sensors and read error handling.

## 🛠️ Hardware Requirements
* Development board (e.g., Arduino Uno/Nano)
* Temperature and humidity sensor **DHT11** 
* 1602 LCD Display with **I2C** module 
* Jumper wires

## 💻 Software Dependencies (Libraries)
To compile this project, the following libraries must be installed in the Arduino IDE:
1.  **LiquidCrystal_I2C** (for the LCD screen, address `0x27`) 
2.  **DHT Sensor Library** (for the DHT11 sensor)
3.  **Wire** (standard inclusion for I2C protocol) 

## ⚙️ Key Features
* **Dual Display:** Data is visible on the LCD (for the user) and in the Serial Monitor (for debugging/logging).
* **Software Calibration:** The code includes an offset correction for the specific sensors used (`+21.9°C` temperature, `+50.2%` humidity).
* **Error Handling:** The system detects if the sensor is not responding (`NaN`) and displays the message "Sensor Error / Check DHT11" on the screen.
* **Custom Interface:** Displays user names ("Costi & Bia") on the first row. 

## 🚀 Installation and Usage
1.  Connect the components according to the pinout.
2.  Open the `.ino` file in Arduino IDE.
3.  Install the necessary libraries from the *Library Manager*.
4.  Upload the code to the board.

---
*Project developed at the Faculty of Cybernetics, Statistics and Economic Informatics.*
