# API Documentation

{% page-ref page="api-endpoints.md" %}

{% page-ref page="oracles.md" %}



**Find the right data for your needs**  
Show your users the most transparent data on the market with our API. Whether you're building a financial service, a portfolio management tool, a new media offering, or more, we have the most advanced and updated data on the market for your product.  
For Oracle usage see [Oracles in DIA](https://docs.diadata.org/documentation/api-1/oracles).

**Backtest your strategies**  
Use the most efficient and transparent crypto data to run simulations and backtest your trading or investing strategies. With crowd-aggregated hundreds of exchanges you can be sure that you're getting the right picture every single time.

**Run Experiments**  
Build your own models with our data, to further your interest or just for fun. With our flexible and powerful API, we provide you with a set of data that will help you draw insights and make conclusions.

**Request your data**  
Set a bounty on gitcoin.io or drop us a [line](mailto:API@diadata.org).

Version: 1.0

## API Access

The DIA base url is `https://api.diadata.org/v1`. All API paths are sub-paths of this base URL. You can find specific documentation for the endpoints of our API on the [API documentation site](https://docs.diadata.org/documentation/api-1/api-endpoints). 

Currently, DIA collects reference rates from traditional financial markets and data from several cryptocurrency exchanges \(see the table below\).

| Name | Number of Pairs | API link |
| :--- | :--- | :--- |
| Binance | [47](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/Binance.json) | [Binance API Documentation](https://binance-docs.github.io/apidocs/spot/en/#introduction) |
| Bitfinex | [25](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/Bitfinex.json) | [Bitfinex Websocket Documentation](https://docs.bitfinex.com/docs/ws-general) |
| Coinbase | [3](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/CoinBase.json) | [Coinbase v2 API](https://developers.coinbase.com/api/v2) |
| GateIO | [42](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/GateIO.json) | [Gate.io API Documentation](https://www.gate.io/api2) |
| HitBTC | [43](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/HitBTC.json) | [HitBTC API Browser](https://api.hitbtc.com/) |
| Huobi | [40](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/Huobi.json) | [Huobi API Documentation](https://huobiapi.github.io/docs/spot/v1/en/#introduction) |
| Kraken | [8](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/Kraken.json) | [Kraken Public API Documentation](https://www.kraken.com/features/api#public-market-data) |
| LBank | [20](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/LBank.json) | [LBank API Documentation](https://docs.lbkex.net/en/#introduction) |
| OKEx | [27](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/OKEx.json) | [OKEx API Documentation](https://www.okex.com/docs/en/) |
| Simex | [14](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/Simex.json) | [Simex API Documentation](https://simex.global/en/docs/introduction) |
| ZB.com | [127](https://github.com/diadata-org/diadata/tree/c982072de2ac488c5f0bdf32b677cbac1965583e/documentation/config/ZB.json) | [Zb.com API Documentation](https://www.zb.com/api) |

## Use cases

### Bash scripting

The API can be accessed through a Linux terminal by using curl. For example  
`curl https://api.diadata.org/v1/interestrate/ESTER/2020-03-16 >> userPath/myFile.txt`  
writes the return value of the GET request into `myFile.txt` for further processing.

### Usage with Python

The JSON object obtained in an API GET request complies with Python syntax. It can be cast into a list or dictionary resp. using Python's `eval(string)` function.

