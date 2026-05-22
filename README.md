# 🌫️ IoT Based Temperature & Air Pollution Monitoring System

An IoT-based environmental monitoring system developed using ESP8266, DHT11, MQ-6 gas sensor, OLED display, and Blynk Cloud. The system continuously monitors temperature and air pollution levels and displays real-time data on both OLED display and Blynk mobile application.

---

# 📌 Features

✅ Real-time temperature monitoring  
✅ Air pollution detection using MQ-6 sensor  
✅ OLED live data display  
✅ Wireless IoT monitoring using Blynk  
✅ WiFi-enabled ESP8266 system  
✅ Pollution status indication  
✅ Mobile app visualization  
✅ Low-cost smart monitoring system

---

# 🛠️ Components Used

| Component | Quantity |
|---|---|
| ESP8266 NodeMCU | 1 |
| DHT11 Sensor | 1 |
| MQ-6 Gas Sensor | 1 |
| OLED Display (128x64 I2C) | 1 |
| Jumper Wires | As required |
| Breadboard | 1 |

---

# ⚙️ Working Principle

The system uses:

- **DHT11 Sensor** to measure temperature
- **MQ-6 Sensor** to detect harmful gases and air pollution
- **ESP8266 NodeMCU** for WiFi communication
- **OLED Display** for local monitoring
- **Blynk IoT Platform** for remote monitoring

The sensor data is continuously updated every 2 seconds and transmitted to the Blynk cloud platform.

---

# 📲 Blynk Dashboard

## Virtual Pins Used

| Parameter | Virtual Pin |
|---|---|
| Temperature | V0 |
| Gas Sensor Value | V1 |

---

# 🔌 Circuit Connections

## DHT11 Sensor

| DHT11 | ESP8266 |
|---|---|
| VCC | 3.3V |
| GND | GND |
| DATA | D4 |

---

## MQ-6 Gas Sensor

| MQ-6 | ESP8266 |
|---|---|
| VCC | 5V |
| GND | GND |
| AO | A0 |

---

## OLED Display (I2C)

| OLED | ESP8266 |
|---|---|
| VCC | 3.3V |
| GND | GND |
| SDA | D2 |
| SCL | D1 |

---

# 📊 OLED Output

The OLED display shows:

- Temperature value
- Gas sensor value
- Pollution status

### Status Conditions

| Gas Value | Status |
|---|---|
| > 400 | POLLUTED |
| ≤ 400 | NORMAL |

---

# 💻 Arduino Libraries Required

Install the following libraries from Arduino IDE:

- ESP8266WiFi
- Blynk
- DHT Sensor Library
- Adafruit GFX
- Adafruit SSD1306

---

# 🌐 IoT Features

- Real-time cloud monitoring
- Mobile notification support
- Wireless sensor monitoring
- Remote environmental tracking

---

# 🚀 Future Improvements

- Add humidity monitoring
- AI-based pollution prediction
- GSM alert system
- Firebase cloud integration
- Mobile push notifications
- Multi-sensor air quality analysis

---

# 🎯 Applications

- Smart homes
- Industrial safety monitoring
- Air quality monitoring
- Environmental monitoring systems
- IoT smart city projects

---

# 📁 Project Structure

```txt
IoT-Air-Pollution-Monitoring/
│
├── README.md
├── main.ino
├── circuit_diagram.png
├── blynk_dashboard.png
└── images/
