# Binance Futures Trading Bot (Testnet)

## Overview

This project is a Python CLI-based trading bot that simulates placing MARKET and LIMIT orders on Binance Futures Testnet.

## Features

* Supports BUY and SELL orders
* MARKET and LIMIT order types
* Command-line interface (CLI)
* Input validation
* Logging of order execution
* Modular code structure

## Setup

```bash id="j0z9rd"
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run

### Market Order

```bash id="0o7x4u"
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001
```

### Limit Order

```bash id="h8q9k6"
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 60000
```

## Logs

All order activity is logged in `trading_bot.log`.

## Notes

* Uses Binance Futures Testnet
* Mock responses used when API access is unavailable
