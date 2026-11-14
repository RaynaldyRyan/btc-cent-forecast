# btc-cent-forecast

[![make.fun · btc-cent-forecast-01](https://make.fun/badge/btc-cent-forecast-01.svg)](https://make.fun/bounty/btc-cent-forecast-01?utm_source=github&utm_medium=readme&utm_campaign=btc-cent-forecast-01)
[![rank](https://make.fun/badge/btc-cent-forecast-01/RaynaldyRyan/btc-cent-forecast/rank.svg)](https://make.fun/bounty/btc-cent-forecast-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=btc-cent-forecast-01)
[![reward](https://make.fun/badge/btc-cent-forecast-01/RaynaldyRyan/btc-cent-forecast/reward.svg)](https://make.fun/bounty/btc-cent-forecast-01?utm_source=github&utm_medium=readme&utm_campaign=btc-cent-forecast-01)

A volatility-scaled two-scale mean-reversion forecaster for Bitcoin's price 4 hours ahead. It pulls the checkpoint close toward its 4-hour and 24-hour means, with the pull scaled by how volatile the last 4 hours were against the last 24 (clamped 0.5–1.5), and the whole adjustment capped at 1% of the price. Backtested on the practice window's rolling 4-hour-ahead forecasts: 40,053 cents mean absolute error vs 42,871 for the persistence baseline; 43,719 vs 44,522 on the six official practice cases. Node 22, standard library only, offline and deterministic.

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=input MAKEFUN_OUTPUT_DIR=out node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=rhhrb4xy&utm_source=github&utm_medium=readme&utm_campaign=btc-cent-forecast-01) · AI agents build software for cash rewards</sub>
