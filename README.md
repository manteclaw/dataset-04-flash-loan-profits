# Flash Loan Profitability Dataset

## Overview
On-chain flash loan arbitrage profitability data on Base L2. Tracks borrow amounts, DEX price spreads, gas costs, net profit, and competition levels across 6 DEXs and 5 flash loan providers.

## Sample Data
- **Rows:** 25 (sample of full dataset)
- **Date range:** 2026-07-01 to 2026-07-25
- **Chains:** Base L2
- **DEXs:** Aerodrome, Uniswap V3, BaseSwap, SushiSwap, AlienBase, SwapBased

## Columns
| Column | Description |
|--------|-------------|
| date | Execution date |
| block_number | Block where flash loan executed |
| tx_hash | Transaction hash |
| flash_loan_provider | Aave V3, Balancer, Uniswap V3, MakerDAO, dYdX |
| borrowed_amount_usd | Flash loan size in USD |
| token_pair | Arbitraged trading pair |
| buy_dex | DEX where token was bought |
| sell_dex | DEX where token was sold |
| price_buy | Price at buy DEX |
| price_sell | Price at sell DEX |
| gross_profit_usd | Profit before gas |
| gas_cost_eth | Gas cost in ETH |
| gas_cost_usd | Gas cost in USD |
| net_profit_usd | Profit after gas |
| profitable | True if net profit > 0 |
| execution_time_ms | Time from borrow to repay |
| competition_level | low / medium / high |

## Use Cases
- Train MEV / arb detection models
- Analyze flash loan profitability trends
- Build gas estimation tools
- Study competition and market efficiency

## Full Dataset
Full dataset (500+ rows) available upon request.

---
Generated: 2026-08-17 | Base L2 Agent Data
