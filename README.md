# Traffic Flow Prediction Models

## 📌 Project Overview
This project develops and evaluates predictive models for traffic flow forecasting, comparing statistical and deep learning approaches.

## 🚀 Models Developed
### 1️⃣ Model A: **ARIMA Model**
- Uses historical traffic flow data.
- Baseline statistical model for time-series forecasting.

### 2️⃣ Model B: **LSTM Model**
- Deep learning model using historical traffic data.
- Captures sequential dependencies in traffic flow.

### 3️⃣ Model C: **Enhanced LSTM Model**
- Incorporates additional variables:
  - **Weather conditions**
  - **Rainfall data**
  - **Weekend patterns**
- Improves long-term traffic prediction accuracy.

---

## 🔬 Two-Level Model Comparison
This study evaluates the models at two levels:

### 🔹 **Level 1: ARIMA vs. LSTM (Model A vs. Model B)**
- Tests the effectiveness of deep learning over traditional time-series forecasting.

### 🔹 **Level 2: Basic LSTM vs. Enhanced LSTM (Model B vs. Model C)**
- Analyzes the impact of incorporating external factors into LSTM models.

---

## 📊 Model Performance Comparison
The models are evaluated using **Mean Absolute Error (MAE), Root Mean Square Error (RMSE), and R² (coefficient of determination)**.

### **Short-Term Forecasting (1Hr – 3Hr)**
| Model             | MAE (1Hr) | MAE (2Hr) | MAE (3Hr) | RMSE (1Hr) | RMSE (2Hr) | RMSE (3Hr) | R² (1Hr) | R² (2Hr) | R² (3Hr) |
|------------------|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| **ARIMA**        | 27       | 421      | 710      | 27       | 429      | 840      | 0.99     | 0.95     | 0.79     |
| **Univariate LSTM** | 189   | 215      | 232      | 269      | 316      | 349      | 0.975    | 0.969    | 0.957    |
| **Multivariate LSTM** | 156  | 187      | 175      | 230      | 278      | 307      | 0.987    | 0.98     | 0.977    |

### **Long-Term Forecasting (1Hr – 12Hr – 24Hr)**
| Model             | MAE (1Hr) | MAE (12Hr) | MAE (24Hr) | RMSE (1Hr) | RMSE (12Hr) | RMSE (24Hr) | R² (1Hr) | R² (12Hr) | R² (24Hr) |
|------------------|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| **Multivariate LSTM** | 156  | 269      | 300      | 230      | 435      | 470      | 0.987    | 0.952    | 0.944    |

---

