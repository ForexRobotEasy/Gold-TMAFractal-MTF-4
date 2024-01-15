# Gold TMAFractal MTF 4 Indicator

This code is a custom indicator for MetaTrader 5 (MQL5) called Gold TMAFractal MTF 4. It is developed by the Forex Robot Easy Team and can be found on their website [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/gold-tmafractal-mtf-4-review-high-accuracy-forex-indicator/). Please note that ForexRobotEasy is not the official developer of this product and this code is provided as a sample that can work similarly to the described product.

## Indicator Description

The Gold TMAFractal MTF 4 indicator is designed to provide trading signals based on the TMA (Triangular Moving Average) and fractal indicators. It calculates the TMA and fractals for a specified period and timeframe and generates buy or sell signals based on confirmed arrow signals or fractal signals.

The indicator consists of two main buffers: `buffer_main` and `buffer_entry_zone`. The `buffer_main` buffer stores the type of signal (buy, sell, or no signal) while the `buffer_entry_zone` buffer stores the entry zone value for potential trades.

## Indicator Inputs

The indicator has two input parameters:

- `period`: Period for TMA calculation (default: 20)
- `timeframe`: Timeframe for analysis (default: H1)

## Indicator Initialization

During initialization, the indicator sets up the required buffers and labels for display. It maps the indicator buffers and sets their styles and labels.

## Indicator Calculation

The `OnCalculate` function is called to calculate the indicator values for each bar. It first checks if the TMA and fractal indicators have been calculated for the required number of bars. If not, it prints an error message and exits.

Next, it iterates through each bar and checks for confirmed arrow signals. If a confirmed signal is found, it stores the signal type and entry zone value in the respective buffers. If no confirmed signal is found, it calculates the fractal signal and stores it in the `buffer_main` buffer. The `buffer_entry_zone` buffer is set to 0 in this case.

The function returns the total number of calculated bars.

## Signal Confirmation

The `IsConfirmedSignal` function is called to check if a signal is confirmed or not. The logic for signal confirmation is not provided in the code and needs to be implemented separately.

## Signal Type Determination

The `GetSignalType` function is called to determine the type of signal (buy, sell, or no signal). The logic for determining the signal type is not provided in the code and needs to be implemented separately.

## Entry Zone Calculation

The `GetEntryZone` function is called to calculate the entry zone for potential trades. The logic for calculating the entry zone is not provided in the code and needs to be implemented separately.

## Fractal Signal Calculation

The `GetFractalSignal` function is called to calculate the fractal signal. The logic for calculating the fractal signal is not provided in the code and needs to be implemented separately.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/gold-tmafractal-mtf-4-review-high-accuracy-forex-indicator/).
