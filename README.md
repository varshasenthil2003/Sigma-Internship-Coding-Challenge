# SIGMA INTERNSHIP CODING CHALLENGE

## Overview
This repository contains code for building a simple stock trading model using the Quantrocket platform. The objective of the model is to make decisions on certain days based on pre-specified logic and maximize the portfolio value. The model utilizes historical price data of Apple Inc. (AAPL) for the year 2023 to make buy/sell decisions.

## Getting Started
1. Install Quantrocket on your local machine or on a cloud platform of your choice.
2. Clone this repository to your local machine.

## Dependencies
- Quantrocket
- pandas
- matplotlib
- PyPortfolioOpt
- statsmodels

## Usage
1. Ensure Quantrocket is installed and configured on your system.
2. Run the provided code to retrieve data and execute the trading model.
3. Review the outputs and adjust parameters as needed for further experimentation.

## Code Breakdown

### Data Retrieval
- The code retrieves daily close price data for AAPL stock for the year 2023 from the Quantrocket platform.

### Data Preprocessing
- The retrieved price data is formatted into a pandas DataFrame with 'Date' as the index and 'FIBBG000B9XRY4' (closing price) as the only column.

### Data Visualization
- The closing prices of AAPL for 2023 are plotted using matplotlib to visualize the price trends over time.

### Calculations and Analysis
- Returns are calculated based on daily percentage changes in closing prices.
- Portfolio optimization techniques such as Efficient Frontier and Discrete Allocation are applied to maximize portfolio value.
- Forecasting using the ARIMA model is performed to predict future price movements.
- State classification is implemented to categorize states as Bull, Flat, or Bear based on returns.
- Buy/sell signals are determined based on state transitions and portfolio value maximization.

## Outputs
- **Closing Prices Plot**: A plot showing the closing prices of AAPL for 2023.
- **Portfolio Value**: The final portfolio value achieved by the trading model.
    Portfolio values for each day: [0, 0, 0, 0, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 5, 5, 5, 6, 6, 7, 7, 7, 6, 6, 6, 5, 5, 5, 4, 4, 5, 5, 5, 5, 4, 4, 4, 4, 4, 5, 5, 6, 6, 6, 6, 6, 5, 5, 6, 6, 7, 7, 7, 6, 6, 5, 5, 5, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 7, 7, 7, 7, 7, 7, 8, 8, 8, 9, 9, 9, 9, 9, 9, 10, 10, 10, 9, 9, 9, 10, 10, 10, 11, 11, 11, 11, 11, 12, 12, 13, 13, 13, 14, 14, 14, 14, 15, 15, 15, 16, 16, 16, 17, 17, 17, 17, 17, 16, 16, 16, 16, 16, 17, 17, 17, 16, 16, 16, 16, 16, 16, 17, 17, 17, 16, 16, 15, 15, 15, 15, 15, 15, 15, 14, 14, 13, 13, 13, 13, 14, 14, 14, 14, 15, 15, 15, 15, 15, 14, 14, 14, 14, 13, 13, 13, 13, 14, 14, 13, 13, 13, 13, 12, 12, 12, 12, 13, 13, 13, 13, 14, 14, 14, 14, 14, 13, 13, 13, 13, 13, 12, 12, 12, 11, 11, 11, 12, 12, 13, 13, 13, 14, 14, 14, 14, 15, 15, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 17, 17, 18, 18, 17, 17, 18, 18, 18, 18, 18, 17, 17, 17, 17, 17, 17, 17]
-----------------------------------------------------------
Final portfolio value: 17
-----------------------------------------------------------

- **Optimal Buy Indices**: Indices representing the optimal points where buy orders should be placed.
  Optimal Buy Indices: [5, 7, 11, 15, 20, 27, 29, 32, 35, 38, 40, 44, 49, 51, 56, 58, 60, 63, 65, 68, 78, 84, 87, 93, 96, 99, 102, 107, 109, 112, 116, 119, 122, 127, 132, 135, 141, 144, 146, 153, 155, 159, 163, 168, 172, 176, 178, 182, 186, 190, 195, 200, 203, 206, 208, 211, 215, 217, 231, 233, 235, 237, 242]

- **Probability Distribution**: Probability distribution of transitioning from one state to another.
  Probability Matrix:
[0.04435483870967742, 0.1532258064516129, 0.028225806451612902]
[0.16129032258064516, 0.3790322580645161, 0.09274193548387097]
[0.016129032258064516, 0.10483870967741936, 0.020161290322580645]

- **Corresponding Dates for Buy Indices**: Dates corresponding to the optimal buy indices.
    Corresponding dates for buy indices:
2023-01-10
2023-01-12
2023-01-19
2023-01-25
2023-02-01
2023-02-10
2023-02-14
2023-02-17
2023-02-23
2023-02-28
2023-03-02
2023-03-08
2023-03-15
2023-03-17
2023-03-24
2023-03-28
2023-03-30
2023-04-04
2023-04-06
2023-04-12
2023-04-26
2023-05-04
2023-05-09
2023-05-17
2023-05-22
2023-05-25
2023-05-31
2023-06-07
2023-06-09
2023-06-14
2023-06-21
2023-06-26
2023-06-29
2023-07-07
2023-07-14
2023-07-19
2023-07-27
2023-08-01
2023-08-03
2023-08-14
2023-08-16
2023-08-22
2023-08-28
2023-09-05
2023-09-11
2023-09-15
2023-09-19
2023-09-25
2023-09-29
2023-10-05
2023-10-12
2023-10-19
2023-10-24
2023-10-27
2023-10-31
2023-11-03
2023-11-09
2023-11-13
2023-12-04
2023-12-06
2023-12-08
2023-12-12
2023-12-19
- **Covariance Matrix**: Covariance matrix for the portfolio.
    COVARIANCE MATRIX :  Sid             FIBBG000B9XRY4
Sid                           
FIBBG000B9XRY4        0.039816

- **Portfolio Variance**: Variance of the portfolio.
  0.0398164650843007
  
- **Portfolio Volatility**: Volatility of the portfolio.
   0.1995406351706356
- **Portfolio Return (Annual)**: Expected annual return of the portfolio.
  Expected annual return :  46.0%
  Annual risk            :  20.0%
  Annual variance        :  4.0%

- **Backtesting Output**: Final portfolio value and trade signals obtained from backtesting.
    Final Portfolio Value: 20
Trade Signals: ['Sell', 'Buy', 'Sell', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Buy', 'Buy', 'Buy', 'Hold', 'Buy', 'Buy', 'Sell', 'Hold', 'Hold', 'Buy', 'Buy', 'Sell', 'Buy', 'Sell', 'Hold', 'Hold', 'Buy', 'Hold', 'Buy', 'Sell', 'Hold', 'Sell', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Sell', 'Hold', 'Buy', 'Buy', 'Sell', 'Hold', 'Sell', 'Sell', 'Buy', 'Buy', 'Hold', 'Buy', 'Hold', 'Buy', 'Buy', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Buy', 'Hold', 'Buy', 'Hold', 'Hold', 'Sell', 'Hold', 'Sell', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Buy', 'Buy', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Sell', 'Hold', 'Sell', 'Sell', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Buy', 'Sell', 'Buy', 'Hold', 'Buy', 'Buy', 'Hold', 'Hold', 'Hold', 'Sell', 'Sell', 'Hold', 'Hold', 'Sell', 'Sell', 'Hold', 'Hold', 'Buy', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Sell', 'Sell', 'Hold', 'Buy', 'Hold', 'Buy', 'Buy', 'Hold', 'Buy', 'Buy', 'Hold', 'Hold', 'Buy', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Buy', 'Hold', 'Buy', 'Hold', 'Sell', 'Hold', 'Buy', 'Hold', 'Hold', 'Hold', 'Hold', 'Sell', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold', 'Hold']

- **VISULAIZATIONS** :
- 
  ![Closing Price plot ](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/closing%20price.png)
  ![Count Plot](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/count.png)
  ![Drawdown](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/drawdown.png)
  ![matrix ](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/matrix.png)
  ![portfolio ](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/portfolio.png)
  ![rolling returns ](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/rolling%20returns.png)
  ![forecasting ](https://github.com/varshasenthil2003/Sigma-Internship-Coding-Challenge/blob/main/Visualizations/forecasting.png)

## Author
[Your Name]

