---
description: Platform Mechanics & Fairness
icon: swords
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
metaLinks:
  alternates:
    - https://app.gitbook.com/s/yE16Xb3IemPxJWydtPOj/basics/markdown
---

# How Salatto works

> #### Salatto connects creators who design lotteries with players who participate in them. Every step — from ticket purchase to winner selection to payout — is transparent, automated, and verifiable.

***

#### Game Lifecycle

Every game on Salatto follows a predictable lifecycle:

1. **Creator publishes a game** — defines ticket price, total tickets, prize amount, and duration
2. **Rules are locked** — once live, no parameters can be changed
3. **Players buy tickets** — the prize pool grows in real-time and is visible to everyone
4. **Game completes** — when all tickets are sold or the timer expires (depending on game type)
5. **Winner is selected** — using provably fair on-chain randomness (VRF)
6. **Prizes are distributed automatically** — winners receive funds directly to their wallets
7. **Platform takes a 5% fee** — deducted from the prize pool of successful games only

No manual interference. No hidden outcomes. No delays.

***

#### Randomness & Fairness

Salatto uses **Verifiable Random Function (VRF)** technology to determine all game outcomes.

**What this means:**

* The randomness is generated on-chain and can be independently verified by anyone
* Neither Salatto, nor creators, nor any third party can predict or manipulate results
* Every ticket in a game has an equal, provable chance of winning

**How to verify:** Each completed game links to its on-chain transaction, where the VRF output and winner selection logic can be inspected.

***

#### Flexible RTP

Some games on Salatto **in the future** may have variable RTP (Return to Player) ranges depending on the game type and creator configuration.

**Important rules:**

* RTP ranges are always **disclosed before participation**
* No retroactive changes are possible — once a game is live, its economics are locked
* All game logic is **deterministic** — outcomes follow directly from on-chain randomness and predefined rules

***

#### Failed Games

If a game **does** **not reach** its minimum participation threshold:

* All funds are **returned automatically** to participants
* The creator earns nothing
* Salatto platform also earns nothing
* A small Solana network fee may apply for the refund transaction

The game status changes to **Refunded**, and this is visible in the game history.

***

#### Supported Tokens & Networks

* **Network:** Solana
* **Supported tokens:** SOL and select SPL tokens (varies by game)
* **Wallets:** Phantom, Solflare, Backpack, and other Solana-compatible wallets

***

#### Fee Structure

Salatto's fee model is simple and transparent:

| Fee Type                 | Amount   | Details                                              |
| ------------------------ | -------- | ---------------------------------------------------- |
| Platform fee             | 5%       | Taken from the prize pool of successful games only   |
| Early exit fee           | 15%      | Applied when a player sells a ticket before the draw |
| Gas fees                 | Variable | Standard Solana network fees (typically < $0.0001)   |
| Withdrawal fees          | None     | No platform fee on withdrawals                       |
| Hidden fees              | None     | What you see is what you pay                         |
| VRF fees                 |          | Standard Solana network fees (typically < $0.01)     |
| Refund fees              |          | Standard Solana network fees (typically < $0.0)      |
| Creating lottery         | Variable | Standard Solana network PDAs fees ($1-2,5)           |
| Upgrade button "Medium"  | 2$       | Custom button color + custom text                    |
| Upgrade button "Premium" | 10$      | Gradient colors, custom text, and emojis             |

{% hint style="info" %}
Upgrades — are **optional** and charged once at creation.
{% endhint %}

***

The **early exit fee** exists to protect game liquidity and fairness for remaining participants. If you sell your ticket before the lottery completes, 15% is deducted to compensate for the disruption to the game's economics.

{% hint style="info" %}
**DYOR** — always review game rules, ticket price, prize structure, and odds before participating.
{% endhint %}





* How tickets work
* Number of tickets per lottery
* Disputes & edge cases
* How randomness works (VRF, on-chain, provable randomness)
* Can users verify results?





