# API Surface (Observed from Code Usage)

> This page documents public endpoints **as observed from this repository**.
> It is **not official ThetaSwap API documentation**.

## ThetaSwap Market Data Endpoints

### GET /swap/top-tokens

**URL**
https://swap-api.thetatoken.org/swap/top-tokens

**Used for**
- Token list population
- Price, liquidity, and volume columns
- Filtering tokens with non-zero liquidity

---

### GET /swap/top-pairs

**URL**
https://swap-api.thetatoken.org/swap/top-pairs

**Used for**
- Pair-level metadata (server-side)

**Note**
- Endpoint exists in the backend but is not fully surfaced in the UI.

---

### GET /swap/pair/{pairAddress}/transactions

**Example**
https://swap-api.thetatoken.org/swap/pair/{PAIR_ADDRESS}/transactions

**Used for**
- Recent swap transaction table
- Buy / Sell direction
- USD value calculations

**Observed behavior**
- Transactions appear tied to a single hardcoded pair in the current MVP.

---

## Token Metadata and Assets

### Wallet Metadata JSON
https://assets.thetatoken.org/wallet-metadata/v1/data.json

### Token Logo Assets
https://assets.thetatoken.org/tokens/{symbol}.png

---

## Explorer Links
https://explorer.thetatoken.org/txs/{transactionHash}

---

## Rate Limits and Reliability

- Rate limits are **not documented**
- No retry, caching, or backoff logic observed in this repo

**Recommended improvements**
- Cache token lists
- Handle 429 responses gracefully
