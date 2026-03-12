---
title: "Forest Monitoring Network"
excerpt: "IoT system with LoRa communication for microclimate monitoring in forested areas."
collection: portfolio
---

## Project Description

This project involves the development of a **microclimate sensor network** designed to operate in remote forested areas. The system utilizes **LoRa (Long Range)** communication technology to transmit temperature, humidity, and other environmental variables without the need for conventional cellular coverage.

The primary objective is to generate robust databases for time-series analysis, facilitating water availability prediction and wildfire prevention.

 **💡 Practical Applications**
* **Precision Silviculture:** Delivers high-fidelity thermal and $CO_2$ data essential for modeling spatio-temporal forest structures and carbon dynamics.
* **Automated Fault Diagnostics:** Reduces operational costs by enabling remote identification of sensor drift versus real climatic events, minimizing unnecessary field expeditions to remote areas.
* **Sustainable Forest Management:** Provides verified environmental inputs for accurate carbon sequestration quantification and biomass estimation.

## Project Progress

### 1. Hardware Design (Nodes)
* **Microcontroller:** Successful implementation using ESP32.
* **Power:** Autonomous power system via solar panels and Li-Po batteries.
* **Sensors:** Integration of SHT30 sensors for temperature and capacitive soil moisture sensors. BME688 sensor for barometric pressure, temperature, humidity, altitude, and gas resistance. MHZ-16 for CO<sub>2</sub> concentration (ppm)
![datalogger](/images/03-2026-project-forest-monitoring/xx-datalogger.png)

### 2. Explotarory Data Analysis
* Initial data collection at the test site (Sierra Madre Occidental).
* Development of Python scripts for cleaning and visualizing historical data.

#### Anomaly Detection
During the monitoring cycle on January 21, 2026, the system deployed in the Sierra Madre Occidental detected a significant anomaly in CO<sub>2</sub> concentrations. While baseline levels remained stable at around 400 ppm, a sudden event was recorded at approximately 2:30 p.m., reaching a peak of over 2,500 ppm. Can we use this data for something? Yes, this dataset can be used for wildfire detection. The detected anomaly corresponds to a controlled test conducted using a fire pit.
![Anomaly Detection](/images/03-2026-project-forest-monitoring/00-anomaly.png)

####  Temperature overview: SHT vs BME

By employing a redundant design with **BME680** and **SHT3x** sensors, the system ensures data continuity in high-altitude conditions. The January 2026 data cycle serves as a compelling case study in hardware resilience; as visualized in the time-series analysis, the system successfully identified a critical failure in the BME680 unit on January 25th. While the faulty sensor drifted toward unrealistic values below **-40°C**, the high-precision SHT3x fail-safe maintained a reliable thermal baseline, preserving the integrity of the long-term data and preventing permanent information loss during the doctoral research phase.
![shtvsbme](/images/03-2026-project-forest-monitoring/01-shtvsbme.png)




## Gallery: Field installations

Data logger installed

![installed](/images/03-2026-project-forest-monitoring/x1-datainstalled.jpeg)


Checking data

![reacal](/images/03-2026-project-forest-monitoring/x2-recalibration.jpeg)

