# 📈 Time Series Forecasting: ETS vs ARIMA vs Regression

## A Comparative Study Using R

This project compares three time series forecasting models—**Exponential Trend Smoothing (ETS)**, **ARIMA**, and **Time Series Regression**—using monthly data from **1982 and 1983**. Built in **R**, the project explores patterns, develops models, and evaluates performance to determine the best method for predicting the next 14 periods.

---

## 🧠 Models Compared

* **ETS (Exponential Trend Smoothing)** – Captures trend and seasonality through smoothing
* **ARIMA** – Combines autoregression, differencing, and moving average
* **Time Series Regression** – Regression with time-based features and seasonal dummies

---

## 🔍 Key Findings

### 📊 Performance Summary (on Test Set)

| Metric   | ETS    | ARIMA  | Regression |
| -------- | ------ | ------ | ---------- |
| **MAE**  | 4.27   | 4.52   | **4.12**   |
| **RMSE** | 5.19   | 5.44   | **4.83**   |
| **MAPE** | 12.78% | 13.65% | **11.93%** |

✅ **Time Series Regression** was chosen as the most effective model due to:

* The **lowest error metrics** across MAE, RMSE, and MAPE
* High **interpretability**, making it suitable for analysis and explanation
* Robust performance with seasonality captured via dummy variables

---

## 🛠️ Tools & Packages Used

* R, RStudio
* `forecast`, `ggplot2`, `dplyr`
* Evaluation metrics: MAE, RMSE, MAPE

---

## 📁 Repository Structure

```
time-series-forecasting/
1. data/            # Input time series data
2. scripts/         # R scripts for each model and evaluation
3. results/         # Model performance and summary files
4. README.md        # Project documentation
```

---

## 📌 Conclusion

While **ETS** and **ARIMA** offered solid baseline forecasts, **Time Series Regression** proved to be the most suitable approach for this dataset. It delivered the **most accurate predictions** and provided clear, interpretable outputs for decision-making.

Organizations or researchers forecasting economic or business indicators with seasonal behavior may benefit from using regression-based forecasting for **short- to mid-term projections**.

