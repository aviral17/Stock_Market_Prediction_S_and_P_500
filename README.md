# Comprehensive Stock Market Analysis and Portfolio Optimization

## Project Overview
This project performs an in-depth analysis of 10 major stocks over a 5-year period (2013-2018) using advanced financial analytics, machine learning, and portfolio optimization techniques. The analysis includes risk assessment, return prediction, and optimal portfolio allocation to maximize returns while minimizing risk.

## Dataset
- **Source**: Kaggle S&P500 Stock Dataset
- **File**: `all_stocks_5yr.csv`
- **Time Period**: April 22, 2013 to February 7, 2018 (1,210 trading days)
- **Stocks Analyzed**: BAC, AAPL, GE, F, FB, MSFT, AMD, MU, INTC, CSCO

## Key Findings

### Performance Highlights
- **Best Performing Stock**: FB with 600.27% cumulative return
- **Worst Performing Stock**: GE with -29.89% cumulative return
- **Most Volatile Stock**: AMD (0.604 annualized volatility)
- **Most Traded Stock**: BAC (110,101,336,519 total volume)

### Portfolio Optimization Results
- **Maximum Sharpe Ratio Portfolio**:
  - Return: 33.41%
  - Volatility: 20.30%
  - Sharpe Ratio: 1.5475
  - Optimal Allocation: MSFT (31.65%), GE (15.46%), CSCO (15.11%), BAC (11.02%), INTC (7.05%), MU (7.60%), AAPL (6.76%), AMD (2.52%), FB (1.61%), F (1.21%)

- **Minimum Volatility Portfolio**:
  - Return: 16.15%
  - Volatility: 14.93%
  - Sharpe Ratio: 0.9479
  - Conservative Allocation: AMD (19.44%), INTC (16.50%), BAC (16.60%), F (11.52%), MU (9.86%), FB (9.63%), GE (9.20%), MSFT (5.18%), AAPL (1.44%), CSCO (0.63%)

### Risk Assessment
- **Highest Risk Stock**: CSCO (VaR at 5% confidence: -0.0184)
- **Lowest Risk Stock**: AMD (VaR at 5% confidence: -0.0515)
- **Maximum Drawdown**: MU (-73.80%)

### Stock Price Prediction
- **Best Model**: Linear Regression (R² = 1.000)
- **Prediction Accuracy**:
  - Mean Absolute Error: $0.16
  - Root Mean Squared Error: $0.28
  - Error Range: -$1.75 to $3.23

### Stock Clustering
Identified 3 distinct clusters based on performance metrics:
- **Cluster 0**: AMD, CSCO, F, GE, INTC, MSFT, MU (Traditional Tech & Industrial)
- **Cluster 1**: FB (Social Media - High Performer)
- **Cluster 2**: AAPL, BAC (Consumer Tech & Finance)

## Methodology

### Technical Analysis
- Calculated key technical indicators: RSI, MACD, Bollinger Bands, Moving Averages
- Analyzed correlation patterns between stocks
- Measured volatility and risk metrics

### Portfolio Optimization
- Implemented Modern Portfolio Theory using Monte Carlo simulation
- Optimized for both maximum Sharpe ratio and minimum volatility
- Generated efficient frontier visualization

### Machine Learning Models
- Trained and evaluated 6 regression models for stock price prediction:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Random Forest
  - Gradient Boosting
  - Support Vector Regression

### Risk Analysis
- Calculated Value at Risk (VaR) at 5% confidence level
- Measured maximum drawdown for each stock
- Performed risk-adjusted performance evaluation

### Clustering Analysis
- Applied K-means clustering to group stocks by performance characteristics
- Used Principal Component Analysis (PCA) for visualization
- Identified optimal number of clusters using elbow method



## How to Run the Analysis
1. Download the dataset from Kaggle: [S&P500 Stock Dataset](https://www.kaggle.com/datasets/camnugent/sandp500)
2. Place `all_stocks_5yr.csv` in the project directory
3. Open and run the Jupyter notebook `stock_analysis.ipynb`
4. All visualizations will be generated automatically and saved as PNG files

## Required Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- yfinance (for real-time data updates)

## Conclusion
This comprehensive analysis provides valuable insights into stock performance, risk characteristics, and optimal portfolio allocation. The key findings demonstrate:
1. Significant performance variation among stocks, with FB showing exceptional returns while GE declined
2. The possibility of constructing optimized portfolios with superior risk-adjusted returns (Sharpe ratio of 1.5475)
3. Linear regression's effectiveness in predicting stock prices with high accuracy (R² = 1.000)
4. Distinct clustering patterns that can inform diversification strategies

The analysis tools and methodologies developed in this project can be applied to any set of stocks to inform investment decisions and risk management strategies.

## Future Enhancements
- Incorporate real-time data feeds for continuous analysis
- Implement deep learning models for improved prediction accuracy
- Add fundamental analysis metrics to complement technical indicators
- Develop a web-based interactive dashboard for portfolio visualization
- Include options and derivatives for more sophisticated risk management
