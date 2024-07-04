Forget Everything You Think You Know About Scalping Trading Strategy
https://www.youtube.com/watch?v=dYvmLnnoF90

[b]-- Overview[/b]

A private strategy for backtesting purposes.
The "Std-149-dpmo" strategy, developed by DailyPanda, is designed for intraday trading on 5 and 15 minute charts to be used on BTC/U.S.Dollar. This strategy combines several technical analysis tools to create a robust trading system that aims to provide reliable buy and sell signals.

[b]-- Considerations[/b]
The strategy uses by default an initial capital of 2000 USD. The size of contract is also based on that.
No comission and slippage were added by default, since the idea behind this strategy is to perform backtesting purposes only.


[b]-- Credit[/b]

This strategy is inspired upon open-source indicators originally written by loxx and LazyBear. It leaverages on the idea of having some indicators and with additional features and customized inputs, enhance and build good trading signals. Significant modifications and enhancements have been made to adapt these tools into a cohesive strategy, adding unique risk management and signal filtering mechanisms.
Since

[b]-- Key Features[/b]
This strategy leaverages the following elements to build its entries.
[list]
[*]Ehlers Gaussian: Used for smoothing. It rejects high frequencies (fast movements)
[*]149-SMA: Acts as a long-term trend filter to validate signals.
[*]Price Momentum Oscillator (PMO): Helps identify momentum in the market.
[*]Swing High/Low Levels: Used for setting stop-loss and take-profit levels.
[/list]


[b]-- Risk Management[/b]

The strategy includes customizable risk management parameters:

Lookback Period for Swing High/Low: Defines the period for identifying swing points used for stop-loss.
Trading Time Window: Allows users to specify the hours during which the strategy can open new positions.


[b]-- Customizable Inputs[/b]

Traders can adjust the following inputs to tailor the strategy to their preferences:
[list]
[*]Risk Reward Ratio: Defines the risk/reward ratio for each trade.
[*]Start and Stop Trading Times: Set the hours during which the strategy can open new trades.
[*]Plot Exits: Option to display take-profit and stop-loss levels on the chart.
[/list]

[b]-- Interpreting Signals[/b]

Thi strategy will provide labels of entry signals for long and short based on the Gaussian filter.
It will also filter based on the 149-SMA and the oscilator.
LONG [b]-- Initiated when a long signal is generated, price is above the 149-SMA, and the PMO oscilator is positive. The stop-loss is set at the last swing low, and the take-profit is calculated based on the risk/reward ratio.

SHORT [b]-- Initiated when a short signal is generated, price is below the 149-SMA, and the PMO oscilator is negative. The stop-loss is set at the last swing high, and the take-profit is calculated based on the risk/reward ratio.


[b]-- Table of results[/b]

The strategy includes a performance table that breaks down results on a monthly basis, providing a clear view of equity development over time.


[b]-- Conclusion[/b]

The "Std-149-dpmo" strategy is a tool for intraday traders looking to get new new strategies and understand new tools and market analysis.