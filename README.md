
# NVIDIA Stock Analysis

This project provides a comprehensive analysis of NVIDIA Corporation's (NASDAQ: NVDA) stock performance over several years. The analysis includes various statistical methods, time series forecasting, and advanced machine learning techniques to understand the trends, seasonality, and volatility of the stock prices.

## Table of Contents
- [NVIDIA Stock Analysis](#nvidia-stock-analysis)
  - [Table of Contents](#table-of-contents)
  - [Dataset Description](#dataset-description)
  - [Analysis Overview](#analysis-overview)
  - [Key Insights](#key-insights)
  - [Requirements](#requirements)
  - [Usage](#usage)
  - [Project Structure](#project-structure)
  - [Contributing](#contributing)
  - [License](#license)

## Dataset Description

The dataset used in this analysis includes daily market performance data for NVIDIA Corporation. It contains the following columns:
- **Date**: The date of the market data.
- **Open**: The opening price of NVIDIA stock on that day.
- **High**: The highest price reached by NVIDIA stock during the day.
- **Low**: The lowest price reached by NVIDIA stock during the day.
- **Close**: The closing price of NVIDIA stock on that day.
- **Adj Close**: The adjusted closing price, accounting for corporate actions like stock splits and dividends.
- **Volume**: The volume of NVIDIA stock traded on that day.

## Analysis Overview

The Jupyter Notebook in this repository performs the following analyses:
1. **Exploratory Data Analysis (EDA)**: Initial exploration of the dataset with summary statistics and visualizations.
2. **Moving Averages**: Calculation and plotting of 20-day, 50-day, and 200-day moving averages.
3. **Correlation Analysis**: Calculation and visualization of the correlation matrix.
4. **Volatility Analysis**: Calculation and plotting of daily returns and rolling volatility.
5. **Seasonality Analysis**: Using Fourier transforms and seasonal decomposition to identify seasonal patterns.
6. **Autocorrelation and Partial Autocorrelation**: Analyzing time series dependencies.
7. **ARIMA Modeling**: Time series forecasting using the ARIMA model.
8. **LSTM for Time Series Prediction**: Advanced time series forecasting using LSTM neural networks.
9. **GARCH Model for Volatility Clustering**: Understanding volatility clustering with the GARCH model.
10. **Event Analysis**: Impact of major events on stock prices.

## Key Insights

1. **Seasonality and Trends**:
   - Significant periodic components indicate the presence of seasonality.
   - Clear trends and seasonal patterns are observable in NVIDIA's stock prices.

2. **Autocorrelation and Partial Autocorrelation**:
   - Significant lags suggest past prices influence future prices.

3. **ARIMA Modeling**:
   - Reasonable fit for predicting future stock prices, but more complex models might be needed for higher accuracy.

4. **LSTM Modeling**:
   - LSTM models capture underlying patterns in stock prices better than linear models.

5. **Volatility Analysis**:
   - GARCH model reveals periods of high and low volatility, crucial for risk management and trading strategies.

6. **Event Analysis**:
   - Major events like earnings reports and product launches significantly impact stock prices.

## Requirements

To run the Jupyter Notebook, you need the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scikit-learn
- tensorflow
- arch

You can install these libraries using `pip`:
```sh
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn tensorflow arch
```

## Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/debjit-mandal/NVIDIA-Stock-Analysis.git
   cd NVIDIA-Stock-Analysis
   ```

2. Ensure you have all the required libraries installed:
   ```sh
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:
   ```sh
   jupyter notebook NVDA_Advanced_Analysis.ipynb
   ```

4. Run the cells in the notebook to perform the analysis.

## Project Structure

```
.
├── NVDA_Advanced_Analysis.ipynb                   # Jupyter Notebook with the analysis
├── data/NVDA.csv                                  # Dataset
├── LICENSE                                        # License
├── README.md                                      # Project description and instructions
└── requirements.txt                               # List of required libraries
```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to create a pull request or open an issue.

1. Fork the repository.
2. Create a new branch: `git checkout -b my-branch-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin my-branch-name`.
5. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
