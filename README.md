## Stock Price Prediction



---

## 📋 Project Overview

This project demonstrates the application of machine learning techniques to predict next-day stock closing prices using historical market data. The implementation compares two regression algorithms: **Linear Regression** and **Random Forest Regressor**, providing insights into their performance for time-series financial forecasting.

---

## 🎯 Objective

Use historical stock data to predict the next day's closing price using machine learning models.

---

## 📊 Dataset

**Source**: Yahoo Finance (via yfinance Python library)

**Features Used**:
- **Open**: Opening price of the stock
- **High**: Highest price during the trading day
- **Low**: Lowest price during the trading day
- **Volume**: Number of shares traded
- **Engineered Features**:
  - Moving Averages (5-day, 10-day, 20-day)
  - Volatility measures
  - Price changes and daily range
  - Previous day's closing price

**Sample Stock**: Configurable (e.g., AAPL, TSLA, GOOGL, MSFT)

---

## 🛠️ Technologies Used

- **Python 3.8+**
- **Libraries**:
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computing
  - `matplotlib` & `seaborn` - Data visualization
  - `scikit-learn` - Machine learning models and evaluation
  - `yfinance` - Stock data fetching

---




## 📁 Project Structure

```
Task2-Stock-Price-Prediction/
│
├── Task2_Stock_Price_Prediction.ipynb    # Main Jupyter notebook
├── README.md                               # Project documentation
├── requirements.txt                        # Python dependencies
```

---

## 🔬 Methodology

### 1. Data Collection
- Fetch historical stock data from Yahoo Finance
- Alternative: Use generated sample data for testing

### 2. Data Exploration & Visualization
- Analyze price trends and patterns
- Visualize OHLC data and trading volume
- Examine feature correlations

### 3. Feature Engineering
- Create moving averages (MA_5, MA_10, MA_20)
- Calculate volatility measures
- Compute price changes and daily ranges
- Generate lag features

### 4. Data Preprocessing
- Handle missing values (from rolling windows)
- Split data into training (80%) and testing (20%) sets
- Apply feature scaling for Linear Regression

### 5. Model Training
- **Linear Regression**: Simple, interpretable baseline model
- **Random Forest Regressor**: Ensemble model capturing non-linear patterns

### 6. Model Evaluation
Metrics used:
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **R² Score** (Coefficient of Determination)
- **MAPE** (Mean Absolute Percentage Error)

### 7. Prediction & Analysis
- Generate next-day price predictions
- Compare actual vs predicted prices
- Analyze feature importance

---

## 📈 Key Results

### Model Performance (Sample Results)

| Metric | Linear Regression | Random Forest |
|--------|------------------|---------------|
| RMSE   | $X.XX            | $X.XX         |
| MAE    | $X.XX            | $X.XX         |
| R²     | 0.XXXX           | 0.XXXX        |
| MAPE   | X.XX%            | X.XX%         |

*(Actual values will vary based on stock selection and time period)*

### Key Insights

1. **Feature Importance**: Moving averages and previous closing prices are the most influential predictors
2. **Model Comparison**: Random Forest typically outperforms Linear Regression due to its ability to capture non-linear relationships
3. **Accuracy**: Models can predict next-day prices with reasonable accuracy for short-term forecasting

---

## 📊 Visualizations

The notebook includes comprehensive visualizations:

1. **Stock Price Trends**: Historical closing prices and volume
2. **OHLC Comparison**: All four price metrics over time
3. **Moving Averages**: Price trends with different MA windows
4. **Correlation Heatmap**: Feature relationships
5. **Prediction Plots**: Actual vs predicted prices for both models
6. **Error Distribution**: Histogram of prediction errors
7. **Feature Importance**: Bar chart showing most influential features

---

## 💡 Key Learnings

### Technical Skills
- Time series data handling and preprocessing
- Feature engineering for financial data
- Regression modeling with scikit-learn
- Model evaluation and comparison
- Data visualization with matplotlib/seaborn

### Domain Knowledge
- Understanding stock market data structure
- Importance of technical indicators (moving averages, volatility)
- Limitations of historical price-based predictions
- Need for external factors (news, sentiment, economics)

---

## ⚠️ Limitations & Considerations

1. **Market Complexity**: Stock prices are influenced by numerous factors beyond historical prices (news, sentiment, global events)
2. **External Factors**: The model doesn't account for fundamental analysis, earnings reports, or market sentiment
3. **Black Swan Events**: Unexpected events can cause rapid price changes that models can't predict
4. **Overfitting Risk**: Particularly with Random Forest on small datasets
5. **Time Horizon**: Short-term predictions are more reliable than long-term forecasts

**⚠️ Important Disclaimer**: This project is for educational purposes only. Do NOT use these predictions for actual trading decisions without consulting financial professionals.

---

## 🔮 Future Improvements

1. **Advanced Models**: Implement LSTM/GRU neural networks for better time-series modeling
2. **Sentiment Analysis**: Incorporate news headlines and social media sentiment
3. **Technical Indicators**: Add RSI, MACD, Bollinger Bands
4. **Fundamental Data**: Include P/E ratios, earnings, revenue data
5. **Ensemble Methods**: Combine multiple models for robust predictions
6. **Real-time Updates**: Implement streaming data pipeline
7. **Backtesting**: Test strategy performance over historical periods

---

## 👨‍💻 Author

**Muhammad Bilal Askari**  
AI/ML Engineering Intern  
DevelopersHub Corporation

---

## 📄 License

This project is part of an educational internship program.

---


## 🙏 Acknowledgments

- DevelopersHub Corporation for the internship opportunity
- Yahoo Finance for providing historical stock data
- The scikit-learn and pandas communities for excellent documentation

---

