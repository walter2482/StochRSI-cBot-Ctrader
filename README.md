
# StochRSI-cBot-Ctrader
This C# trading robot uses cAlgo API for automated trading, employing indicators like Stochastic and RSI. It opens/closes positions based on indicators and applies risk management (stop loss, trailing stop, max drawdown). This cBot works fine in EURUSD 1h timeframe and 4h timeframe in others forex instruments.

## AEWMABot - cAlgo Robot

This C# robot, named "AEWMABot," is designed for automated trading in the cAlgo trading platform. It includes various parameters for risk management and trading strategies. Users can customize settings such as lot quantity, grid distance, and more.

### Risk Management Parameters

- **Lot Quantity:** Determines the lot size for trading.
- **Grid Distance:** Sets the distance between grid levels.
- **Stop Loss in Pips:** Specifies the stop loss in pips. (Recommendation: Consider setting this to 0 as the system closes positions on signal crosses.)
- **Max Spread:** Defines the maximum allowable spread.
- **Max Drawdown by Operation (%):** Sets the maximum drawdown percentage per trade.
- **Include Trailing Stop:** Enables or disables trailing stop functionality.
- **Trailing Stop Trigger (pips):** Sets the trigger distance for trailing stop.
- **Trailing Stop Step (pips):** Specifies the step size for trailing stop.
- **Maximum Number of Consecutive Losses:** Limits the consecutive losing trades.

### Grid System Parameters

- **Maximum Number of Positions:** Sets the maximum number of open positions.
- **Grid Size:** Defines the size of the grid.
- **Minimum Grid Distance (pips):** Specifies the minimum distance between grid orders.

### Momentum Indicator Parameters

- **RSI Periods:** Sets the RSI (Relative Strength Index) period.
- **Stochastic %K Periods:** Defines the Stochastic %K period.
- **Stochastic %D Periods:** Defines the Stochastic %D period.
- **Slow %K Periods:** Specifies the slow %K period.
- **Smoothing Speed:** Sets the speed of smoothing.
- **Threshold Buy:** Sets the buy threshold value.
- **Threshold Sell:** Sets the sell threshold value.

The robot utilizes the StochasticRSIEWMASmoothing indicator for trading decisions based on momentum indicators. It opens and closes positions while considering risk management rules such as stop loss (recommended setting: 0 and max operations 3), trailing stop, and maximum drawdown. The robot is designed to automate trading in the financial markets.

![image](https://github.com/walter2482/cBot-s-Ctrader/assets/93685420/20ac71cd-91a4-4603-9ef0-16f28fc40dc1)



## StochasticRSIEWMASmoothing Indicator

This C# indicator, named "StochasticRSIEWMASmoothing," is designed for financial market analysis in the cAlgo trading platform. It calculates the Stochastic RSI, a technical indicator, by combining the Relative Strength Index (RSI) with stochastic calculations. Users can customize parameters such as RSI periods, stochastic periods, and smoothing speed. The indicator provides two output series: "Stochastic RSI" and "Signal," aiding traders in making informed decisions based on market conditions and trends.


# RSICross - cAlgo Robot

The "RSICross" cAlgo robot is a C# trading algorithm designed for automated trading in the cAlgo platform. This robot utilizes the Relative Strength Index (RSI) crossover strategy to make trading decisions. Users can customize various settings to tailor their trading strategy.

### Data Settings

- **Source:** Select the data series source for the RSI calculation.

### Indicator Settings

- **RSI Periods - Buy:** Set the RSI period for buy signals.
- **RSI Periods - Sell:** Set the RSI period for sell signals.

### Threshold Settings

- **RSI Overbought Threshold - Buy:** Define the overbought threshold for buy signals.
- **RSI Oversold Threshold - Buy:** Define the oversold threshold for buy signals.
- **RSI Overbought Threshold - Sell:** Define the overbought threshold for sell signals.
- **RSI Oversold Threshold - Sell:** Define the oversold threshold for sell signals.

### Trade Settings

- **Volume:** Specify the trading volume for positions.
- **Max Spread:** Set the maximum allowable spread for trading.

### Trading Hours

- **Start Hour:** Define the start hour for trading.
- **End Hour:** Define the end hour for trading.

### Risk Management

- **Max Drawdown Threshold (%):** Specify the maximum drawdown threshold as a percentage of equity.

The robot opens buy positions when the RSI crosses below the oversold threshold and opens sell positions when the RSI crosses above the overbought threshold. It incorporates risk management by monitoring drawdown and closing positions when the drawdown exceeds the specified threshold. This robot is designed to automate trading in the financial markets.
