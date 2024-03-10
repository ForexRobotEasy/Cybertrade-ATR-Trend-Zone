# Cybertrade ATR Trend Zone

This is a custom indicator developed by [ForexRobotEasy](https://forexroboteasy.com/forex-robot-review/cybertrade-atr-trend-zone-unbiased-forex-software-review/) for MetaTrader 5 (MQL5). The Cybertrade ATR Trend Zone indicator calculates the Average True Range (ATR) values and determines the trend direction based on the ATR values.

## Indicator Parameters
- `period` (default = 14): ATR period

## Indicator Initialization
The `OnInit()` function is responsible for initializing the indicator. The ATR buffer is mapped to index 0, and the indicator style is set to draw a line. The indicator label is set as 'Cybertrade ATR Trend Zone'.

## Indicator Calculation
The `OnCalculate()` function is called for each new incoming tick to calculate the ATR values and determine the trend direction. 

First, the ATR buffer is set as a series to ensure proper calculations. If the number of bars is less than the specified period, the function returns 0.

Next, the ATR values are calculated using the `iATR()` function for the specified symbol and period. The calculated ATR value is then assigned to the respective index of the ATR buffer.

After calculating the ATR values, the trend direction is determined by comparing the current ATR value with the previous ATR value. If the current ATR value is greater than the previous ATR value, the trend direction is considered upward. If the current ATR value is less than the previous ATR value, the trend direction is considered downward. Otherwise, the trend direction is considered ranging.

Finally, the trend direction is printed on the chart using the `Comment()` function.

## Product Description
The Cybertrade ATR Trend Zone is an unbiased forex software that utilizes the Average True Range (ATR) indicator to determine the trend direction. This indicator can be used in MetaTrader 5 (MQL5) to assist traders in identifying potential market trends and making informed trading decisions.

The indicator calculates the ATR values based on the specified period and compares the current ATR value with the previous ATR value to determine the trend direction. The trend direction can be either upward, downward, or ranging.

Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [ForexRobotEasy](https://forexroboteasy.com/forex-robot-review/cybertrade-atr-trend-zone-unbiased-forex-software-review/).
