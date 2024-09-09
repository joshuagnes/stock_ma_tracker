# Stock Price Simulation with Moving Averages

## Overview
This project simulates stock prices using random data and calculates both the 5-day and 10-day moving averages. The goal of the project is to visualize how moving averages interact with stock price trends over time.

## Key Features
- **Simulated Stock Prices:** Randomly generated stock prices using a normal distribution with a cumulative sum.
- **Moving Averages:** Calculation of the 5-day and 10-day moving averages of the stock price.
- **Data Visualization:** Matplotlib is used to plot the stock prices along with the moving averages.

## Libraries Used
- **Pandas:** For handling date ranges and calculating the moving averages.
- **Numpy:** For generating random stock price data.
- **Matplotlib:** For visualizing the stock prices and moving averages.

## Code Explanation

### Data Generation:
- A series of 200 dates is created starting from January 1, 2023.
- Simulated stock prices are generated using `np.random.randn()` to create random values, and a cumulative sum is applied to create a realistic stock price trend.

### DataFrame Setup:
- A `pandas` DataFrame is used to store the stock prices with the dates as the index.
- Two new columns are added to the DataFrame to calculate the 5-day and 10-day moving averages.

### Moving Averages:
- The 5-day and 10-day moving averages are calculated using the `rolling()` function provided by pandas.

### Plotting:
- A line chart is generated using `matplotlib` that includes:
  - The stock prices.
  - The 5-day moving average.
  - The 10-day moving average.

### Display:
- The plot is displayed using `plt.show()` and the last few rows of the data are printed to the console using `data.tail()` to check the latest moving averages.

