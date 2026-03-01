# VPNL — Verifiable PnL

> *The trust infrastructure for competitive intent markets.*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Built for ERC-7683](https://img.shields.io/badge/Built%20for-ERC--7683-3C3C3D.svg)]()
[![Deployed: Arbitrum Sepolia](https://img.shields.io/badge/Deployed-Arbitrum%20Sepolia-orange.svg)](https://sepolia.arbiscan.io/address/0xD3Acf580A28977D24da7d20364A2F557606d439A)
[![Powered by DIA Lumina](https://img.shields.io/badge/Powered%20by-DIA%20Lumina-orange.svg)]()

-----

## The Problem

DeFi spent a decade removing human judgment from markets. AMMs replaced market makers. Orderbooks replaced negotiation. Algorithms replaced discretion.

It worked — for simple, single-chain, liquid swaps.

Then intent markets arrived.

Intent protocols reintroduce what algorithms can’t provide: competitive human optimization. Solvers hold inventory across chains in anticipation of flow, route orders across venues, and compete to deliver the best outcome for users. The result is better prices, cross-chain execution, and capital efficiency that no orderbook or AMM can match.

But competitive discretionary markets have a structural requirement that mechanical markets don’t: **trust.**

When a solver commits to fill your cross-chain order, you’re relying on their infrastructure, their inventory, their incentive to perform. The protocol needs to know how much collateral to require. The user needs to know their order will be filled. New solvers need a way to prove themselves without posting 100% collateral on every trade.

Without reputation infrastructure, intent markets stay small, overcollateralized, and gated behind centralized allowlists — defeating the purpose entirely.

-----

## What VPNL Is

VPNL is the verifiable PnL layer for ERC-7683 intent markets.

It derives solver performance scores directly from on-chain settlement events — no self-reporting, no trusted intermediaries. Scores are committed to an on-chain registry and delivered cross-chain via DIA Lumina, making them queryable by any protocol on any chain.

The ERC-7683 standard — co-authored by Uniswap Labs and Across Protocol — explicitly identified this gap in its Security Considerations:

> *“We hope that this standard can eventually support an ERC dedicated to standardizing a safe, trustless, crosschain verification system.”*

VPNL is that system.

-----

## Repositories

|Repo                                           |Description                                                                 |
|-----------------------------------------------|----------------------------------------------------------------------------|
|[**vpnl**](https://github.com/vpnlnetwork/vpnl)|Core registry contracts, scoring model, deployment scripts, and testnet demo|

*Indexer, SDK, and DIA integration repos coming in Phase 2.*

-----

## Documentation

- [Protocol README](https://github.com/vpnlnetwork/vpnl#readme) — architecture, scoring model, integration guide
- [Scoring Model Spec](https://github.com/vpnlnetwork/vpnl/blob/main/docs/) — metric definitions, weighting, epoch design
- [DIA Lumina Integration](https://github.com/vpnlnetwork/vpnl/blob/main/docs/dia-lumina-integration.md) — cross-chain delivery architecture
- [Security Policy](https://github.com/vpnlnetwork/vpnl/blob/main/SECURITY.md)
- [Contributing](https://github.com/vpnlnetwork/vpnl/blob/main/CONTRIBUTING.md)

-----

## Deployment

|Network         |Contract    |Address                                                                                                                       |
|----------------|------------|------------------------------------------------------------------------------------------------------------------------------|
|Arbitrum Sepolia|VPNLRegistry|[`0xD3Acf580A28977D24da7d20364A2F557606d439A`](https://sepolia.arbiscan.io/address/0xD3Acf580A28977D24da7d20364A2F557606d439A)|
|Arbitrum One    |VPNLRegistry|Post-audit                                                                                                                    |

-----

## Community

- 🌐 [vpnl.io](https://vpnl.io)
- 🐦 [@vpnlnetwork](https://twitter.com/vpnlnetwork)
- 💬 [t.me/vpnlnetwork](https://t.me/vpnlnetwork)
- 🔗 [DIA Lumina](https://www.diadata.org/lumina/)
- 📄 [ERC-7683](https://eips.ethereum.org/EIPS/eip-7683)

-----

*VPNL: Open standards for verifiable solver performance.*
*Building the trust infrastructure that competitive intent markets require.*