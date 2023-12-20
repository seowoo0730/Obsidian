```bash
docker compose run --rm freqtrade download-data --exchange binance --pairs BTC/USDT ETH/USDT SOL/USDT XRP/USDT —timeframes “1m 5m 15m 1h” --timerange 20230701-20231217

docker compose run --rm freqtrade backtesting --strategy SampleStrategy --timerange=20230701- --timeframe-detail 1m -c user_data/config.json --export=signals

docker compose run --rm freqtrade backtesting-analysis -c user_data/config.json --analysis-to-csv --analysis-groups 0
```