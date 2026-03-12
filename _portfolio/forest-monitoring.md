---
title: "Forest Monitoring Network"
excerpt: "IoT system with LoRa communication for microclimate monitoring in forested areas."
collection: portfolio
---

## Project Description

This project involves the development of a **microclimate sensor network** designed to operate in remote forested areas. The system utilizes **LoRa (Long Range)** communication technology to transmit temperature, humidity, and other environmental variables without the need for conventional cellular coverage.

The primary objective is to generate robust databases for time-series analysis, facilitating water availability prediction and wildfire prevention.

## Project Progress

### 1. Hardware Design (Nodes)
* **Microcontroller:** Successful implementation using ESP32.
* **Power:** Autonomous power system via solar panels and Li-Po batteries.
* **Sensors:** Integration of SHT30 sensors for temperature and capacitive soil moisture sensors. BME688 sensor for barometric pressure, temperature, humidity, altitude, and gas resistance.

### 2. Communication Network
* A star network topology has been established.
* Successful LoRa range tests conducted up to 5km within line of sight.
* Gateway configuration for uploading data to the cloud.

### 3. Data Analysis
* Initial data collection at the test site (Sierra Madre Occidental).
* Development of Python scripts for cleaning and visualizing historical data.

## Gallery
*(Here you can add images of your prototypes or field installations)*