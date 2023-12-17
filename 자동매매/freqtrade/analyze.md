## Plotting
```bash
docker compose run --rm freqtrade plot-dataframe --strategy AwesomeStrategy -p BTC/ETH --timerange=20180801-20180805
```
## jupyter
```bash
docker compose -f docker/docker-compose-jupyter.yml up
```
`https://127.0.0.1:8888/lab`