```bash
docker compose run --rm freqtrade download-data --exchange binance --pairs BTC/USDT ETH/USDT SOL/USDT XRP/USDT —timeframes “1m 5m 15m 1h” --timerange 20230701-20231217

docker compose run --rm freqtrade backtesting --strategy SampleStrategy --timerange=20230701- --timeframe-detail 1m > 

docker compose run --rm freqtrade plot-profit --export-filename user_data/backtest_results/.json --timeframe 1m
```
