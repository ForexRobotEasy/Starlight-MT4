# Starlight MT4 ReadMe

This code is for the Starlight MT4 Forex robot, developed by Forex Robot Easy Team. It is an advanced low-risk night scalper with a unique entry algorithm. For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/review-starlight-mt4-advanced-low-risk-night-scalper-with-unique-entry-algorithm/).

## Input Parameters

1. **StopLoss** - The stop loss value for each trade.
2. **TakeProfit** - The take profit value for each trade.
3. **MaxSpread** - The maximum allowed spread for entering trades.
4. **Slippage** - The maximum allowed slippage for entering trades.

## Currency Pairs

The following currency pairs are defined for trading:

- EURUSD
- GBPUSD
- AUDCAD
- EURAUD
- EURCAD
- GBPAUD
- GBPCAD
- USDCAD
- EURGBP
- USDCHF
- GBPCHF
- EURCHF
- CHFJPY

## Entry Algorithm

The entry algorithm of the Starlight MT4 Forex robot is unique and must be implemented by the user. The function `uniqueEntryAlgorithm()` should be modified to include the custom entry conditions. It should return `true` if the entry condition is met, otherwise `false`.

## Mean Reverse Strategy

The mean reverse strategy should be implemented in the function `meanReverseStrategy()`. It should include the logic for opening and closing trades based on the strategy.

## Compatibility Check

The function `isCompatible()` checks if the current currency pair is compatible for trading. It compares the current currency pair with the defined list of currency pairs. If a match is found, it returns `true`, otherwise `false`.

## Low Risk Check

The function `isLowRisk()` checks if the current trade is low risk. The logic for determining low risk should be implemented in this function. It should return `true` if the trade is low risk, otherwise `false`.

## Entry Point

The `start()` function is the entry point of the EA. It loops through all the defined currency pairs and performs the following steps for each pair:

1. Check if the currency pair is compatible.
2. Check if the unique entry condition is met.
3. Execute the mean reverse strategy.
4. Check if the trade is low risk.
5. Place the trade based on the algorithm.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please use MQL5.
