🪙 **Gold Price Forecasting with Time Series Analysis (ARIMA & SARIMA)**

This project leverages time series analysis to forecast monthly gold prices using ARIMA and SARIMA models. A fully interactive Streamlit app is included for easy exploration, model selection, and dynamic forecasting.

📦 **Key Features**

✅ **Time Series Analysis Steps:**

* Download data from Yahoo Finance for gold prices

* Trend visualization over time

* Perform STL decomposition to extract trend, seasonality, and noise

* Conduct the ADF test for stationarity

* Apply differencing to achieve stationarity

* Generate ACF and PACF plots for determining model orders

* Build ARIMA and SARIMA models

* Forecast for the next 12 months

* Model comparison using AIC criteria

* Save models using pickle for future use

✅ **Streamlit Web Application Features:**

* Choose between ARIMA and SARIMA models

* Forecast up to 36 months ahead

* Visualize forecast results along with confidence intervals

* Access a summary of the model and historical gold price data

🗃️ **Project Structure**

📁 gold-price-forecasting/

├── app.py                    # Streamlit application file

├── arima_gold_model.pkl      # ARIMA model (auto-generated)

├── sarima_gold_model.pkl     # SARIMA model (auto-generated)

├── model_deployment.ipynb    # Main notebook for analysis & modeling (optional)

├── requirements.txt          # Required Python libraries

└── README.md                 # Overview of the project

🚀 **How to Get Started**

1. **Clone the Repository**

git clone https://github.com/your-username/gold-price-forecasting.git
cd gold-price-forecasting

3. **Install the Required Libraries**
Install dependencies with pip:
pip install -r requirements.txt

3. **Run the Streamlit App**
Start the app with:
streamlit run app.py

🔬 **Insights for ACF & PACF Plots**:

PACF cut-off after lag p → 1

ACF cut-off after lag q → 1

🧪 **Example ADF Test Output**

ADF Statistic: 1.535441
p-value: 0.997650

Conclusion: The time series is **non-stationary**.Since, the data that we worked with is not stationary,
hence we cannot use AR, MA and ARMA models. Differencing is required.

🧰 **Technologies Utilized**

* Python

* Pandas, Matplotlib, Statsmodels

* yfinance for data retrieval

* Streamlit for interactive UI

* Pickle for model serialization


📌 **requirements.txt**
For easy deployment or sharing, here's the list of required libraries for the project:

* streamlit
* pandas
* matplotlib
* statsmodels
* yfinance
* python-dateutil
