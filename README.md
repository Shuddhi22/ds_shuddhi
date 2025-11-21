# ds_shuddhi
Combines Crypto Fear & Greed Index data with detailed crypto trade execution logs. Includes sentiment values, classifications, timestamps, execution prices, trade sizes, fees, PnL, and transaction hashes. Useful for sentiment analysis, trading insights, and strategy development.

## How to Run This Notebook
--Open the Colab notebook using the link below.
https://colab.research.google.com/drive/11Xo6AYwhfJ2iFxYdmjuIm4PLZRJWoclh?usp=sharing


*Overview *:
Fear & Greed Index Data
– Tracks overall crypto market sentiment
– Includes timestamps, values, and sentiment classifications

Trade Execution Data:
– Detailed trading logs with execution price, size, fees, PnL, and on-chain transaction hashes
– Useful for studying execution quality, position tracking, and real-time trading behavior

Folder structure:
ds_shuddhi/
│
├── notebook_1.ipynb             
├── csv_files/                   
│     ├── fear_greed.csv
│     ├── historical_data.csv.zip
│     
├── outputs/                     
│     ├── graph 1.png
│     ├── graph2.png
│     ├── graph3.png
│     ├── graph4.png
│     ├── graph5.png
│     ├── graph6.png
│     ├── graph7.png
│     ├── graph8.png
│     ├── graph9.png
│     ├── graph10.png
│     ├── graph11.png
│     ├── graph12.png
│     └── correlation graph.png
│
├── ds_report.pdf                
└── README.md 

FEAR AND GREED COLUMN DISCRIPTION

| Column Name        | Description                                                                                               |
| ------------------ | --------------------------------------------------------------------------------------------------------- |
| **timestamp**      | Unix timestamp (in seconds) representing the exact date/time of the Fear & Greed reading.                 |
| **value**          | Numerical value of the Fear & Greed index (0–100). Lower = Fear, Higher = Greed.                          |
| **classification** | Market sentiment category based on the value (e.g., *Fear, Extreme Fear, Neutral, Greed, Extreme Greed*). |
| **date**           | Human-readable date converted from the timestamp (YYYY-MM-DD).                                            |


TRADE COLUMN DISCRIPTION

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

