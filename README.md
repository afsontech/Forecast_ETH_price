# 🧠 Ethereum Price Forecast (ARIMA Model)

This project presents a short-term **Ethereum (ETH-USD) price prediction web app** built using Python, Streamlit, and ARIMA modeling. It leverages one year of historical closing price data to forecast the next 1–30 days based on trend, seasonality, and autocorrelations.

## 📌 Features

* 📈 Interactive time series plot of Ethereum closing prices
* 🔮 ARIMA-based forecasting with adjustable prediction horizon (1–30 days)
* 📊 ADF test and differencing for stationarity analysis
* 📉 Autocorrelation and partial autocorrelation visualizations
* 🔁 Seasonal decomposition
* 📦 Built-in forecast confidence interval

## ⚙️ Technologies Used

* Python
* Streamlit
* Statsmodels
* Pandas
* Matplotlib
* YFinance

## 📡 How It Works

* Downloads 1 year of ETH-USD data from Yahoo Finance
* Performs statistical checks (ADF test, ACF/PACF, decomposition)
* Fits a SARIMA model with optimized `(p,d,q)` values
* Forecasts up to 30 future days with confidence bounds
* Visualizes historical and predicted data in the web interface

## 📂 How to Run

1. Clone the repository

   ```bash
   git clone https://github.com/yourusername/eth-price-forecast.git
   cd eth-price-forecast
   ```

2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app

   ```bash
   streamlit run model.py
   ```

## ⚠️ Disclaimer

This forecast is a statistical projection based solely on past price behavior. **It does not account for real-time market news, events, or regulatory developments**. Use this tool as a learning or research aid—not as financial advice.

---
