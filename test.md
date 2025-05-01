# **MARVEL LEVEL 1 TASKS**

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

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/_Amx9fiMfHA?si=8rFLYoBAuXU5zV_o"></iframe>

---
```
```








## **TASK 2: Basics of MQTT protocol and other communication protocols**

```
MQTT (Message Queuing Telemetry Transport)

Introduction

MQTT is a lightweight and efficient messaging protocol.  
It was originally designed for networks that are low-bandwidth, high-latency, or unreliable. 
 
This makes it ideal for Internet of Things (IoT) applications.  
MQTT uses a publish-subscribe (pub/sub) messaging model.  
This model is more efficient than traditional client-server communication.  
It’s especially useful for devices with limited resources, like sensors, wearables, and embedded systems.

Key Components 
 
Client: A device (like a sensor or application) that publishes or subscribes to messages.  
Broker: A server that receives all messages from publishers and routes them to subscribers.  
Topic: A string that defines how messages are categorized and filtered. Topics are hierarchical, for example: home/livingroom/temperature.

How MQTT Works
 
A publisher sends a message to a specific topic.  
The broker receives the message and forwards it to all subscribers of that topic.  
Devices subscribe to specific topics to receive relevant data.  
This system decouples devices from one another, allowing flexible and scalable communication.

Protocol Comparison

1. AMQP (Advanced Message Queuing Protocol)
 
Type/Layer: Messaging / Application Layer  
Key Features: Reliable, secure, supports asynchronous messaging; works across platforms and over unreliable networks.  
Use Cases: Enterprise systems, cloud integration, finance, secure machine-to-machine communication.

2. Bluetooth / BLE (Bluetooth Low Energy)
 
Type/Layer: Wireless / Physical and Data Link Layer  
Key Features: BLE is optimized for low power and short range; standard Bluetooth is used for higher data needs.  
Use Cases: Wearables, smartwatches, health trackers, in-store navigation, smart home applications.

3. Cellular (2G/3G/4G/5G)

Type/Layer: Wireless / Network Layer  
Key Features: Long-range, high-bandwidth communication; 5G provides low latency.  
Use Cases: Vehicle telemetry, mobile IoT, asset tracking, remote monitoring.

4. CoAP (Constrained Application Protocol)

Type/Layer: Application Layer  
Key Features: Lightweight, RESTful protocol that works over UDP and integrates well with HTTP.  
Use Cases: Smart agriculture, environmental sensors, remote device control.

5. DDS (Data Distribution Service)
 
Type/Layer: Middleware / Application Layer  
Key Features: Real-time, low-latency, scalable publish-subscribe communication.  
Use Cases: Aerospace, robotics, industrial control systems, defense.

6. LoRa / LoRaWAN

Type/Layer: Wireless / Physical and Network Layer  
Key Features: Long-range, low-power, non-cellular communication; LoRaWAN supports cloud connectivity.  
Use Cases: Smart agriculture, rural IoT, environmental monitoring, water management.

7. LWM2M (Lightweight M2M)

Type/Layer: Device Management Protocol  
Key Features: Designed for constrained devices; supports remote management and firmware updates.  
Use Cases: Metering, remote monitoring, IoT device lifecycle management.

8. MQTT (Message Queuing Telemetry Transport)

Type/Layer: Messaging / Application Layer  
Key Features: Lightweight, publish-subscribe model; works over TCP/IP; supports QoS levels 0–2; efficient in low-bandwidth conditions.  
Use Cases: Smart homes, IoT sensors, industrial IoT, mobile applications, telemetry.

9. Wi-Fi

Type/Layer: Wireless / Physical and Data Link Layer  
Key Features: High data rate, low latency; suitable for short to medium range; relatively power-consuming.  
Use Cases: Smart appliances, indoor surveillance, LAN-based IoT systems.

10. XMPP (Extensible Messaging and Presence Protocol)

Type/Layer: Messaging / Application Layer  
Key Features: XML-based protocol for real-time, structured communication.  
Use Cases: Smart appliances, lightweight messaging systems, chat-enabled IoT devices.

11. Zigbee

Type/Layer: Mesh Network / Physical and Data Link Layer  
Key Features: Low-power, short-range communication; self-healing mesh network; secure and reliable.  
Use Cases: Home automation, lighting, HVAC systems, industrial monitoring.

12. Z-Wave

Type/Layer: Mesh Network / Physical Layer  
Key Features: Proprietary low-power mesh network; operates on sub-GHz frequencies; secure and scalable.  
Use Cases: Home security systems, smart locks, smart energy devices.

```
---
```
```



## **TASK 3: Basics of Creating a Website**

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/colorweb.PNG?raw=true)


For this task, I learned how websites work from both the front-end and back-end. I made a simple webpage with a button that changes the background color through VIBGYOR colors when clicked. I used HTML for the structure, CSS for styling, and JavaScript to make the button work. It helped me understand how the front-end looks and feels, and how the back-end connects everything behind the scenes. This was a fun and helpful way to get started with web development.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/cvlxigZiR78?si=2RsKofGUCvDuK_Aw"></iframe>

---
```
```



## **TASK 4:  ESP32 CAM-Based Surveillance Robot using Arduino IDE**
For this task, I built a surveillance robot using the ESP32-CAM for video streaming and the ESP32 for controlling movement.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250423_225108.jpg?raw=true)

Since I couldn't do both tasks on a single ESP32-CAM, I split the work: the ESP32-CAM streamed live video, while the ESP32 controlled the robot’s movement using the L298N motor driver. The robot could capture video, stream it over Wi-Fi, and be controlled remotely, making it a fully functional surveillance tool.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/_0svTEkJVTs?si=Jbt2kRfql6Dg5fVG"></iframe>

---
```
```




## **TASK 5: MQTT Publish and Subscribe Using Cloud MQTT**
In this task, I used the HiveMQ broker, a public MQTT broker, to enable communication between a Python script (publisher) and an ESP32 (subscriber).

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_013559.jpg?raw=true)

The Python script sends messages like "LED 1 ON" or "LED 2 OFF" to specific topics on HiveMQ. The ESP32 listens to these topics and controls the corresponding LEDs based on the received commands. In this setup, both the publisher and the subscriber identify themselves by subscribing or publishing to specific topics. This setup allows easy remote control of the LEDs, demonstrating how MQTT can be used to manage devices in IoT projects.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)


---

<iframe height="315" src="https://www.youtube.com/embed/wgJ2SzBcFAo?si=h2BIc0D8ML10DA6z"></iframe>

---
```
```





## **TASK 6: Sending Data to ThingSpeak**
In this task, I used the DHT11 sensor and ESP32 to send temperature and humidity data to the ThingSpeak website using its API.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_004137.jpg?raw=true![])

The data was uploaded to ThingSpeak and displayed as a graph showing the temperature over time. After processing the data, I was able to retrieve it back from the website. Additionally, I used Python’s matplotlib library to plot the temperature vs time graph by downloading the dataset from ThingSpeak. This task helped me understand how to send sensor data to a website, visualize it, and retrieve it for further analysis.

How does that DHT11/DHT22 WORK?
It uses a thermistor internally to detect temperature.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/AlCcWPXMWC8?si=5p05JzXKVD7hy82M"></iframe>

---
```
```





## **TASK 7: Communication Using I2C Protocol**
The I2C (Inter-Integrated Circuit) protocol is a serial communication method that allows multiple devices to communicate over just two wires: SDA (Data) and SCL (Clock). It’s used for short-distance communication between microcontrollers and peripheral devices like sensors and displays. 

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_010059.jpg?raw=true)

I2C follows a master-slave setup, where one master device can control multiple slave devices, each with a unique address. In this task, I used the ESP32 as the master and the Arduino UNO as the slave. The ESP32 hosted a webserver where I could input messages, which were then sent over I2C to the Arduino. The message was displayed on the Arduino serial monitor, while the ESP32 also showed updates on its web interface.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/dw3nten0KtI?si=HLdIzMNc2-CmaN4y"></iframe>

---
```
```

## **TASK 8: Flashing Morse Code**
In this task, I set up an ESP32 to host a web server where users can enter a message through a simple HTML interface. The ESP32, connected to an LED, captures the message, converts it into Morse code, and then flashes the LED accordingly.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_012051.jpg?raw=true)

Each letter and number is represented by dots (short blinks) and dashes (long blinks). This task demonstrated a real-life application of a web server for communication, allowing messages to be sent and displayed in Morse code through the LED.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/jRET0_93eJU?si=5NTpD_W2adjtibrg"></iframe>

---
```
```


## **TASK 9: SOIL MOISTURE SENSOR**
In this task, I used a Capacitive Soil Moisture Sensor with an ESP32 to check how wet or dry the soil is. The sensor works by creating an electric field, and when placed in soil, the amount of water affects this field. Wet soil gives a stronger signal, while dry soil gives a weaker one. This change is converted into an analog value that the ESP32 reads.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_003331.jpg?raw=true)

The ESP32 displays the moisture level on the serial monitor. If the analog value goes above a certain threshold (meaning the soil is too dry), the ESP32 gives an alert message like "Low Moisture Level" on the serial monitor to notify the user.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/PQ6eaDFVtzI?si=lc_i413c9IUaY_DA"></iframe>

---

```
```






## **Task 10: Read and Display Vitals**

Failed to do this as per task per some what built a prototype.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250424_024206%20(10).jpg?raw=true)

For this task, I used two phototransistors, a red LED, and an IR sensor to measure heart rate (BPM) and blood oxygen (SpO2). The phototransistors detect changes in light caused by blood flow, while the red LED and IR sensor help calculate the BPM and oxygen levels in the blood. I sent the data to Blynk IoT, where the readings are displayed in real-time. If the heart rate or oxygen levels go outside the normal range, the app sends a notification to alert the user. This setup enables easy monitoring of health vitals through an IoT platform.

---

<iframe height="315" src="https://www.youtube.com/embed/Rcgef1AF710?si=-nxRMh-gGcCsopsX"></iframe>

---

```
```



## **TASK 11: Fire alaram system with E-mail alerts**
For this task, I used an infrared flame sensor and an ESP32. The flame sensor detects infrared radiation emitted by fire using a photodiode that responds to the specific light wavelengths produced during combustion. When a flame is present, the sensor sends a digital signal to the ESP32.

![](https://github.com/TR33SS/forMARVEL/blob/main/LVL1/20250423_232616.jpg?raw=true)

The ESP32, always connected to Wi-Fi, continuously monitors the sensor. When fire is detected, it immediately sends an email alert to notify selected recipients about the potential fire hazard.

[SOURCE CODE](https://github.com/TR33SS/LVL1/tree/code)

---

<iframe height="315" src="https://www.youtube.com/embed/gBO4x-jJo9M?si=Z9fuo8c5VKGEh15N"></iframe>

---



```
                                                                                           THANK YOU!

```

---

