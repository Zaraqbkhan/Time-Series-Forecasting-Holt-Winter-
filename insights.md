# 📊 Forecasting Insights – Telecom Complaints

This project applied time series forecasting to weekly complaint data for a telecom company.

## 🔍 Key Insights

- Complaint spikes are often associated with **commercial events**, especially **big promotions**, regardless of discount rate.
- Weeks with higher discount rates sometimes show **increased complaints**, possibly due to customer expectations or service load.
- All three exponential smoothing methods were tested. **Holt-Winters (Triple Exponential Smoothing)** provided the best results for capturing seasonality and trend.

## 📈 Forecasting Outcome

- The model projects a **gradual rise in complaints** during weeks with commercial campaigns.
- Helps operational teams **staff support resources proactively** ahead of anticipated demand surges.

## 🛠️ Technical Notes

- Seasonality was handled using **additive and multiplicative models**
- Model tuning was performed based on **AIC/BIC values and RMSE**
