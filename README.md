# ds_shuddhi
Combines Crypto Fear &amp; Greed Index data with detailed trade execution logs. Includes sentiment scores, classifications, timestamps, prices, token sizes, fees, PnL, and transaction hashes. Useful for sentiment analysis, trading research, and strategy development.
COLUMN DISCRIPTION

| Column Name        | Description                                                                                               |
| ------------------ | --------------------------------------------------------------------------------------------------------- |
| **timestamp**      | Unix timestamp (in seconds) representing the exact date/time of the Fear & Greed reading.                 |
| **value**          | Numerical value of the Fear & Greed index (0–100). Lower = Fear, Higher = Greed.                          |
| **classification** | Market sentiment category based on the value (e.g., *Fear, Extreme Fear, Neutral, Greed, Extreme Greed*). |
| **date**           | Human-readable date converted from the timestamp (YYYY-MM-DD).                                            |


| Column Name          | Description                                                               |
| -------------------- | ------------------------------------------------------------------------- |
| **Account**          | The blockchain wallet address or exchange account ID used for the trade.  |
| **Coin**             | The trading pair or asset symbol (e.g., `@107`).                          |
| **Execution Price**  | The exact price at which the trade was executed.                          |
| **Size Tokens**      | Quantity of tokens bought or sold in the trade.                           |
| **Size USD**         | Dollar value of the order at execution (Size Tokens × Price).             |
| **Side**             | Indicates whether the order is a **BUY** or **SELL** trade.               |
| **Timestamp IST**    | Local timestamp (Indian Standard Time) when the trade was executed.       |
| **Start Position**   | Position size *before* the trade was executed.                            |
| **Position**         | Updated position size *after* the trade was executed.                     |
| **Direction**        | Trade direction (Buy / Sell).                                             |
| **Closed PnL**       | Realized profit or loss from this trade.                                  |
| **PnL**              | Profit or loss from the position (may show 0 if still open).              |
| **Transaction Hash** | On-chain transaction ID for blockchain-verified trades.                   |
| **Order ID**         | Internal order reference number given by the exchange.                    |
| **Crossed**          | Boolean (True/False): whether the order crossed the book (market order).  |
| **Fee**              | Trading fee charged for the execution.                                    |
| **Trade ID**         | Unique execution ID for the trade (exchange-specific).                    |
| **Timestamp**        | Unix timestamp of the trade (in scientific notation, e.g., 1.730000e+12). |

