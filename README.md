# 🚗 Dynamic Pricing for Urban Parking Lots

**Capstone Project – Summer Analytics 2025**  
Organized by **Consulting & Analytics Club × Pathway**

---

## 📌 Overview

In rapidly urbanizing cities, parking spaces are limited and demand varies throughout the day. Static pricing often leads to **either overcrowding or underutilization** of parking lots. To solve this, we built a **real-time dynamic pricing engine** for 14 urban parking spaces using data-driven models and real-time data streams.

The project simulates how smart cities can optimize parking revenue and traffic by **adjusting prices dynamically** based on:

- Real-time occupancy
- Vehicle queue lengths
- Traffic congestion
- Special events or holidays
- Capacity of parking lots

---

## 🎯 Project Objective

To build **two levels of intelligent pricing models** that increase in complexity:

### ✅ Model 1: Baseline Linear Model
- Linear price increase with occupancy.
- `Price(t+1) = Price(t) + α × (Occupancy / Capacity)`

### ✅ Model 2: Demand-Based Model
- Price influenced by:
  - Occupancy Rate
  - Queue Length
  - Traffic Level
  - Special Day Indicator
  - Vehicle Type (Car, Bike, Truck)
- Normalized demand modifies base price smoothly.


---

## 🛠️ Tech Stack

| Component                | Technology                      |
|-------------------------|----------------------------------|
| Data Manipulation       | `Pandas`, `NumPy`                |
| Real-Time Simulation    | `Pathway`                        |
| Visualization           | `Bokeh`                          |
| Development Environment | Google Colab                     |


---

## 🧪 Data Description

- **14 parking lots** × **73 days** × **18 time slots/day**
- Data Features:
  - Lot: Latitude, Longitude, Capacity, Occupancy, Queue
  - Vehicle: Type (Car/Bike/Truck)
  - Environment: Traffic level, Special day flag
  - Interval: Every 30 minutes from 8:00 AM to 4:30 PM

---

## Visualization Goals

All visualizations are built in **Bokeh** and run in real-time:

- Price over time for each lot
- Price comparison with nearby competitors
- Dynamic rerouting suggestions when lots are full

---

## Real-Time Engine with Pathway

The system is powered by **Pathway**, allowing:

- Real-time data streaming and delayed ingestion
- Processing of features per timestamp
- Continuous price prediction outputs




