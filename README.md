# TRS Model Portfolio — data feed

Published CSV feed for the **Total Return Strategy Model Portfolio**
(James A. Kostohryz · JK Investment Consulting).

| file | contents |
|---|---|
| `data/positions.csv`    | current holdings — shares, FIFO cost basis, mark, weight, P&L |
| `data/transactions.csv` | full trade ledger |
| `data/income.csv`       | deposits, dividends and interest |
| `data/dashboard.csv`    | NAV, cash, return and allocation as key/value pairs |
| `data/meta.csv`         | generation timestamp and coverage dates |

**Cost basis is FIFO**, which ties to the broker's Price Paid to the cent.
Average cost is never used.

The TRS model portfolio holds **no options and no margin**. It is the long-only
equity sleeve of a larger real account that trades both; options, margin interest
and margin transfers are excluded by construction.

These files are generated. Check `meta.csv` for freshness before relying on them.
