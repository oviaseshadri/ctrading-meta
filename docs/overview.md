# Product Overview

## What Theta Screener Is

Theta Screener is a lightweight analytics dashboard that surfaces:
- Token lists
- Price, liquidity, and volume metrics
- Recent swap activity

It acts as a **market discovery and routing UI**, not a trading terminal.

## What Theta Screener Is Not

- Not an SDK
- Not a smart contract interface
- Not a swap executor
- Not a wallet-integrated dApp

All swap execution happens on **ThetaSwap**, which this app links to externally.

## Intended Audience

- Developers exploring the Theta ecosystem
- Builders looking for a reference UI for market data visualization
- Teams looking for a starter template for analytics dashboards

## Architecture Boundary (Observed)

- **Frontend:** React-based dashboard UI
- **Data Source:** ThetaSwap public APIs and token metadata assets
- **Execution:** Redirect to ThetaSwap
