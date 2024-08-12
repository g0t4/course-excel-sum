## Gold Stock Prices

- https://www.kaggle.com/datasets/sahilwagh/gold-stock-prices
- `Apache License, Version 2.0`:
  - [LICENSE-2.0.txt](./LICENSE-2.0.txt)
  - originals: [html](https://www.apache.org/licenses/LICENSE-2.0) and [txt](https://www.apache.org/licenses/LICENSE-2.0.txt)
- I downloaded version `3` on 2021-08-12
- Based on [Nasdaq GC:CMX Futures](https://www.nasdaq.com/market-activity/commodities/gc-cmx)
  - FYI get the data here too:
    - https://www.nasdaq.com/market-activity/commodities/gc-cmx/historical (select a time period and click Download link)
  - Contract specs
    - https://www.cmegroup.com/markets/metals/precious/gold.contractSpecs.html
  - price is quoted as $ per troy ounce
  - volume is in contracts, where 1 contract = 100 troy ounces
    - IOTW price per 1 contract = ($ per troy ounce \* 100)
    - IOTW 100 \* volume = volume in troy ounces

## subsets

```bash

# ten-days subset:
cat "goldstock v2.csv" | head -11 > subsets/goldstock-ten-days.csv

```
