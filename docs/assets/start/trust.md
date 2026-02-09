---
description: LottoFi
icon: cubes
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Ecosystem & Protocol

**Salatto is a LottoFi platform** — the infrastructure layer connecting lotteries with decentralized finance.

***

* Core: **LottoFi (new vertical)**
* By nature: **DeFi-native**
* By experience: **Game-like**
* By infra: **runs on L2 (on Solana)**

***

#### What is LottoFi

LottoFi is a new vertical that bridges traditional lottery mechanics with DeFi primitives. In a LottoFi model:

* Lotteries are no longer "one-way bets" — tickets gain secondary market potential
* Fairness is guaranteed by on-chain VRF, not by operator reputation
* Liquidity mechanisms (ticket buyback) replace dead-end ticket purchases
* Settlement, payouts, and verification happen on-chain

> Salatto is the **first** platform to bring this model to market.

***

#### Architecture Overview

Salatto's protocol consists of several core components:

**Game Contracts** — each lottery or game is deployed as an independent PDA on-chain program with immutable rules, prize logic, and payout distribution.

**VRF Oracle** — a Verifiable Random Function oracle provides tamper-proof randomness for every draw. The VRF output is recorded on-chain and can be independently verified.

**Payout Engine** — automated distribution of winnings to player wallets upon game completion. No manual approvals or delays.

**Creator Module** — a no-code interface for creating and configuring games. Creators define parameters. The protocol handles execution.

***

#### For Creators / Lottery Operators

Salatto provides creators with:

* **No-code lottery creation** — launch a game in minutes
* **Instant liquidity** — prize pools fill in real-time as tickets are sold
* **DeFi tools** — games, pools, staking, and treasury mechanics (expanding)
* **Global distribution** — anyone with a Solana wallet can participate

***

#### For Players

Players benefit from:

* **Live prize pools** — view participants and funds in real-time
* **Verifiable draws** — provably fair outcomes using on-chain VRF
* **Instant payouts** — winnings go directly to your wallet
* **Full transparency** — every game's rules, odds, and economics are visible before participation

***

#### Wallets, Payments & Withdrawals

| Detail                         | Info                                                             |
| ------------------------------ | ---------------------------------------------------------------- |
| Supported wallets              | Phantom, Solflare, Backpack, and other Solana-compatible wallets |
| Supported network              | Solana                                                           |
| Supported tokens               | SOL, select SPL tokens (varies by game)                          |
| Minimum withdrawal             | None                                                             |
| Minimum tickets (participants) | None                                                             |
| Maximum tickets (participants) | None                                                             |
| Maximum prize pool             | None                                                             |
| Processing time                | Instant (standard Solana transaction time)                       |
| Failed transactions            | Retry through your wallet; funds remain safe in the contract     |

***

#### Security & Audits

* Smart contract audits are planned and will be published upon completion
* Bug bounty program — coming soon
* For vulnerability reports, contact the team via Support

***

#### What's Next

Salatto's protocol is designed to expand. Future developments include:

* SLTO token with deflationary mechanics tied to lottery activity and staking
* Monthly Jackpot based on all games played and millions of participants
* Staking and yield mechanics integrated with game participation
* API and embeddable widgets for third-party sites and streamers
* Multi-chain expansion (TON, Aptos, Sui, Polygon)
* Telegram WebApp integration
* and much more..

See the **Roadmap** for the full development plan.



