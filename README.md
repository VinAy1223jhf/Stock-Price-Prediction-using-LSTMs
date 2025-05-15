# 📈 Stock Price Prediction Using LSTM

This project demonstrates how to use a Long Short-Term Memory (LSTM) neural network to predict stock prices, specifically for **Apple Inc. (AAPL)**, using historical data from Yahoo Finance.

---

## ✅ Project Overview

Forecasting stock prices is a classic problem in time series analysis. This project aims to:
- Build a robust deep learning model to **predict stock closing prices** using past observations.
- Use **LSTM networks**, which are ideal for sequential and time-series data, to learn trends and temporal dependencies.
- Visualize actual vs predicted results and forecast the **next 10 days of stock prices**.

---

## 🧰 Tech Stack & Concepts Used

### 📦 Libraries & Frameworks:
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- yfinance
- scikit-learn
- TensorFlow/Keras

### 📚 Concepts Applied:
- Time series forecasting
- Long Short-Term Memory (LSTM)
- Data normalization and windowing
- Deep learning model stacking and dropout
- Model evaluation and inverse transformation

---

## 🧠 Model Architecture

The LSTM model is composed of the following layers:

```text
Input Shape: (60 timesteps, 1 feature)
↓
LSTM (50 units) + Dropout (0.2)
↓
LSTM (60 units) + Dropout (0.3)
↓
LSTM (80 units) + Dropout (0.4)
↓
LSTM (120 units) + Dropout (0.5)
↓
Dense (1 unit) – Final stock price prediction
