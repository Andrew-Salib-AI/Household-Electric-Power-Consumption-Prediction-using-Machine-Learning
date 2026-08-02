# ⚡ Household Electric Power Consumption Prediction

A complete end-to-end machine learning project that analyzes and predicts household electricity consumption using real-world time series data. Seven models are trained, evaluated, and compared to find the best predictor.

---

## 📌 Project Overview

This project covers the full data science pipeline — from raw data cleaning to model deployment-ready predictions — using the UCI Household Power Consumption dataset recorded at one-minute intervals over nearly 4 years.

---

## 🔄 Pipeline

```
Raw Data → Cleaning → Feature Engineering → EDA → Modeling → Evaluation → Insights
```

---

## 📊 Dataset

- **Source:** UCI Machine Learning Repository — Individual Household Electric Power Consumption
- **Size:** ~2 million minute-level records
- **Target:** `Global_active_power` (kW)
- **Features:** Voltage, Global reactive power, Sub-metering 1/2/3, date/time

---

## 🛠️ What's Inside

### 1. Data Preprocessing
- Parsed datetime index from Date + Time columns
- Time-based interpolation for missing values
- Resampled from minute-level to hourly averages
- Removed duplicates and statistical outliers (IQR method)

### 2. Feature Engineering
- Extracted: `hour`, `day_of_week`, `month`, `year`, `is_weekend`
- Normalized features using MinMaxScaler

### 3. Exploratory Data Analysis
- Time series trends
- Correlation heatmap
- Consumption by hour, weekday, and month (boxplots)
- Distribution histogram with outlier visualization

### 4. Models Trained
| Model | Type |
|---|---|
| Linear Regression | Baseline |
| Support Vector Machine (SVR) | Kernel-based |
| Gradient Boosting | Ensemble |
| Random Forest | Ensemble |
| MLP Neural Network | Deep Learning |
| XGBoost | Boosting |
| LSTM | Recurrent Neural Network |

### 5. Evaluation Metrics
- RMSE (Root Mean Squared Error)
- R² Score
- MAE (Mean Absolute Error)
- Training Time

---

## 📈 Key Results

- ✅ **Best models:** XGBoost & Random Forest (highest R², lowest RMSE)
- 🕐 **Most important features:** Hour of day, Sub-metering 3
- 🌙 **Peak consumption:** Evening hours (6–9 PM)
- 📅 **Weekend patterns** differ significantly from weekdays

---

## 🧰 Tech Stack

| Library | Purpose |
|---|---|
| Pandas / NumPy | Data manipulation |
| Scikit-learn | ML models & preprocessing |
| XGBoost | Gradient boosting |
| TensorFlow / Keras | LSTM model |
| Matplotlib / Seaborn | Visualization |

Just replace `your-username` and `Your Name` with your actual info, and you're ready to publish. Would you like me to also generate the `requirements.txt` file for this project?
