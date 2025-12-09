Cracking the Market Code: AI-Driven Stock Price Prediction (LSTM + Tkinter GUI)

This project is an AI-powered desktop application that predicts the next trading day's stock closing price using LSTM deep learning models, NSE historical data, and a Tkinter GUI. It fetches real-time market data from Yahoo Finance, processes it, makes predictions, and visualizes the price trend with gradients and interactive hover insights.

FEATURES

• LSTM-based deep learning model for time-series stock prediction
• Automatically identifies the next valid trading day (skips weekends and NSE holidays)
• Gradient-based visualization of historical and predicted prices
• Interactive hover feature showing date and price
• Simple Tkinter GUI for user entry and result display
• Downloads historical stock data from Yahoo Finance
• Uses MinMaxScaler for preprocessing and scaling
• Validates NSE stock tickers
• Includes prediction confidence range (±5%)

TECHNOLOGIES USED

Python
TensorFlow / Keras
NumPy
Pandas
Scikit-learn
Matplotlib
Yahoo Finance API (yfinance)
Tkinter (GUI)

INSTALLATION

Clone the repository:
git clone https://github.com/yourusername/stock-price-predictor.git

cd stock-price-predictor

Install required libraries:
pip install numpy pandas yfinance matplotlib scikit-learn tensorflow tk

HOW TO RUN THE APPLICATION

Run the following command:
python main.py

Enter a valid NSE stock ticker, for example:
RELIANCE.NS
TCS.NS
HDFCBANK.NS
INFY.NS

HOW THE PROJECT WORKS

Ticker Validation: Confirms if the ticker exists and has data.

Data Download: Fetches historical closing prices from 2000 to the present.

Preprocessing:
– Builds 60-day sequences
– Scales values using MinMaxScaler
– Creates training inputs for the LSTM model

Model Training:
A two-layer LSTM model is trained to learn price trends.

Prediction:
Predicts the next trading day's closing price using the last 60 days of data.

Visualization:
– Gradient plot of historical data
– Marked predicted point
– Prediction range shading
– Hover-to-view date and price values

NEXT TRADING DAY CALCULATION

The program skips:
• Saturdays
• Sundays
• Defined NSE holidays (included in code)

GUI OVERVIEW

• Clean and interactive interface
• Input box for ticker
• Prediction results displayed below
• Graph updates dynamically
• Hover enabled for checking approximate values

FUTURE IMPROVEMENTS

• Add multi-feature prediction (OHLC, volume, indicators)
• Provide long-term forecasting
• Introduce GRU or Transformer models
• Add dark mode UI
• Enable exporting predictions to Excel

AUTHOR

P.V.Sandeep
Andhra Pradesh, India
Email: sandeeppv1223@gmail.com

LinkedIn: (add your LinkedIn link)
GitHub: (add your GitHub profile link)

SUPPORT

If you find this project useful, consider starring the repository on GitHub.
