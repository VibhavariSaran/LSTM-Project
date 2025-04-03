# LSTM-Project
**NIFTY 50 vs BPCL LSTM Stock Price Prediction Project**:  

## **Overview**  
This dataset consists of **historical stock price data** for **NIFTY 50 and BPCL (Bharat Petroleum Corporation Ltd.)**, sourced from **Yahoo Finance**. The dataset is used for **training and evaluating deep learning models**, specifically **LSTM-based models**, to forecast stock prices based on past trends and patterns.  

---

## **Features**  
- **Date** – Trading date.  
- **Open, High, Low, Close Prices** – Daily stock price fluctuations.  
- **Volume** – Number of shares traded per day.  
- **Moving Averages (50-day, 200-day)** – Long-term trend indicators.  
- **RSI (Relative Strength Index) & MACD (Moving Average Convergence Divergence)** – Momentum indicators for analyzing market trends.  
- **Volatility Metrics** – Standard deviation of stock returns to analyze market fluctuations.  
- **Technical Indicators** – Bollinger Bands, Exponential Moving Averages for deeper market insights.  

---

## **Usage**  
### **Load the dataset into a Pandas DataFrame:**  
```python
import pandas as pd  
df = pd.read_csv('nifty50_bpcl_stock_data.csv')  
print(df.head())  
```  

### **Perform exploratory data analysis (EDA) to visualize trends:**  
```python
import matplotlib.pyplot as plt  
df['Close'].plot(title='Stock Closing Prices')  
plt.show()  
```  

### **Train an LSTM model for stock price prediction:**  
- Preprocess the dataset (normalize values using MinMax Scaling).  
- Create time-series sequences using a **60-day rolling window**.  
- Train a **deep learning model using LSTM layers** to capture stock market patterns.  

---

## **Installation**  
To set up the environment, install the necessary libraries:  
```bash
pip install numpy pandas matplotlib tensorflow keras scikit-learn yfinance
```  

---

## **Applications**  
**Algorithmic Trading:** Use predictive models to automate stock buying/selling.  
**Risk Management:** Identify potential risks using volatility and trend analysis.  
**Investment Strategies:** Backtest strategies using historical price movements.  

---

## **Future Enhancements**  
**Integration of real-time stock data** for live trading applications.  
**Implementation of sentiment analysis** from financial news and social media.  
**Exploration of Transformer-based models** (such as the Attention mechanism) for improved sequence forecasting.  

---

## **License**  
This dataset and analysis are intended for **research and educational purposes only**.  

---

## **Contributors**  
**Vibhavari Saran**  
**Samuya Raghuvanshi**  
