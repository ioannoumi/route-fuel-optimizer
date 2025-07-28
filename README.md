# 🚚 route-fuel-optimizer  
**Cost‑Optimized Refueling for Fixed‑Route Fleets**

This project builds a **fuel-efficient refueling optimization system** for logistics fleets. It combines **fuel consumption modeling** with **refueling strategy optimization** to minimize fuel costs for trucks operating on fixed routes.

---

## 🔍 Overview

We estimate **fuel consumption per trip** (in liters per 100 km and total fuel used) using regression models trained on truck telemetry data. The project focuses on:

- **Segmenting time-series data** into meaningful trips  
- **Analyzing trip-level features**  
- **Optimizing refueling decisions** under real-world constraints  

---

## 🧠 Core Components

### 🚛 Fuel Consumption Modeling
Regression-based prediction of trip-level fuel usage using features like distance, speed, elevation, and vehicle weight.

### ⛽ Refueling Optimization Strategies
Three methods are implemented and compared:
1. **Greedy heuristic** – A fast, rule-based refueling approach.  
2. **Exhaustive (Cartesian) search** – Tests all combinations of stations to find the cost-optimal plan.  
3. **Multi-Objective Linear Programming** – Optimizes fuel cost, travel time, and station access using a weighted objective function.

---

## 🗂️ Project Structure

| Notebook | Description |
|----------|-------------|
| `1_EDA_and_Cleaning.ipynb` | Initial data import, cleaning, and exploratory analysis. Basic feature extraction (e.g., distance, elevation, duration). |
| `2_Trip_Segmentation.ipynb` | Segmentation of raw telemetry data into meaningful trips. Transformation into trip-level records. |
| `3_Model_Training_and_Evaluation.ipynb` | Training and evaluation of regression models (MAE, R²) for fuel consumption prediction. |
| `4_Fuel_Consumption_Optimization.ipynb` | Implementation of the three refueling strategies and comparative evaluation across cost and performance. |

---

## 📌 Project Steps

1. **Data Preprocessing** – Clean raw time-series truck data.  
2. **Trip Segmentation** – Identify stop patterns and extract trips.  
3. **Feature Engineering** – Derive useful trip-level features.  
4. **Modeling** – Train regression models to predict fuel efficiency.  
5. **Optimization** – Apply strategies to minimize refueling cost.  
6. **Evaluation** – Visualize and validate performance across models and strategies.

---

## 🙏 Acknowledgements

This project was developed in collaboration with George Konstantinos Dimou during our MSc studies. We extend our sincere gratitude to:

- **Professors Anastasios Gounaris and John Paparizos**  
- **PhD Candidate Apostolos Gianoulidis** (academic supervisor)
- **Emisia** for providing industry support and access to real-world data  
- **Michail Perdikopoulos** for continuous guidance and domain expertise
