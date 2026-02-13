# flight_prices_analysis
Workintech Grad Project<br>
https://www.kaggle.com/datasets/dilwong/flightprices/data<br>
https://lookerstudio.google.com/reporting/d2b0e86a-f455-4145-afe4-20bfeaf6f0ab<br>
# ✈️ Flight Market Analysis & Price Forecasting

This project analyzes airline ticket pricing dynamics using historical flight price data and presents actionable booking insights through interactive dashboards and time-series forecasting.

The analysis focuses on:
- **Optimal booking windows (lead time)**
- **Best day of week to search**
- **Route-level price behavior**
- **Price volatility & last-minute effects**
- **Time-series price forecasting using SARIMA**

---

## 📊 Live Dashboard (Looker Studio)

Interactive dashboards built with **Google Looker Studio**:

🔗 **Dashboard Link**
https://lookerstudio.google.com/reporting/d2b0e86a-f455-4145-afe4-20bfeaf6f0ab

The dashboard includes:
- Global booking behavior insights
- Route-level price optimization
- Final booking recommendations by route
- Airline & fare structure analysis
- SARIMA-based price forecasts

---

## 🗂️ Dataset

**Source:** Kaggle
🔗 https://www.kaggle.com/datasets/dilwong/flightprices/data

**Description:**
- US domestic flight prices
- Includes route, airline, fare class, search date, flight date, seat availability, and pricing details
- Time range used in analysis: **June 2022**

---

## 🧠 Key Analyses

### 1️⃣ Global Price Patterns
- Lead time vs median ticket price
- Cheapest booking window identified
- Day-of-week effects on prices and search volume
- Price volatility metrics

### 2️⃣ Route-Level Price Analysis
- Last-minute price increase by route
- Early booking advantage by route
- Best booking window per route
- Best day to search per route
- Route-specific price vs demand dynamics

### 3️⃣ Airline & Fare Structure
- Price comparison by airline
- Fare class & flight type impact
- Base fare vs tax analysis
- Seat availability effects on pricing

### 4️⃣ Final Booking Recommendation
For each selected route:
- **Optimal booking window (lead time bucket)**
- **Best day of week to search**
- **Typical lowest median price**
- Based on historical median prices and sufficient sample size

---

## ⏱️ Time Series Forecasting (SARIMA)

To model future ticket prices, a **SARIMA (Seasonal ARIMA)** model was applied.

**Target Route Example:** `LAX-BOS`

### Model Highlights
- Daily median price time series
- Seasonal patterns handled via SARIMA
- Train / test split on time axis
- Forecast horizon: future daily prices

### Evaluation Metrics
- **MAE:** 18.36
- **RMSE:** 24.35
- **MAPE:** 5.95%

The model demonstrates strong performance in capturing seasonal trends and short-term price movements.

---

## 📈 Technologies Used

- **Python**
  - pandas, numpy
  - statsmodels (SARIMA)
  - matplotlib / seaborn
- **Google Looker Studio**
