# AutoPilotYield
![AutoPilotYield logo](assets/logo.png)

**AIが複数チェーンの利回りを自動で巡回・運用する不労所得ボルト**

## Overview

AutoPilotYield is a Solana-based vault managed by an autonomous AI agent. Users deposit assets once, and the agent continuously analyzes yield opportunities across multiple chains, automatically rebalancing funds to capture the best risk-adjusted returns — no manual monitoring required.

## Problem

Manually tracking and rebalancing yield across multiple chains is time-consuming and requires deep DeFi expertise. Rates shift constantly, and most users don't have the time, tools, or knowledge to move funds between chains to chase the best returns.

## Solution

An AI agent monitors on-chain yield data across chains and autonomously moves funds through a Solana vault using cross-chain bridges to capture the best returns. Users simply deposit, pick a risk profile, and let the agent handle the rest.

## Features (MVP)

- Solana vault contract accepting deposits/withdrawals
- AI agent scoring yield opportunities across 2-3 chains via oracle/API data
- Automated cross-chain rebalancing using a bridge (e.g. Wormhole)
- Dashboard showing current allocation, APY, and AI rebalancing history
- Risk profile selector (conservative/balanced/aggressive)

## Tech Stack

- Anchor, Rust (Solana vault program)
- Wormhole SDK (cross-chain messaging)
- Python / LLM agent (yield scoring and decision-making)
- Node.js backend (orchestration)
- React dashboard (frontend)
- Chainlink or Pyth oracle (on-chain data)

## How It Works

```
User
 |
 v
Solana Vault (Anchor/Rust) <---- deposits/withdrawals
 |
 v
AI Agent (Python/LLM) ---- scores yield via Chainlink/Pyth + APIs
 |
 v
Wormhole Bridge ---- moves funds Solana <-> Ethereum
 |
 v
React Dashboard ---- shows allocation, APY, rebalancing history
```

1. User deposits into the Solana vault and selects a risk profile.
2. The AI agent scores yield opportunities across chains using oracle/API data.
3. When a better risk-adjusted opportunity is found, the agent triggers a rebalancing transaction via Wormhole.
4. The vault contract updates allocations on-chain.
5. The dashboard reflects current allocation, APY, and the full history of AI decisions.

## Roadmap

- Integrate more chains and yield protocols for broader coverage
- Add backtesting and strategy performance audits for trust
- Launch tokenized shares of the vault for liquidity and composability

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- Name — Role (placeholder)
- Name — Role (placeholder)
- Name — Role (placeholder)

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)
