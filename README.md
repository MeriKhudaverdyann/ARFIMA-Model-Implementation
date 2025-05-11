# Fractal Time Series Forecasting GUI

## Project Overview  
This project provides a desktop-based application for time series forecasting using fractal analysis and ARFIMA modeling. The system integrates Python-based data processing and forecasting techniques with an interactive GUI built in PyQt5. Key analytical components include the Hurst exponent, fractal dimension estimation, and ARFIMA-based forecasting, all wrapped into an easy-to-use interface. The main code and functionality are included across three notebooks: `Interface.ipynb`, `Fractal Analysis.ipynb`, and `ARFIMA Model.ipynb`.

---

## Dataset  
The application accepts any **univariate time series dataset** in CSV format. Users can select the time series column during GUI interaction.

**Dataset Expectations:**
- Format: CSV
- Structure: One column should contain a sequential, time-ordered numerical series
- Typical Applications: Stock prices, climate measurements, temperature data, etc.

---

## Analysis Highlights  

### 1. Fractal Feature Extraction  
- **Hurst Exponent:** Estimated using rescaled range (R/S) analysis to assess long-term memory in the series  

### 2. Stationarity and Seasonal Decomposition  
- **Stationarity Tests:** Includes Augmented Dickey-Fuller (ADF) and KPSS tests  
- **Decomposition:** Visual seasonal-trend decomposition using moving averages  

### 3. ARFIMA Forecasting Model  
- **Fractional Differencing:** The order of differencing `d` is automatically estimated  
- **Model Fitting:** ARFIMA model is fitted using GPH semi-parametric estimation method  

### 4. Forecast Evaluation  
- Metrics like **RMSE** and **MAE** are computed on test data  
- Forecast plots compare training, actual, and predicted series  

---

## GUI Features  
- **File Loader:** Browse and select CSV files  
- **Column Selector:** Choose which column to analyze  
- **Plot Output:** All visual outputs are embedded and scrollable  
- **Forecast Visuals:** Train-test-forecast comparison  

---

## Recommendations  
- **Academic Use:** Great for teaching and experimentation with fractal time series concepts  
- **Financial Forecasting:** Apply on financial datasets to capture long-memory behavior  
- **Climate Research:** Useful for examining trends and cycles in environmental time series  

---

## Conclusion  
This application provides an accessible way to perform sophisticated time series forecasting using fractal analysis and ARFIMA modeling. It combines statistical rigor with a user-friendly GUI, enabling data exploration, model fitting, and interpretation for a wide range of users.
