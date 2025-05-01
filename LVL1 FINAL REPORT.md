# MARVEL LEVEL 2 TASKS

---

## **TASK 1: Simon Says**
Simon Says is a simple electronic memory game: the user has to repeat a growing sequence of
colors. The sequence is displayed by lighting up the LEDs. Each color also has a
corresponding tone.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250427_204542.jpg?raw=true)


In each turn, the game will play the sequence, and then wait for the user to repeat
the sequence by pressing the buttons according to the color sequence. If the user
repeated the sequence correctly, the game will play a "leveling-up" sound, add a new
color at the end of the sequence, and move to the next turn.

The game continues until the user has made a mistake. Then a game over sound is
played, and the game restarts.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_Amx9fiMfHA?si=8rFLYoBAuXU5zV_o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)


---



## **TASK 2: Basics of MQTT protocol and other communication protocols**

🛰️ MQTT (Message Queuing Telemetry Transport) 
📌 Introduction
MQTT is a lightweight and efficient messaging protocol. It was originally designed for low-bandwidth, high-latency, or unreliable networks, making it ideal for Internet of Things (IoT) applications.

MQTT uses a publish-subscribe (pub/sub) messaging model, which is more efficient than traditional client-server communication, especially for resource-constrained devices like sensors, wearables, and embedded systems.

🔧 Key Components
Client: A device (e.g., sensor or application) that publishes or subscribes to messages.

Broker: A server that receives all messages from publishers and routes them to subscribers.

Topic: A string that defines where messages are sent and how they are filtered. Topics are hierarchical (e.g., home/livingroom/temperature).

🔄 How MQTT Works
A publisher sends a message to a specific topic.

The broker receives the message and forwards it to all subscribers of that topic.

Devices subscribe to specific topics to receive relevant data.

This decouples devices from one another, allowing for flexible and scalable communication.

| **No.** | **Protocol / Standard** | **Type / Layer** | **Key Features** | **Use Cases** |
|--------|-------------------------|------------------|------------------|----------------|
| 1 | **AMQP** (Advanced Message Queuing Protocol) | Messaging / Application Layer | Reliable, secure, supports asynchronous messaging; works across platforms and over unreliable networks. | Enterprise systems, cloud integration, finance, secure M2M communication. |
| 2 | **Bluetooth / BLE** (Bluetooth Low Energy) | Wireless / Physical & Data Link Layer | BLE is optimized for low power, short-range; standard Bluetooth is for higher data needs. | Wearables, smartwatches, health trackers, in-store navigation, smart home. |
| 3 | **Cellular (2G/3G/4G/5G)** | Wireless / Network Layer | Long-range, high-bandwidth; 5G offers low latency. | Vehicle telemetry, mobile IoT, asset tracking, remote monitoring. |
| 4 | **CoAP** (Constrained Application Protocol) | Application Layer | Lightweight, RESTful protocol; works with HTTP, based on UDP; good for constrained devices. | Smart agriculture, environmental sensors, remote device control. |
| 5 | **DDS** (Data Distribution Service) | Middleware / Application Layer | Real-time, low-latency, scalable pub-sub communication. | Aerospace, robotics, industrial control systems, defense. |
| 6 | **LoRa / LoRaWAN** | Wireless / Physical & Network Layer | Long-range, low-power, non-cellular; LoRaWAN enables cloud communication. | Smart agriculture, rural IoT, environmental monitoring, water management. |
| 7 | **LWM2M** (Lightweight M2M) | Device Management Protocol | Designed for constrained devices; supports remote management and firmware updates. | Metering, remote monitoring, IoT device lifecycle management. |
| 8 | **MQTT** (Message Queuing Telemetry Transport) | Messaging / Application Layer | Lightweight, publish-subscribe model, works on TCP/IP; supports QoS 0–2. Efficient on low bandwidth. | Smart homes, IoT sensors, industrial IoT, mobile apps, telemetry. |
| 9 | **Wi-Fi** | Wireless / Physical & Data Link Layer | High data rate, low latency; short to medium range; power-hungry. | Smart appliances, indoor surveillance, LAN-based IoT systems. |
| 10 | **XMPP** (Extensible Messaging and Presence Protocol) | Messaging / Application Layer | XML-based protocol for real-time structured communication. | Smart appliances, lightweight messaging systems, chat-enabled IoT. |
| 11 | **Zigbee** | Mesh Network / Physical & Data Link Layer | Low-power, short-range; self-healing mesh network; secure and reliable. | Home automation, lighting, HVAC, industrial monitoring. |
| 12 | **Z-Wave** | Mesh Network / Physical Layer | Proprietary low-power mesh; secure and scalable; operates on sub-GHz frequencies. | Home security systems, smart locks, smart energy products. |



---



## **TASK 3: Basics of Creating a Website**

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/colorweb.PNG?raw=true)


For this task, I learned how websites work from both the front-end and back-end. I made a simple webpage with a button that changes the background color through VIBGYOR colors when clicked. I used HTML for the structure, CSS for styling, and JavaScript to make the button work. It helped me understand how the front-end looks and feels, and how the back-end connects everything behind the scenes. This was a fun and helpful way to get started with web development.

<iframe width="560" height="315" src="https://www.youtube.com/embed/cvlxigZiR78?si=2RsKofGUCvDuK_Aw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 4:  ESP32 CAM-Based Surveillance Robot using Arduino IDE**
For this task, I built a surveillance robot using the ESP32-CAM for video streaming and the ESP32 for controlling movement.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250423_225108.jpg?raw=true)

Since I couldn't do both tasks on a single ESP32-CAM, I split the work: the ESP32-CAM streamed live video, while the ESP32 controlled the robot’s movement using the L298N motor driver. The robot could capture video, stream it over Wi-Fi, and be controlled remotely, making it a fully functional surveillance tool.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_0svTEkJVTs?si=Jbt2kRfql6Dg5fVG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 5: MQTT Publish and Subscribe Using Cloud MQTT**
In this task, I used the HiveMQ broker, a public MQTT broker, to enable communication between a Python script (publisher) and an ESP32 (subscriber).

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_013559.jpg?raw=true)

The Python script sends messages like "LED 1 ON" or "LED 2 OFF" to specific topics on HiveMQ. The ESP32 listens to these topics and controls the corresponding LEDs based on the received commands. In this setup, both the publisher and the subscriber identify themselves by subscribing or publishing to specific topics. This setup allows easy remote control of the LEDs, demonstrating how MQTT can be used to manage devices in IoT projects.

<iframe width="560" height="315" src="https://www.youtube.com/embed/wgJ2SzBcFAo?si=h2BIc0D8ML10DA6z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 6: Sending Data to ThingSpeak**
In this task, I used the DHT11 sensor and ESP32 to send temperature and humidity data to the ThingSpeak website using its API.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_004137.jpg?raw=true![])

The data was uploaded to ThingSpeak and displayed as a graph showing the temperature over time. After processing the data, I was able to retrieve it back from the website. Additionally, I used Python’s matplotlib library to plot the temperature vs time graph by downloading the dataset from ThingSpeak. This task helped me understand how to send sensor data to a website, visualize it, and retrieve it for further analysis.

<iframe width="560" height="315" src="https://www.youtube.com/embed/AlCcWPXMWC8?si=5p05JzXKVD7hy82M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 7: Communication Using I2C Protocol**
The I2C (Inter-Integrated Circuit) protocol is a serial communication method that allows multiple devices to communicate over just two wires: SDA (Data) and SCL (Clock). It’s used for short-distance communication between microcontrollers and peripheral devices like sensors and displays. 

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_010059.jpg?raw=true)

I2C follows a master-slave setup, where one master device can control multiple slave devices, each with a unique address. In this task, I used the ESP32 as the master and the Arduino UNO as the slave. The ESP32 hosted a webserver where I could input messages, which were then sent over I2C to the Arduino. The message was displayed on the Arduino serial monitor, while the ESP32 also showed updates on its web interface.

<iframe width="560" height="315" src="https://www.youtube.com/embed/dw3nten0KtI?si=HLdIzMNc2-CmaN4y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 8: Flashing Morse Code**
In this task, I set up an ESP32 to host a web server where users can enter a message through a simple HTML interface. The ESP32, connected to an LED, captures the message, converts it into Morse code, and then flashes the LED accordingly.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_012051.jpg?raw=true)

Each letter and number is represented by dots (short blinks) and dashes (long blinks). This task demonstrated a real-life application of a web server for communication, allowing messages to be sent and displayed in Morse code through the LED.

<iframe width="560" height="315" src="https://www.youtube.com/embed/jRET0_93eJU?si=5NTpD_W2adjtibrg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 9: SOIL MOISTURE SENSOR**
In this task, I used a Capacitive Soil Moisture Sensor with an ESP32 to check how wet or dry the soil is. The sensor works by creating an electric field, and when placed in soil, the amount of water affects this field. Wet soil gives a stronger signal, while dry soil gives a weaker one. This change is converted into an analog value that the ESP32 reads.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_003331.jpg?raw=true)

The ESP32 displays the moisture level on the serial monitor. If the analog value goes above a certain threshold (meaning the soil is too dry), the ESP32 gives an alert message like "Low Moisture Level" on the serial monitor to notify the user.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PQ6eaDFVtzI?si=lc_i413c9IUaY_DA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **Task 10: Read and Display Vitals**

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_024206%20(10).jpg?raw=true)

For this task, I used two phototransistors, a red LED, and an IR sensor to measure heart rate (BPM) and blood oxygen (SpO2). The phototransistors detect changes in light caused by blood flow, while the red LED and IR sensor help calculate the BPM and oxygen levels in the blood. I sent the data to Blynk IoT, where the readings are displayed in real-time. If the heart rate or oxygen levels go outside the normal range, the app sends a notification to alert the user. This setup enables easy monitoring of health vitals through an IoT platform.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PQ6eaDFVtzI?si=lc_i413c9IUaY_DA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

## **TASK 11: Fire alaram system with E-mail alerts**
For this task, I used an infrared flame sensor and an ESP32. The flame sensor detects infrared radiation emitted by fire using a photodiode that responds to the specific light wavelengths produced during combustion. When a flame is present, the sensor sends a digital signal to the ESP32.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250423_232616.jpg?raw=true)

The ESP32, always connected to Wi-Fi, continuously monitors the sensor. When fire is detected, it immediately sends an email alert to notify selected recipients about the potential fire hazard.

<iframe width="560" height="315" src="https://www.youtube.com/embed/gBO4x-jJo9M?si=Z9fuo8c5VKGEh15N" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---
```
                                                          THANK YOU!

```

---




