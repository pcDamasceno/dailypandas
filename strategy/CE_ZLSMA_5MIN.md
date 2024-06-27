[b]-- Overview[/b]

The "CE_ZLSMA_5MIN_CANDLECHART" strategy, developed by DailyPanda, is a comprehensive trading strategy designed for analyzing trading on 5-minute candlestick charts.
It aims to use some indicators calculated from a Hekin Ashi chart, while running it on a normal candlestick chart, making sure that [b]no price distortion affects the strategy results[/b].

It also brings a feature to show, on the candlestick chart, where the entries would take place on the HA chart, to also be able to study the effect that the price distortion would make on your backtest.

[b]-- Credit[/b]

The code in this script is based on open-source indicators originally written by veryfid and everget, I've made significant changes and additions to the scripts but all credit for the idea goes to them, I just built on top of it:

[b]-- Key Features[/b]
It incorporate already built indicators (ZLSMA) and CandelierExit (CE)

[b]-- Zero Lag Least Squares Moving Average (ZLSMA) - by veryfid[/b]
The ZLSMA is used to detect trends with minimal lag, improving the accuracy of entry and exit signals.
It incorporates a double-smoothed linear regression to minimize lag and enhance trend-following capabilities.
Buy signals are generated when the price closes above the ZLSMA together with the CE signal.
It is calculated based on the HA candlestick pattern.


[b]-- Chandelier Exit (CE) - by everget[/b]
The Chandelier Exit indicator is used to dynamically manage stop-loss levels based on the Average True Range (ATR).
It ensures that stop-loss levels are adaptive to market volatility, protecting profits and limiting losses.
The ATR period and multiplier can be customized to fit different trading styles and risk tolerances.
It is calculated based on the HA candlestick pattern.

[b]-- Heikin Ashi Candles[/b]

The strategy leverages Heikin Ashi candlesticks to be able identify trends more clearly and leverage this to stay on winning trades longer.
Traders can choose to display Heikin Ashi candlesticks and order fills on the chart for better visualization.

[b]-- Risk Management[/b]

The strategy includes multiple risk management options to protect traders' capital.
Maximum intraday loss limit based on a percentage of equity.
Maximum stop-loss in points to filter out entries with excessive risk.
Daily profit target to stop trading once the goal is achieved.
Options to use fixed contract sizes or dynamically adjust based on a percentage of equity.
These features help traders manage risk and ensure sustainable trading practices.
Moving Averages

Several moving averages (EMA 9, EMA 20, EMA 50, EMA 72, EMA 200, SMA 200, and SMA 500) are plotted to provide additional context and trend confirmation.
A "Zone of Value" is highlighted between the EMA 200 and SMA 200 to identify potential support and resistance areas.

[b]-- Customizable Inputs[/b]

The strategy includes various customizable inputs, allowing traders to tailor it to their specific needs.
Start and stop trading times.
Risk management parameters (e.g., maximum stop-loss, daily drawdown limit, and daily profit target).
Display options for Heikin Ashi candles and moving averages.
ZLSMA length and offset.

[b]-- Usage[/b]

[b]-- Setting Up the Strategy[/b]
Configure the start year for the strategy and the trading hours using the input fields. The first candle of each day will be filled black for easy identification, while candles that are outside the allowed time range will be filled purple.

Customize the risk management parameters to match your risk tolerance and trading style.
Enable or disable the display of Heikin Ashi candlesticks and moving averages as desired.

[b]-- Interpreting Signals[/b]
Buy signals are indicated by a "Buy" label when the Heikin Ashi close price is above the ZLSMA and the Chandelier Exit indicates a long position.
The strategy will automatically enter a long position with a stop-loss level determined the swing low.
Positions are closed when the close price falls below the ZLSMA.

[b]-- Risk Management[/b]

The strategy monitors the maximum intraday loss and stops trading if the loss limit is reached.
If enabled, also stops trading once the daily profit target is achieved, helping to lock in gains.
You have the option to filter operations based on a maximum accepted stop-loss level, based on your risk tolerance.
You can also operate with a fixed amount of contracts or dynamically adjust it based on your allowed risk per trade, ensuring optimal protection of capital.

[b]-- Visual Aids[/b]

The strategy plots various moving averages to provide additional trend context.
The "Zone of Value" between the EMA 200 and SMA 200 highlights potential support and resistance areas.

Heikin Ashi candlesticks and order fills can be displayed to enhance the difference this strategy would take if you were to backtest it on a Heikin Ashi chart.

[b]-- Table of results[/b]
This strategy also breaks down the results on a monthly basis for better understanding of your capital development along the way.

[b]-- Conclusion[/b]

The "CE_ZLSMA_5MIN_CANDLECHART" strategy is a tool for intraday traders looking to understand and leaverage the Heikin Ashi chart while still using the normal candle chart. Traders can customize the strategy to fit their specific needs, making it a versatile addition to any trading toolkit.