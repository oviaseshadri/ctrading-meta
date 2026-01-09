# cTrading – Theta Screener Reference

This repository provides a **reference walkthrough and documentation** for the **Theta Screener (cTrading MVP)**, a lightweight analytics dashboard built on top of ThetaSwap market data.

The focus of this project is to clarify **product scope, developer-facing surfaces, and known limitations** of the current implementation, based on a direct code walkthrough.

---

## Project Overview

**Theta Screener** functions as a **read-only market discovery and routing interface**. It surfaces token and swap data from ThetaSwap and delegates trade execution externally.

This repository does **not** modify or extend core product logic. Instead, it documents how the existing MVP behaves and how developers might reason about or build on top of it.

---

## Documentation

Lightweight reference documentation is available under `/docs` and is publicly hosted for ease of access:

https://oviaseshadri.github.io/ctrading-devrel-evaluation/

The documentation covers:

- Product boundaries and intended behavior  
- Observed ThetaSwap API usage  
- Local setup and expected runtime behavior  
- Known issues and current MVP limitations  

All documentation is **observational**, based on reviewing the codebase, and should not be treated as official protocol documentation.

---

## Key Observations

- Theta Screener is designed as a **market data and analytics UI**, not a trading terminal  
- Wallet connection and swaps are handled externally via **ThetaSwap**  
- Several UI elements would benefit from clearer labeling to improve developer and user experience  
- Explicit documentation significantly improves onboarding clarity for new contributors  

---

## Disclaimer

This repository reflects observations from a specific version of the Theta Screener MVP.  
APIs, behavior, and implementation details may change over time.

---

## Maintainer

Ovia Seshadri  
Developer Relations / Blockchain Engineer  
https://github.com/oviaseshadri
