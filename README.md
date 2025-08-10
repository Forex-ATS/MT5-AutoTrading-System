# MT5 Auto Trading System (Expert Advisor)
This project provides an automated trading system for the MetaTrader 5 platform built on a price action breakout strategy.

> **Forex ATS** stands for "Automated Trading System".
> For more information and updates, visit www.forexats.com.

## Requirements
- MetaTrader 5 (latest version)
- Copy the files into the appropriate MQL5 folders:
  - Experts/ → put `MyEA.mq5`
  - Indicators/ → put supporting indicators
  - Include/ → put helper files

## Installation
1. Open MetaTrader 5 → File → Open Data Folder.
2. Copy the files to their respective paths (`MQL5/Experts`, `MQL5/Indicators`, `MQL5/Include`).
3. Restart the platform or refresh the Navigator.
4. Drag the expert to the chart and enable "Allow Algo Trading".

## Settings
- Example preset: `presets/example.set` (do not upload sensitive data).

## How it Works (TL;DR)
- Enters trades according to the following conditions:
  - The EA looks for H1 candle breakouts aligned with the dominant H4 and D1 trends.
- Risk management:
  - Fixed risk [%] of the balance per trade.
  - SL/TP based on ATR, recent highs/lows, or other configurable criteria.
- Trailing:
  - Optional trailing stop can be enabled in the code if desired.

## Roadmap
- [ ] Improve trade management
- [ ] Support additional time frames
- [ ] Perform backtesting and forward testing

## License
See the LICENSE file for license information.
