# Store Sales Time Series Forecasting

## Summary
This project focuses on forecasting daily sales for retail stores using historical sales data, store information, transactions, oil prices, and holiday events. The goal is to predict sales accurately to support inventory management and strategic planning. Seasonal trends, holidays, and promotions are important factors influencing sales.

---

## Dataset
- **train.csv:** Daily sales data for each store and product family  
- **stores.csv:** Store metadata including type and cluster  
- **transactions.csv:** Daily transaction counts per store  
- **oil.csv:** Historical oil prices  
- **holidays_events.csv:** Holiday and event information  

---

## Models Used
- **Linear Regression**  
- **Random Forest Regressor**  
- **Bagging Regressor**  
- **Extra Trees Regressor**  
- **SARIMAX and ARIMA** for time series modeling  

**Features:** `onpromotion`, `type`, `Oil_Price`, `weekday`  
**Target:** `sales`

---

## Evaluation Metrics
- **Mean Absolute Percentage Error (MAPE)**  
- **Mean Squared Log Error (MSLE)**  

**Key Results:**  
- Random Forest and Bagging Regressor performed best (MAPE ~18–20%)  
- Linear Regression had higher errors (MAPE ~45%)  
- SARIMAX and ARIMA captured seasonality with MAPE ~28–31%  

---

## Future Work
- Incorporate more granular transaction and product-level features  
- Explore advanced models like **Prophet, LSTM, or XGBoost**  
- Automate hyperparameter tuning and cross-validation  
