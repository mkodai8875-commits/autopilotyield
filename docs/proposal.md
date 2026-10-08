# AutoPilotYield

_AIが複数チェーンの利回りを自動で巡回・運用する不労所得ボルト_

## Summary

Users deposit assets into a Solana-based vault, and an AI agent continuously analyzes yield opportunities across multiple chains via cross-chain messaging, automatically reallocating funds to the best risk-adjusted returns. The agent executes rebalancing transactions autonomously, giving users hands-off passive income without needing to monitor markets themselves.

## Target users

Busy professionals, crypto beginners, and large holders who want hands-off multi-chain yield exposure

## Problem

Manually tracking and rebalancing yield across multiple chains is time-consuming and requires deep DeFi expertise.

## Solution

An AI agent monitors on-chain yield data across chains and autonomously moves funds through a Solana vault using cross-chain bridges to capture the best returns.

## MVP features

- Solana vault contract accepting deposits/withdrawals
- AI agent scoring yield opportunities across 2-3 chains via oracle/API data
- Automated cross-chain rebalancing using a bridge (e.g. Wormhole)
- Dashboard showing current allocation, APY, and AI rebalancing history
- Risk profile selector (conservative/balanced/aggressive)

## Chains

Solana, Ethereum, Wormhole

## Tech

Anchor, Rust, Wormhole SDK, Python/LLM agent, Node.js backend, React dashboard, Chainlink or Pyth oracle

## Category

DeFi

## Why now

Cross-chain infrastructure (Wormhole, LayerZero) and AI agent frameworks have matured enough to combine autonomous decision-making with real on-chain execution at hackathon speed.

## Roadmap

- Integrate more chains and yield protocols for broader coverage
- Add backtesting and strategy performance audits for trust
- Launch tokenized shares of the vault for liquidity and composability
