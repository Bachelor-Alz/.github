# Health Monitoring System

This GitHub organisation hosts the repositories for a **Health Monitoring System** designed for elderly care.

## About the Project

The **Health Monitoring System** is an **Arduino-based** health tracking solution that specifically **predicts falls for elderly individuals** and provides **direct notifications to caregivers**.

This project is developed by students at **Aalborg University** as part of a **bachelor project** for the **BSc in Software Engineering**.

---

## System Overview

The system consists of several key components working together:

1.  **Device:** Data is initially gathered by a **wearable health monitoring device** running code from the [`Device` repository](https://github.com/Bachelor-Alz/Device). This Arduino-based device collects real-time sensor data, including fall-related data, heart rate, SpO2, steps, and distance.
2.  **Fall-Detection:** Fall data collected by the device is specifically used by the **Fall Detection component** ([`Fall-Detection` repository](https://github.com/Bachelor-Alz/Fall_detection)). This component analyzes the data to predict if a fall has occurred.
3.  **Backend:** An **external backend server** ([`Backend` repository](https://github.com/Bachelor-Alz/Backend)) receives the fall prediction data from the `Fall-Detection` component. It also receives the other health data (heart rate, SpO2, steps, distance) directly from the device. The backend processes, stores, and manages all this health information.
4.  **App:** A **mobile application for caregivers** ([`App` repository](https://github.com/Bachelor-Alz/App)) connects to the backend to retrieve and display the processed health data. The app showcases the collected data, including falls, heart rate, SpO2, steps, and distance, enabling caregivers to monitor the individual's health and receive timely alerts for detected falls.
