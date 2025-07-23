# Cosmin Ilea - Portfolio

Welcome to my online portfolio! This page serves as a showcase of my academic and personal projects, focused on automation, IoT (Internet of Things), embedded systems, and infrastructure management.

## Projects

### 1. Smart Knob in Building Automation Applications (Bachelor Thesis)

[cite_start]This was my bachelor's thesis project at the Technical University of Cluj-Napoca, where I designed, built, and validated a centralized controller for a smart home[cite: 202, 280]. [cite_start]The objective was to simplify the interaction with smart devices by offering a physical, tactile interface that eliminates the need for multiple mobile applications[cite: 203, 237, 283].

**Key Contributions and Technologies:**

* [cite_start]**Mechanical Design:** I created a custom, 3D-printed enclosure that allowed the display's cable to pass through the hollow shaft of the motor, ensuring 360-degree rotation without the risk of entanglement[cite: 248, 1050].
* [cite_start]**Haptic Feedback:** I implemented an advanced haptic feedback system using a **Brushless DC (BLDC)** motor and the **Field-Oriented Control (FOC)** technique[cite: 242, 273, 288]. [cite_start]This allowed for the creation of unique physical sensations, such as discrete detents for fan speed control and spring-like end-stops for adjusting volume or temperature[cite: 242, 288, 1375].
* [cite_start]**Real-Time Firmware:** The firmware was developed in C++ on an **ESP32** microcontroller with a dual-core architecture[cite: 248, 316, 839]. [cite_start]I used FreeRTOS to separate the time-critical motor control logic from other tasks (like communication and display updates), ensuring instant and uninterrupted haptic feedback[cite: 843, 855, 1390].
* [cite_start]**Smart Home Integration:** The device communicates with the **Home Assistant** platform using the **MQTT** protocol[cite: 243, 291]. [cite_start]I configured `MQTT sensors` and `automations` in Home Assistant to translate physical interactions (rotation, press) into commands for various devices, such as lights and media players[cite: 245, 1378].

### 2. Home Lab Infrastructure Management

[cite_start]I built and manage a personal server (`home lab`) on an HP ProDesk 600 G2 mini PC[cite: 1789]. It runs **Ubuntu Server** and hosts a variety of services via **Docker** and **Portainer**, demonstrating practical skills in system administration and infrastructure management.

**Technical Details and Applications:**

* [cite_start]**Containerization:** I implemented a **Docker** runtime environment, managing services like **Home Assistant**, **Nextcloud** (a self-hosted file storage service), and a **MariaDB** database, all running in containers[cite: 1799].
* **Secure Networking:** Remote access to the server is achieved via **SSH** and a **Tailscale VPN**, ensuring a secure connection without exposing public services to the internet.
* [cite_start]**Automation and Monitoring:** I configured an automated watchdog to restart network services in case of connectivity loss, ensuring continuous availability[cite: 1819]. I also use **Cockpit** for monitoring resources (CPU, storage).

### 3. SmartBreeze: IR Air Conditioner Control

[cite_start]This IoT project was designed to remotely control an infrared (IR) air conditioner using an Android mobile application and an **ESP32** microcontroller[cite: 15, 22]. [cite_start]The system mimics the functions of a traditional remote control (power toggle, temperature adjustment, fan speed control) through a wireless connection over Wi-Fi[cite: 16, 24].

**Technologies and Implementation:**

* [cite_start]**Platforms:** The Android application was developed with **Kotlin** and **Jetpack Compose**[cite: 21, 27]. [cite_start]The firmware for the **ESP32** was written in **C++** using the Arduino Framework[cite: 22, 28].
* [cite_start]**Communication:** Interaction between the mobile app and the ESP32 is done via a **WebSocket** connection on a local Wi-Fi network[cite: 24, 29, 76].
* [cite_start]**Functionality:** The ESP32 receives commands from the app, parses them, and sends the corresponding IR signals to the air conditioner unit[cite: 25, 110].

---

**Note:** For more details on my projects, I invite you to explore the official documents (bachelor's theses, technical documentation) included in this repository, as well as my LinkedIn and GitHub profiles.

* [LinkedIn](https://www.linkedin.com/in/cosmin.ilea)
* [GitHub](https://github.com/ileacosmin)
