# 🦠 COVID-19 Live Tracker (NodeMCU + OLED)

This project is a **COVID-19 Live Tracker** built using an **ESP8266 NodeMCU** and an **OLED display**.  
It fetches real-time COVID-19 data (cases, deaths, recovered) from **Worldometer** using **ThingSpeak** as a data pipeline, and displays it on the OLED.

---
# 🧠 Features
- 📡 Fetches live COVID-19 data (Cases, Deaths, Recovered)
- 📶 Connects to Wi-Fi using NodeMCU (ESP8266)
- 📊 Uses ThingSpeak API as an intermediary for fetching Worldometer data
- 🖥️ Displays results on a 0.96" OLED (128x64)
- 🔄 Auto-refreshes data at fixed intervals
---

# ⚙️ Hardware Required
- NodeMCU ESP8266
- OLED Display (128x64, I2C)
- Breadboard + Jumper wires
- USB cable for flashing
---

# ▶️ How to Run
- Install the Arduino IDE with ESP8266 board support.
- Clone this repo and open covid_tracker.ino.
- Add your Wi-Fi credentials in wifi_config.h.
- Upload the code to NodeMCU
- The OLED will show:
- 🟢 Confirmed Cases
- ⚰️ Deaths
- 💚 Recovered
---

# 🎯Goals
- Explore IoT + API integration
- Display real-time data on hardware
- Understand API requests & JSON parsing on microcontrollers
---

# ⚠️ Notes
- Data source: Worldometer COVID-19 stats via ThingSpeak API
- ThingSpeak is used to avoid direct HTTPS calls from ESP8266 (since SSL is heavy).
- This was a learning project during the pandemic, not for medical use.
---
