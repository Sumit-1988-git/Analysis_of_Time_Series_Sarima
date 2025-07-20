🪙 **Gold Price Forecasting with Time Series Analysis (ARIMA & SARIMA)**
This project conducts a thorough time series analysis and forecasting of monthly gold prices using the ARIMA and SARIMA models. It also includes a fully interactive Streamlit app for model selection, exploration, and dynamic forecasting.

📦 **Key Features**

✅ Time Series Workflow Includes:

Data Collection from Yahoo Finance for gold prices

Trend Visualization over time

STL Decomposition to break down trend, seasonality, and noise

ADF Test for checking stationarity

Differencing to achieve stationarity

ACF & PACF Plots to identify model orders

ARIMA & SARIMA Model Building

Forecasting for the next 12 months

Model Comparison using AIC/BIC

Model Saving with pickle

🚀 **Getting Started**

1. Clone the Repository

git clone https://github.com/your-username/gold-price-forecasting.git
cd gold-price-forecasting
2. Install Dependencies
Install the required libraries:


pip install -r requirements.txt
3. Run the Streamlit App

streamlit run app.py
📈 Forecast Visualization Example
Forecast using the SARIMA model (green) with 95% confidence interval:


🧠 **Model Information**

Model	AIC / BIC	Seasonality	Stationarity	Forecast Horizon
ARIMA	Evaluated	❌ No	Differenced	Short-term
SARIMA	Evaluated	✅ Yes	Differenced	Seasonal-aware

🔬 **ACF & PACF Insights:**
Spikes at seasonal lags in ACF → Add seasonal components

PACF cut-off after lag p → Suggests AR order

ACF cut-off after lag q → Suggests MA order

🧪 Example of ADF Test Output

ADF Statistic: -1.56
p-value: 0.51
Conclusion: The time series is **non-stationary**. Differencing is needed.

🧰 **Technologies Used**

Python

Pandas, Matplotlib, Statsmodels

yfinance for data fetching

Streamlit for UI

Pickle for model persistence

📌 **requirements.txt**
For deployment or sharing, use the following requirements.txt:

Copy
streamlit
pandas
matplotlib
statsmodels
yfinance
python-dateutil
