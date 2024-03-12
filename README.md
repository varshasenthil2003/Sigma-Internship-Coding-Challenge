# Sigma-Internship-Coding-Challenge

## Overview

This repository contains my solution to the ASigma Internship coding challenge, focusing on algorithmic trading with the goal of maximizing portfolio value through strategic buy orders. The challenge revolves around Apple Inc. (AAPL) stock data for the year 2023.

## Outputs

### Final Portfolio Value

The final portfolio value achieved using the trading strategy is 17.

### Optimal Buy Indices

The optimal buy indices, representing the days on which buy orders should be executed, are as follows:
[5, 7, 11, 15, 20, 27, 29, 40, 49, 51, 58, 60, 68, 78, 84, 87, 93, 99, 102, 107, 109, 112, 116, 119, 122, 132, 141, 159, 163, 176, 186, 190, 206, 208, 211, 215, 217, 231, 233, 237]


### Transition Probabilities Matrix

The transition probabilities matrix, indicating the likelihood of transitioning between different market states, is as follows:
From/To | Bear | Flat | Bull
Bear | 0.14 | 0.74 | 0.11
Flat | 0.15 | 0.60 | 0.25
Bull | 0.12 | 0.68 | 0.20


## Visualizations Output

### Line Plot: Daily Closing Prices
This line chart illustrates the daily closing prices of Apple Inc. (AAPL) stock throughout the year 2023. It provides insights into the stock's performance over time, highlighting trends and fluctuations.



## Getting Started

1. Clone the repository to your local machine.
2. Install the required dependencies listed in `requirements.txt`.
3. Run the Python script `Sigma_wedge_Varsha_S.py` to execute the portfolio analysis and optimization code.
4. View the generated outputs and visualizations to understand the results of the trading strategy.

## Dependencies

- `quantrocket`: Quantitative research platform for automated trading strategies.
- `pandas`: Data manipulation and analysis library.
- `matplotlib`: Data visualization library.
- `statsmodels`: Library for statistical modeling and analysis.
- `seaborn`: Statistical data visualization library.
- `PyPortfolioOpt`: Python library for portfolio optimization.

## Strategy Development

The strategy involves calculating daily returns, classifying market states, defining a value function for buy orders, and calculating transition probabilities to inform buying decisions.


## Conclusion

This repository provides a comprehensive solution to the Sigma Internship coding challenge, demonstrating a strategic approach to algorithmic trading and portfolio optimization. Through careful analysis of market data and informed decision-making, the strategy aims to maximize returns and mitigate risks in AAPL stock trading.
