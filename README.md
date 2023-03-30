## Binance Trading Bot in Python

The following Python script implements a mean reversion trading strategy to make profitable trades. A live price stream is fed in through the Binance WebSocket API which is stored in a continuously updated dataframe.

The script place a market buy order if the latest price (``last_price``) is above the n-second Simple Moving Average (SMA). Once it has an open position, it will place a market sell order if the latest price indicates a profit of ``target_profit`` or a loss of ``stop_loss``.
