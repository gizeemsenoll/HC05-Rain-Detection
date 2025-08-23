# 🌧️ HC05 Rain Detection

## 📌 Project Description

In this project, a rain sensor with an analog output is used to detect whether it is raining in the environment. The status information is wirelessly transmitted to a mobile phone via the **HC-05 Bluetooth module**. At the same time, an audible warning is given with a **buzzer**. The sensor values are analyzed so that alerts are only triggered under specific conditions.

## 🎯 Project Purpose

To warn the user both audibly and wirelessly (via Bluetooth) when rain is detected outdoors.
This project was carried out **under the guidance of the IT supervisor during my internship**, and it provided valuable experience in sensor usage and data analysis.

## 🔌 Components Used

* Arduino UNO
* HC-05 Bluetooth module
* Rain sensor (analog output)
* Buzzer
* Jumper wires
* Breadboard

## 📲 Application Used

To read the Bluetooth data, the **Serial Bluetooth Terminal** application was installed on an Android phone. The data sent from the Arduino was monitored in real time through this application.

## ⚙️ System Operation

1. The analog values from the rain sensor are read by the Arduino.
2. The rate of change in the values is evaluated at certain intervals.
3. If sudden and significant increases are detected and the values exceed a specific threshold (e.g., 500):

   * The buzzer is activated
   * A **“Rain detected”** message is sent to the mobile phone via the HC-05 module.
4. When the rain stops, the buzzer turns off and the updated status is transmitted to the phone application.

## 🖥️ Code

* Project codes are located in the `code/rain_detection.ino` file.

## 📷 Images

* Circuit diagram
* Screenshots from the Serial Bluetooth Terminal application
* Project photos are available in the `images` folder.

## 🔍 Observations

* Real-time outdoor rain detection was successfully achieved.
* Since the system only reacts to meaningful changes, false alarms were prevented.

✍️ **Prepared by:** Gizem Şenol
📅 **Year:** 2025

