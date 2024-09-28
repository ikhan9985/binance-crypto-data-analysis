# Binance Crypto Data Analysis
This project retrieves cryptocurrency data from Binance API and performs calculations based on the price and candlestick information. The code is divided into three cells, each performing different analyses on selected cryptocurrency symbols.

# Project Overview
The script fetches real-time and historical price data for the following cryptocurrency pairs:

- ETH/USDT (Ethereum)
- BTC/USDT (Bitcoin)
- SOL/USDT (Solana)
- BNB/USDT (Binance Coin)

## Three different sets of calculations are performed:

1. Current Prices: Fetches the latest prices of the cryptocurrencies.
2. Highest Gain and Loss: Retrieves 500 historical daily candles for each symbol and calculates the highest gain and loss.
3. Historical Analysis: Fetches data within a specific time period and calculates the highest and lowest points, as well as the biggest gains and losses.

## Files in the Repository
getCrypto.ipynb: The main script containing the three cells of code.

API Endpoints Used
Price Ticker: Fetches the latest price for each cryptocurrency pair.

URL: https://api.binance.com/api/v3/ticker/price
Kline (Candlestick): Retrieves historical candlestick data for calculating gains, losses, and price ranges.

URL: https://api.binance.com/api/v3/klines

# Example Output

## Current Prices:

ETHUSDT: 1634.35
BTCUSDT: 22726.52
SOLUSDT: 22.82
BNBUSDT: 322.1

## Highest Gain and Loss:

ETHUSDT: highest gain = 483.28, highest loss = -364.03
BTCUSDT: highest gain = 5233.84, highest loss = -5460.92
SOLUSDT: highest gain = 23.89, highest loss = -22.56
BNBUSDT: highest gain = 60.1, highest loss = -49.1

## Historical Analysis:

ETHUSDT: highest point = 1714.68, lowest point = 1190.57, biggest gain = 150.84, biggest loss = 9.79
BTCUSDT: highest point = 24255.0, lowest point = 16499.01, biggest gain = 1894.65, biggest loss = 73.91
SOLUSDT: highest point = 26.8, lowest point = 9.69, biggest gain = 6.55, biggest loss = 0.4
BNBUSDT: highest point = 337.8, lowest point = 240.7, biggest gain = 24.3, biggest loss = 2.6

## Requirements
Python 3.x
Requests Library
You can install the dependencies by running:

pip install requests
