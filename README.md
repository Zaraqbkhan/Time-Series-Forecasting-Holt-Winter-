# 📈 Weekly Complaint Forecasting – Telecom Time Series Project (Python)

This project focuses on forecasting weekly customer complaints for a telecom company using time series analysis techniques. We apply three types of exponential smoothing methods and finalize the forecast using Holt-Winters (Triple Exponential Smoothing). The analysis is performed using Python.

---

## 🔧 Tools & Libraries Used

- Python (Jupyter Notebook)
- Pandas, NumPy
- Statsmodels
- Matplotlib / Seaborn

---

## 📁 Files Included

- `complaint_forecasting.ipynb` – Main notebook with EDA and forecasting
- `data_description.txt` – Description of the dataset columns
- `insights.md` – Summary of findings and forecast insights

---

## 📊 Forecasting Techniques Used

- Simple Exponential Smoothing (SES)
- Holt’s Linear Trend Method
- Holt-Winters (Additive/Multiplicative)

---

## 🕒 Time Period

- Weekly data  
- Forecast focuses on upcoming complaint volumes based on historical patterns

---

## ✅ Use Case

Helps the telecom company prepare operational resources (like support staff) based on projected complaint volumes, particularly around commercial events or discount weeks.

---

# 📁 Dataset: Weekly Telecom Complaints (Time Series)

This dataset contains weekly complaint volumes for a telecom provider, along with marketing and promotional indicators.

### Columns:

- `week`: Weekly time index  
- `complaints`: Number of complaints logged  
- `discount_rate`: Promotional discount percentage  
- `small_commercial_event`: Binary flag (minor promo)  
- `medium_commercial_event`: Binary flag (mid-level campaign)  
- `big_commercial_event`: Binary flag (major promo like product launch)

---

# 📊 Forecasting Insights – Telecom Complaints

This project applied time series forecasting to weekly complaint data for a telecom company.

## 🔍 Key Insights

- **Complaint spikes** are often associated with **big commercial events**, regardless of discount rates.
- High **discount weeks sometimes see increased complaints**, potentially due to unmet expectations or increased demand.
- **Triple Exponential Smoothing (Holt-Winters)** captured the trend and seasonality better than single/double smoothing.

### 📉 Seasonal Decomposition of Complaints
![Seasonal Decomposition](plot/seasonal_decomposition.png)

### 🔄 Autocorrelation Pattern
Shows seasonality and dependence on past values:
![Autocorrelation](plot/auto_correlation.png)

---

## 🧪 Model Comparisons & Predictions

### 🔹 Simple Exponential Smoothing (SES)
![SES Prediction](plot/single_exp_smoothing_prediction.png)

### 🔹 Holt’s Linear Trend Method
![Holt Prediction](plot/double_exp_smooting_prediction.png)

### 🔹 Holt-Winters Forecast (Triple Exponential Smoothing)
![Triple Exp Prediction](plot/triple_exp_smoothing_prediction.png)

### 🔮 Future Forecast with Holt-Winters
![Holt-Winters Forecast](plot/Holt_winter_future_prediction.png)

---

## 🧠 Conclusion

- The Holt-Winters model is ideal for handling **weekly seasonality + trend** in telecom complaint data.
- This approach enables the business to **proactively plan customer support** based on forecasted complaint volumes.
