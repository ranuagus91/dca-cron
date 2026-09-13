# dca-cron

> dca · schedule · dip

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

DCA cron paper loop — interval buys, daily-loss switch.

## Features

- Default venue coinbase / BTCUSDT
- Built-in dca strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd dca-cron
python -m pip install -e .
python -m dcacron --help
```

## CLI Usage

```bash
dcacron backtest --bars 200
# Replay stub candles

dcacron paper
# Start a paper session

dcacron status
# Print engine state

dcacron orders
# List simulated fills
```

## Project Structure

```
dcacron/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `dcacron/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `coinbase` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `dca` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

Schedulers search dca-cron, not dca-bot.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![dca](https://img.shields.io/badge/dca-111827?style=flat-square) ![cron](https://img.shields.io/badge/cron-111827?style=flat-square) ![dca-cron](https://img.shields.io/badge/dca%20cron-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`dca` `cron` `dca-cron` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: dca-cron · dca · schedule · dip · DCA cron paper loop — interval buys, daily-loss switch.

---

<sub>DCA cron paper loop — interval buys, daily-loss switch.</sub>
