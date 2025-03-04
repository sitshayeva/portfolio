# London Weather Forecasting with Prophet (Open-Meteo API)

## 📌 Project Overview
This project **retrieves, processes, and forecasts** daily average temperatures for the last 5 years using **Prophet**, an advanced time-series forecasting model developed by Meta (Facebook). The model accounts for **seasonality, trends, and irregular variations** to provide reliable weather predictions.

## 📂 Features
- **Fetches historical weather data** from the Open-Meteo API.
- **Processes raw data** into a structured format.
- **Forecasts temperatures for the next 365 days** using Prophet.
- **Visualizes trends** with color-coded scatter plots and prediction trendlines.
- **Stores data in CSV and SQLite database** for future use.

## 🛠️ Tech Stack
- **Python 3.9+**
- **Prophet (for forecasting)**
- **Matplotlib & Pandas (for data visualization and processing)**
- **Requests (for API calls)**
- **SQLite3 (for database storage)**

## 🚀 Installation & Setup
### 1️⃣ Install Required Dependencies
Ensure you have Python installed, then install the necessary packages:
```bash
pip install requests pandas matplotlib sqlite3 prophet
```

### 2️⃣ Run the Script
Execute the main script to fetch data, forecast, and visualize results:
```bash
python weather_forecast.py
```

## 📊 How It Works
### 1️⃣ **Fetching Weather Data**
The script retrieves **daily average temperatures** from Open-Meteo API for the last 5 years.

### 2️⃣ **Processing Data**
- Converts **API JSON response** into a structured Pandas DataFrame.
- Handles **missing values** to ensure data quality.

### 3️⃣ **Forecasting with Prophet**
- Fits the Prophet model to **historical temperature data**.
- Predicts **next 365 days of temperatures**.

### 4️⃣ **Visualization**
- **Historical data** displayed as a scatter plot with a color gradient.
- **Future predictions** plotted as a **red dashed trendline**.
- **Interactive color bar** for temperature variation.

## 📁 Data Storage
- **CSV Files:** Stores processed data (`daily_avg_temperature.csv`) and predictions (`future_temperature_predictions.csv`).
- **SQLite Database:** Saves structured temperature data for future reference.

## 🔧 Troubleshooting
### ❌ Prophet Import Error
If you see an error while importing Prophet, install it using:
```bash
pip install prophet
```

### ❌ API Request Failed
If the API request fails, check your **internet connection** or try a different **latitude/longitude**.

## 📜 License
This project is open-source under the **MIT License**.

## 📞 Contact
For any issues or improvements, feel free to create an **issue or pull request**!

