# SolSwap AI

AI-powered swap aggregator on Solana — combining smart slippage protection, an agentic buy/sell executor, and automated token risk control.

## Overview

SolSwap AI helps traders swap tokens on Solana more safely and efficiently by aggregating quotes across multiple DEXs, protecting against bad slippage, and screening tokens for common scam patterns (rugpulls, honeypots) before execution. An AI agent layer handles trade execution based on configurable rules, moving beyond a simple swap UI toward agentic, autonomous trading logic.

## Core Features

### 1. Smart Slippage Protection
- Dynamic slippage calculation based on real-time pool liquidity
- Auto-reject or auto-adjust swaps when slippage exceeds safe thresholds

### 2. AI Agent for Buy/Sell Execution
- Rule-based (v1) → autonomous (later) trade execution
- Executes swaps based on price conditions, portfolio rules, or natural-language instructions

### 3. Token Risk Control
- Checks mint authority and freeze authority status
- Checks liquidity lock status
- Checks holder concentration
- Flags high-risk tokens before a swap is executed

## Roadmap

- [ ] **Milestone 1 (MVP):** Core swap engine integrating 2 DEXs (Raydium + Orca) — quote fetching, swap execution, basic slippage protection
- [ ] **Milestone 1 (MVP):** Basic risk check (mint authority / freeze authority) before swap execution
- [ ] **Milestone 1 (MVP):** Rule-based AI agent v1 for triggering buy/sell on price conditions
- [ ] **Milestone 2:** Expand DEX integrations (Meteora, Jupiter, etc.)
- [ ] **Milestone 2:** Full risk scoring (liquidity lock, holder concentration)
- [ ] **Milestone 3:** Autonomous AI agent with natural-language trading instructions

## Why "Agentic"

Unlike a standard swap UI, SolSwap AI's agent layer makes trading decisions with bounded autonomy — reading real-time on-chain data, applying risk rules, and executing trades without manual clicks for every action.

## Tech Stack

- Solana (web3.js / Anchor — TBD)
- [DEX SDKs — Raydium, Orca]
- [Backend/agent framework — TBD]

## Author

Built by [zkgm-55](https://github.com/zkgm-55)
Related work: [solana-rpc-benchmarker](https://github.com/zkgm-55/solana-rpc-benchmarker), [position-manager-skill](https://github.com/zkgm-55/position-manager-skill)

## Status

🚧 Early development — MVP in progress as part of Superteam Agentic Engineering Grant application.
