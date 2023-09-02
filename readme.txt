Creating an asset management portfolio using Python and AI, specifically neural networks, is an advanced project that requires a deep understanding of both finance and machine learning. Here's a high-level overview of how you can approach this:

1. Data Collection:
Historical Data: Gather historical price data for the assets you're interested in. This can be stock prices, bond prices, commodities, etc. You can use APIs like Alpha Vantage, Yahoo Finance, or Quandl.
Fundamental Data: Information about the financial health of companies, economic indicators, etc.
Sentiment Data: News articles, financial reports, and social media can be used to gauge the sentiment around certain assets.
2. Data Preprocessing:
Normalization: Normalize price data to ensure that all assets are on a similar scale.
Feature Engineering: Create features that might be relevant for prediction, such as moving averages, RSI, MACD, etc.
Train/Test Split: Split your data into training and testing sets to validate the performance of your model.
3. Neural Network Model:
Architecture: Use a recurrent neural network (RNN) or long short-term memory (LSTM) network, as they are designed to work with sequential data like time series.
Training: Train your model on the training data.
Validation: Validate the model's performance on the test data.
4. Risk Assessment:
Portfolio Variance: Calculate the variance of the portfolio to assess its volatility.
Sharpe Ratio: Measure the risk-adjusted return of the portfolio.
5. Optimization:
Objective Function: The objective is to maximize potential income while minimizing risk. This can be done using the Sharpe Ratio or any other risk-adjusted performance measure.
Constraints: Set constraints such as not investing more than a certain percentage in a single asset, ensuring diversification, etc.
Optimization Algorithm: Use optimization algorithms like the Efficient Frontier, Genetic Algorithms, or Particle Swarm Optimization to find the optimal asset allocation.
6. Backtesting:
Once you have an optimal portfolio, backtest it using historical data to see how it would have performed.

7. Deployment:
If satisfied with the performance, you can deploy the model in a real-world environment. Ensure you have a mechanism to update the model as new data becomes available.

8. Monitoring and Maintenance:
Regularly monitor the portfolio's performance and retrain the model as necessary.

Challenges:
Overfitting: Neural networks can easily overfit to the training data, making them perform poorly on unseen data.
Noise: Financial data can be very noisy, and it's challenging to distinguish between genuine patterns and random noise.
Non-stationarity: Financial time series are non-stationary, meaning their statistical properties change over time.
Conclusion:
While neural networks offer a sophisticated approach to asset management, it's essential to be aware of their limitations and the complexities of financial markets. It's also crucial to combine AI models with domain knowledge in finance for the best results.