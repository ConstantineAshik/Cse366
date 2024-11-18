# Trading Agent Decision System

This project implements a simple trading decision system with two main functionalities:

1. **Basic Stock Purchase Decision**:
   - Calculates the number of units to buy based on the last price, average price, and current stock levels.

2. **Trading Agent Class**:
   - A more advanced decision-making framework that considers average price, discount thresholds, critical stock levels, and order quantities.
   - Includes a plotting feature to visualize decision-making over time.

## Features

- **Basic Decision Logic**:  
  A standalone function `calculate_tobuy` evaluates whether to purchase stock based on simple conditions.

- **Trading Agent Class**:  
  The `TradingAgent` class provides customizable decision-making logic with parameters such as:
  - `ave_price`: Average price of the stock.
  - `discount_threshold`: Percentage drop below the average price that triggers a large order.
  - `critical_stock_level`: Minimum stock level before a small order is triggered.
  - `order_quantity`: Units to order for large orders.
  - `min_order_quantity`: Units to order for small orders.

- **Visualization**:  
  The `plot_decision` method generates a time series plot showing stock prices, inventory levels, and corresponding decisions.
