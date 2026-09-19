# HAQI-SMART
ESP32-based smart air quality monitoring system that collects environmental data using multiple sensors, displays real-time readings on an OLED, and logs data to Google Sheets for analysis and research.
# HAQI-SMART 🌱

### Smart Air Quality Monitoring System

HAQI-SMART is a low-cost, portable air quality monitoring system developed to monitor environmental conditions and collect air quality data using an ESP32 microcontroller and multiple sensors.

The system displays sensor readings on an OLED screen and supports wireless data logging to Google Sheets. It is designed for environmental monitoring, data collection, and academic research, with potential integration into data analysis and machine learning workflows.

## 🎯 Project Objectives

* Monitor particulate matter and selected air-quality indicators.
* Measure environmental parameters such as temperature and humidity.
* Display real-time sensor readings on an OLED.
* Log sensor data wirelessly to Google Sheets.
* Support structured datasets for analysis and research.
* Develop a portable and affordable air quality monitoring prototype.

## 🛠️ Hardware Components

| Component       | Purpose                                           |
| --------------- | ------------------------------------------------- |
| ESP32 DevKit V1 | Main microcontroller and Wi-Fi connectivity       |
| PMS7003         | Particulate matter measurement                    |
| MQ-7            | Carbon monoxide sensing                           |
| SGP30 / SGP40   | VOC-related sensing, depending on the module used |
| BME280          | Temperature, humidity, and pressure measurement   |
| OLED display    | Real-time display of sensor readings              |
| Power supply    | Powers the monitoring system                      |

**Note:** The final sensor list and exact module versions should be updated to match the hardware installed in the current prototype.

## ⚙️ System Features

* Real-time sensor data acquisition
* OLED-based display
* Wi-Fi connectivity through ESP32
* Google Sheets data logging
* Configurable logging interval
* Modular sensor integration
* Designed for future data analysis and model integration

## 📊 Data Logging

HAQI-SMART supports wireless logging of sensor readings to Google Sheets through a Google Apps Script web app.

The project has used a **15-second logging interval** during data collection and testing. The interval can be adjusted according to the experiment or dataset requirements.

Logged data may include:

* Timestamp
* Particulate matter readings
* Gas-sensor readings
* Temperature
* Humidity
* Other available environmental parameters

The exact column names and units should be documented alongside the firmware to ensure consistent datasets.

## 🔌 Hardware & Firmware

The firmware is developed for the ESP32 using the Arduino IDE.

The repository can include:

* Sensor integration sketches
* OLED display code
* Wi-Fi connection and reconnection logic
* Google Sheets logging code
* Integrated firmware for the complete system
* Wiring diagrams and hardware documentation

## 📁 Suggested Repository Structure

```text
HAQI-SMART/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── system-overview.md
│   ├── hardware-and-wiring.md
│   └── data-format.md
├── firmware/
│   ├── sensor-tests/
│   ├── wifi-test/
│   ├── google-sheets-logging/
│   └── integrated-firmware/
├── hardware/
│   ├── schematics/
│   └── 3d-models/
└── datasets/
    └── README.md
```

## 🚀 Future Development

* Improve sensor calibration and validation.
* Expand environmental parameters.
* Add local data storage when an SD card is available.
* Develop dashboards and data visualization.
* Prepare consistent datasets for machine learning and research.
* Improve enclosure design and portability.

## ⚠️ Measurement Disclaimer

HAQI-SMART is a prototype intended for educational, experimental, and research use. Low-cost sensor readings may be affected by calibration, environmental conditions, and sensor limitations. Measurements should not be treated as certified regulatory air-quality data without appropriate validation.

## 🤝 Contributions

Contributions, suggestions, and improvements related to hardware integration, firmware, data logging, documentation, and analysis are welcome.

## 🏷️ Project Information

* **Project:** HAQI-SMART
* **Domain:** Air Quality Monitoring / IoT / Environmental Sensing
* **Platform:** ESP32
* **Firmware:** Arduino IDE
* **Data Logging:** Google Sheets
* **Application:** Environmental monitoring and research
