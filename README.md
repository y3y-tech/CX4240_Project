# Portfolio Optimization
Financial Machine Learning Project



Textbook Link: https://gtvault-my.sharepoint.com/:b:/g/personal/yyu473_gatech_edu/ERZj-m4bcPxFgUBSHUgFyF4Bav9PQv501_lwqsihVF12ZA?e=K5vTfr



**To install ta-lib for backtesting.py**

```conda install -c conda-forge ta-lib```

## Goal

To classify the next 5-day price movement of the S&P 500 as:
-  `1`: > +0.5% (Bullish)
-  `0`: Between -0.5% and +0.5% (Neutral)
-  `-1`: < -0.5% (Bearish)

And use these predictions to generate algorithmic trades with realistic backtesting.

## Models Implemented

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- XGBoost Classifier
- Transformer-based Neural Network
- Long Short Term Memory (LSTM)
- Random Forest 
- Buy-and-Hold Baseline Strategy (Benchmark)

## Features Used

### Technical Indicators
- Moving Averages (MA5, MA10, MA20)
- Momentum
- Rolling Volatility
- RSI, MACD, Stochastic Oscillator
- Volume Change, Return Aggregates

### Macroeconomic Indicators
- VIX (CBOE Volatility Index)
- TNX (10-year Treasury Yield)s

## Methodology

- Rolling 3-year training windows
- Predict 5-day forward return
- Walk-forward validation to avoid lookahead bias
- Ternary classification target
- Backtesting with `backtesting.py`
  - $10,000 starting capital
  - TP/SL = ±1%
  - 20% equity per trade
  - Commission = 0.02%

## Evaluation Metrics

### Classification
- Accuracy
- Macro F1 Score
- Precision
- Confusion Matrix

### Backtesting
- Cumulative Return
- Sharpe Ratio
- Max Drawdown
- Equity Curve



