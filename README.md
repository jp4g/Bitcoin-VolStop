# Bitcoin-VolStop
Pine Script Volatility Stop

Volatility Stop using Average True Range written in PineScript. 

Performance of Algorithm:
  - Model is fit to work with the BTC/USD trading pair (High performance). 
  - Moderate performance with large market capitalization pairs (ex. ETH/USD, XRP/USD).
  - Poor performance with cryptocurrencies under the top 5 market cap.
  - Poor performance in a down-trending cryptocurrency market.
     - Only trade on signals when trending upwards for maximum profitability (trade at your own discretion).
  - Has not been thoroughly tested with equities markets.
  
How to Use:
  a. How to run bitcoin_volstop_v1.txt
    1. Register with or login to TradingView at https://www.tradingview.com in order to run custom scripts.
    2. Copy ENTIRE bitcoin_volstop_v1.txt file
    3. Visit https://www.tradingview.com/symbols/BTCUSD/
    4. Select button "Full-featured chart"
    5. Select tab "Pine Editor" found on toolbar at the bottom of the screen
    6. Click within script editor panel (i.e. click on any line of code) 
    7. Press "CTRL" + "A" to select all text in the panel
    8. Press "CTRL" + "V" to paste bitcoin_volstop_v1 script into editor
    9. Select "Add to Chart" on the upper right section of the script panel
    10. Select tab "Strategy Tester" found at same toolbar as the previous "Pine Editor" tab
  b. Changing inputs
    1. On the leftmost toolbar at the very bottom, select the square with two bent lines beneath it ("Object Tree" menu)
    2. Locate BTC VolStop Signals(...). On the right side of the entry, select the middle button shaped like a gear
    3. Set beginning of backtest time period using "From" inputs and end of backtest time period using "To" inputs
    4. Set the average true range multiplier factor with "ATR Multiplier"
    5. Set the number of bars included in average true range with "ATR Lookback Period"
    6. Set Risk Reward Ratio with "Risk To Reward Multiplier"
    7. Set number of standard deviations applied to stops with "Stop Deviations"
    8. Set number of bars before standard deviation stoploss becomes trailing stoploss with "Bars Before Trailing Stop"
  c.  Possibly overfit 3200 % retuns Aug 2013 - Nov 2018
    1. ATR Multiplier = 4
    2. ATR Lookback Period = 7
    3. Risk to Reward Multiplier = 4
    4. Stop Deviations = 2
    5. Bars before trailing stops
    
