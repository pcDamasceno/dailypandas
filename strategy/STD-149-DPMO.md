Forget Everything You Think You Know About Scalping Trading Strategy
https://www.youtube.com/watch?v=dYvmLnnoF90

[b]-- Overview[/b]

A private strategy for backtesting purposes.
The "Std-149-dpmo" strategy, developed by DailyPanda, is designed for intraday trading on 5 and 15-minute charts to be used on BTC/U.S.Dollar. This strategy combines several technical analysis tools to create a robust trading system that aims to provide reliable buy and sell signals.

[b]-- Credit[/b]

This strategy is inspired by open-source indicators originally written by loxx and LazyBear. It leverages the idea of having some indicators and with additional features and customized inputs, enhances and builds good trading signals. Significant modifications and enhancements have been made to adapt these tools into a cohesive strategy, adding unique risk management and signal filtering mechanisms.

[b]How the components work together[/b]

This strategy uses the idea from STD-Filtered, N-Pole Gaussian Filter [Loxx] filter with adjusted filters of period 50, order 10, filter deviation 1, filter period 49. With that, the entry points are generated.

The oscillator is based on a Rate of Change calculation that is smoothed twice with custom exponential moving averages. It is used as a relative strength tool. For this trading strategy, we only care if it is above or below zero.


[b]-- Considerations[/b]

The strategy uses by default an initial capital of 2000 USD. The size of the contract is also based on that.

[b]-- Comission and Slippage[/b]

Comission and slippage values were chosen based on Binance values. Please check them and adjust to your current scenario (asset, broker) since they greatly affect the performance.
Commission: 0.02%
Slippage: 0.5%

[b]-- Key Features[/b]

This strategy leverages the following elements to build its entries.
[list]
[*]Ehlers Gaussian: Used for smoothing. It rejects high frequencies (fast movements)
[*]149-SMA: Acts as a long-term trend filter to validate signals.
[*]Price Momentum Oscillator (PMO): Helps identify momentum in the market.
[*]Swing High/Low Levels: Used for setting stop-loss and take-profit levels.
[/list]


[b]-- Inputs and Risk Management[/b]

The strategy includes customizable risk management parameters:

[list]
[*]Risk Reward Ratio: Defines the risk/reward ratio for each trade.
[*]Plot TP and SL: Plot the TP and SL on the graph for each operation.
[*]Lookback Period for Swing High/Low: Defines how many candles to look back for identifying swing points used for stop-loss.
[*]Start and Stop Trading Times: Set the hours during which the strategy can open new trades.
[*]% max Day DD: Once a % of the balance is lost, no more positions will be opened.
[*]Day % Goal: When hit x% of profit on the day, no more operations will be opened.
[*]Plot Oscillator: For each day, the oscillator will be scaled and be plotted on the graph to be able to double-check the entries.
[/list]

[b]-- How The Entries Work[/b]

This strategy will provide labels of entry signals for long and short based on the Gaussian filter.

LONG-- Initiated when a long signal is generated, the price is above the 149-SMA, and the PMO oscillator is above the central line. The stop-loss is set at the last swing low, and the take-profit is calculated based on the risk/reward ratio.

SHORT-- Initiated when a short signal is generated, the price is below the 149-SMA, and the PMO oscillator is below the central line. The stop-loss is set at the last swing high, and the take-profit is calculated based on the risk/reward ratio.

[b]-- Table of results[/b]

The strategy includes a performance table that breaks down results on a monthly basis, providing a clear view of equity development over time.
It also shows how much commission you have paid overall to understand better the impact it has on the performance.

[b]-- Conclusion[/b]

The "Std-149-dpmo" strategy is a tool for intraday traders looking to get new strategies and understand new tools and market analysis.