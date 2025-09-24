# GHS/USD Exchange Rate Forecasting

This project forecasts the Ghanaian Cedi (GHS) against the US Dollar (USD) using historical exchange rate data from the Bank of Ghana (and Yahoo Finance as a supplement).  
We compare **Linear Regression** and **ARIMA** models, highlighting the challenges and best practices in exchange rate prediction.

---

## 📊 Project Overview
- **Goal**: Predict the GHS/USD exchange rate at **monthly** and **weekly** intervals.
- **Approach**:
  1. Data Cleaning & Preprocessing  
  2. Linear Regression (initial attempt — poor performance)  
  3. ARIMA Forecasting (final model)  
  4. Visualization & Evaluation  
  5. Professional PDF Report  

---

## ⚠️ Challenges & Lessons
- **Linear Regression Failure**: Produced negative R² (≈ -15.7) → showed linear models are not well-suited for volatile FX data.
- **Data Errors**: Detected anomalies in Yahoo Finance (e.g., March 2020 recorded **573.0 instead of 5.73**). Corrected manually.
- **Resampling Issues**: Weekly/monthly aggregation introduced spikes, requiring careful inspection.

---

## 🚀 Results
- **Linear Regression**: Failed to capture exchange rate dynamics.  
- **ARIMA**: Performed better, providing stable 6–12 month forecasts with confidence intervals.  
- **Key Insight**: Statistical models work, but structural/economic shocks must be accounted for in future improvements (e.g., GARCH, ML hybrids).  

---

## 📂 Repository Structure

