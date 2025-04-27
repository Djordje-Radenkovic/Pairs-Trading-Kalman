# Pairs Trading Strategy (CAC40 + EuroStoxx 50)

A Python project implementing a **pairs trading strategy** on **CAC40** and **EuroStoxx 50** stocks based on **cointegration test**, **linear model**, and **Kalman filter** beta prediction.

## Features
- ✅ Identifies cointegrated stock indices
- ✅ Builds a **simple linear model** to estimate relationship between two indices
- ✅ Uses **Kalman Filter** to dynamically update today's beta
- ✅ Detects divergences when beta moves out of bounds
- ✅ Executes strategy: **Short outperformer, Long underperformer**
- ✅ Aims to capture profits on mean reversion

## How It Works
1. Test pairs of stock indices for cointegration
2. Model relationship with linear regression
3. Apply Kalman filter to update beta estimate daily
4. When beta deviates outside set thresholds:
   - Short the stock that outperformed
   - Long the stock that underperformed
5. Close positions once spread reverts

## Requirements
- Python 3.8+
- `numpy`
- `pandas`
- `matplotlib`

## Disclaimer
This is a research project. Not financial advice. Trade at your own risk.
