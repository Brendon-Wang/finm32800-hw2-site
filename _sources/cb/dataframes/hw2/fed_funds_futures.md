# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures

Daily bars (ohlcv-1d schema) from the CME Globex dataset GLBX.MDP3, pulled with parent symbology (ZQ.FUT) so every listed ZQ contract is included. Columns: date (trading date), symbol, open, high, low, close, volume. The symbols include calendar spreads such as ZQU6-ZQZ6 alongside outright monthly contracts such as ZQU6; keep only the outrights before using prices. A contract settles at 100 minus the average daily effective fed funds rate over its month, so 100 minus the close is the market's forecast of that average.


## DataFrame Glimpse

```
Rows: 11862
Columns: 7
$ date   <datetime[ns]> 2026-10-23 00:00:00
$ symbol          <str> 'ZQZ6'
$ open            <f64> 95.965
$ high            <f64> 95.965
$ low             <f64> 95.945
$ close           <f64> 95.965
$ volume          <u64> 12677


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Monetary Policy, Futures, Fed Funds                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento API via Python                                                   |
| Data available up to (min)     | 2026-10-23 00:00:00                                                             |
| Data available up to (max)     | 2026-10-23 00:00:00                                                             |
| Dataframe Path                 | /Users/freshstart/Documents/FINM32800/hw2-Brendon-Wang/_data/fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file:///Users/freshstart/Documents/FINM32800/hw2-Brendon-Wang/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-24 14:09:11           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

