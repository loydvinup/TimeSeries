# Time Series Forecasting - Airline Passengers  

## Overview  
This project focuses on **time series forecasting** using the **AirPassengers dataset**, which contains **monthly airline passenger data from 1949 to 1960**. The goal is to analyze **trends, seasonality, and stationarity** and apply **ARIMA & SARIMA models** to predict future passenger traffic.  

Time series forecasting is widely used in finance, sales, weather prediction, and demand forecasting. This project provides an end-to-end implementation of time series analysis, from **data preprocessing** to **forecasting future values**.  

## Dataset  
📂 **File:** `AirPassengers.csv`  
📊 **Rows:** 144  
🔢 **Columns:**  
- **Month** – Date (YYYY-MM) representing the time period  
- **#Passengers** – The number of airline passengers in that month  

The dataset is **non-stationary**, meaning trends and seasonality exist, making it a great candidate for forecasting models.  

## Project Workflow  
### 1️⃣ Data Preprocessing  
- Read and clean the dataset  
- Convert **Month** to a datetime format  
- Set **Month** as the index for time series operations  

### 2️⃣ Exploratory Data Analysis (EDA)  
- Plot the time series to observe **trends and seasonality**  
- Compute **rolling mean** and **standard deviation** to check variability  
- Perform **seasonal decomposition** to separate trend, seasonality, and residuals  

### 3️⃣ Stationarity Check  
- Use **Augmented Dickey-Fuller (ADF) test** to determine if the series is stationary  
- Apply **differencing** to remove trends and make the data stationary  

### 4️⃣ Time Series Modeling  
- Use **Auto ARIMA** to determine optimal parameters  
- Train **ARIMA (AutoRegressive Integrated Moving Average) model**  
- Implement **SARIMA (Seasonal ARIMA) model** to improve seasonal forecasting  

### 5️⃣ Model Evaluation & Forecasting  
- Compare ARIMA and SARIMA models based on **prediction accuracy**  
- Forecast **passenger traffic for the next 60 months**  
- Visualize the predicted values against actual data  

## Technologies Used  
🚀 **Python Libraries:**  
- **Pandas** – Data manipulation  
- **NumPy** – Numerical operations  
- **Matplotlib & Seaborn** – Data visualization  
- **Statsmodels** – ARIMA & SARIMA models  
- **pmdarima** – Auto ARIMA for parameter tuning  

## Results & Insights  
- The dataset shows a **strong upward trend** with **seasonal variations**  
- **Stationarity is achieved** after differencing  
- **SARIMA performs better** than ARIMA for seasonal data  
- Forecasted values provide insights into future airline passenger trends  

## Future Improvements  
🔹 Experiment with **LSTM (Long Short-Term Memory)** for deep learning-based forecasting  
🔹 Use **Prophet by Facebook** for trend detection  
🔹 Optimize hyperparameters for better model accuracy  

