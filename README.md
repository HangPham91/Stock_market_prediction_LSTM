
<div align="center">
<img src="https://github.com/user-attachments/assets/00cdcc74-2ba2-421d-913e-547540078488" width="400" height="200">
</div>

# 📈 Stock Price Prediction for Tesla (TSLA): LSTMs

## Table of Contents
- [1. Objective](#-1-objective)
- [2. Data Collection & Preparation](#%EF%B8%8F-2-data-collection--preparation)
- [3. Tools and Technologies](#%EF%B8%8F-3-tools-and-technologies)
- [4. Key Results](#-4-key-results)
  
## 🎯 1. Objective:

- 📌 **Goal**
  - Predict Tesla’s next-day closing stock price using both **traditional machine learning** (Linear Regression) and **deep learning** (LSTM).
  - Compare performance across different input sequence lengths (e.g., 30, 60, 90, 120 days).

---

## 🗂️ 2. Data Collection & Preparation:

- 📦 **Source**
  - Historical TSLA stock data fetched via the `yfinance` library.

- 🧮 **Features Used**
  - Open, High, Low, Close, Volume

- 🎯 **Target Variable**
  - Next day’s closing price (`Tomorrow_Close`)

- ⚙️ **Preprocessing**
  - For LSTM: Applied `MinMaxScaler` normalization  
  - For Linear Regression: Used raw (unscaled) input values

---

## 🛠️ 3. Tools and Technologies:

- 💻 **Python Ecosystem**
  - pandas, numpy, matplotlib, seaborn, plotly, yfinance

- 🧰 **Machine Learning & Deep Learning**
  - Scikit-learn: MinMaxScaler, metrics, Linear Regression  
  - TensorFlow/Keras: LSTM neural networks

---

## 📌 4. Key Results:

- 📊 **Performance Comparison**
  - LSTM models (30, 60, 90, 120-day sequences) consistently outperformed Linear Regression

- 📈 **Visual Analysis**
  - Prediction results summarized and plotted for side-by-side model evaluation

- 🏆 **Best Model**
  - The top LSTM configuration achieved:
    - Lowest MAPE: **5.02%**
    - Highest R²: **0.94**
