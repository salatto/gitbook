---
description: Player Guide
icon: gamepad-modern
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
    - https://app.gitbook.com/s/yE16Xb3IemPxJWydtPOj/basics/interactive-blocks
---

# For Players (Users)

> Players are users who browse, participate in, and win prizes from lotteries and games on Salatto. No blockchain expertise is required — the platform is designed to be accessible to everyone.

***

#### How to Play

1. **Connect your wallet** — click **Log in** and approve the wallet connection
2. **Browse available games** — explore live lotteries, upcoming games, and instant games
3. **Review Game Details** — before buying, check:
   * Ticket price
   * Prize pool amount
   * Total number of tickets
   * Lottery progress (tickets sold / remaining)
   * Creator info and reputation (CR and DG metrics)
4. **Buy ticket(s)** — confirm the transaction in your wallet.
5. **Wait for the draw** — or get an instant result, depending on the game type
6. **Receive winnings automatically** — prizes are sent directly to your wallet instantly and automatically. No claims process, no waiting period, no paperwork.
7. **Track Your History** — View all your tickets, game results, and statistics in the **My Tickets** section.

> The draw triggers when all tickets are sold, the deadline is reached, or (for flexible lotteries) minimum conditions are met. The draw is automatic and uses on-chain VRF randomness.

{% hint style="info" %}
You can buy multiple tickets in a single lottery to increase your chances.
{% endhint %}

***

#### Buying Multiple Tickets

You can purchase more than one ticket per lottery. There is no restriction on the number of tickets — buying more tickets increases your probability of winning.

However, the platform enforces a smart limit: **you cannot purchase tickets whose total cost exceeds the prize pool value**. This exists to protect you. Spending more on tickets than you could possibly win makes no economic sense, and Salatto prevents this by design.

***

#### Types of Games

**Classic Lotteries (Live)** Standard lottery format — buy tickets, for all tickets to sell, winner is selected by VRF. Simple, transparent, and proven. The most common game type on Salatto.\
The game must sell 100% of its tickets — otherwise a refunds will be issued.

**Flexible Lotteries (Soon)** Same as classic, but the creator has opted to allow the lottery to complete before 100% of tickets are sold. If the game reaches its minimum threshold (time deadline + minimum participation), it completes and the creator receives a reduced fees. This means more games finish successfully instead of being refunded, and CR doesn't drop.

**Jackpot Pool (Soon)** — a monthly shared prize pool funded by participating lotteries. Creators opt in (+5% JP fees cost), and all tickets from those lotteries also automatically enter the monthly Jackpot draw. Jackpot-participating games are marked with a badge and receive priority placement. The more games you play each month, the higher your chances of winning the monthly Jackpot.

**Creator-Exclusive Games** **(Coming Soon)**

**No-Loss Lotteries (Coming Soon)**

**Scratch Cards / Heart Stoppers (Coming Soon)**

**Mini-Games (Coming Soon)**

**Flip Tournaments (Coming Soon)**

***

#### Understanding Odds

Every game on Salatto displays its odds before participation:

* **Win probability** = your tickets / total tickets in the game
* **Your percentage chance** of winning

For example, in a game with 100 tickets at 1 SOL prize pool:

If you buy 1 ticket: win probability = 1/100 = 1%,

If you buy 5 tickets: win probability = 5/100 = 5%.

> All of this is visible on the game page. There are no hidden odds or house edges beyond the disclosed platform fee (5%) and creator determined margin.

***

#### Game Statuses

Your tickets and games progress through these statuses:

| Status         | What it means                                                              |
| -------------- | -------------------------------------------------------------------------- |
| **Active**     | The game is live and selling tickets. You can still buy or sell tickets.   |
| **Completed**  | Draw is done. Prizes have been distributed to winner wallets.              |
| **Refunded**   | The game did not meet minimum requirements. All ticket funds are refunded. |
| **Processing** | Ticket sales have ended. The VRF draw is being executed on-chain.          |

You can view all your tickets grouped by status in the **My Tickets** dashboard.

***

#### Early Exit

Changed your mind after buying a ticket? You can sell it back before the draw completes.

**Early exit fee: 15%**

This fee compensates for the disruption to the game's liquidity and economics. It protects both the creator and other participants.

Buy tickets thoughtfully. DYOR before participating.

***

#### Refunds

If a lottery fails to meet its requirements (e.g., minimum participants not reached), the game status changes to **Refunded** and funds are returned to all participants automatically. A small Solana network fee may apply.

***

#### Rank Progression&#x20;

Salatto uses a **rank progression system** to reflect a user’s activity on the platform.\
Your rank is based on **how many games you have participated in** and is currently displayed in the **My Tickets** section.

***

### Rank Levels

| Rank                                                        | Games Played |
| ----------------------------------------------------------- | ------------ |
| **Beginner**                                                | **0–10**     |
| <mark style="color:$warning;">**Bronze • Top 50%**</mark>   | **11–50**    |
| <mark style="color:$info;">**Silver • Top 40%**</mark>      | **51–150**   |
| <mark style="color:yellow;">**Gold • Top 25%**</mark>       | **151–300**  |
| <mark style="color:$success;">**Platinum • Top 15%**</mark> | **301–500**  |
| <mark style="color:blue;">**Diamond • Top 5%**</mark>       | **501–1000** |
| <mark style="color:purple;">**Legend • Top 1%**</mark>      | **1001+**    |

Your rank updates automatically as you participate in more games.

***

### Current State (v1)

* Ranks are **non-financial**
* No direct rewards or advantages yet
* Used mainly for **visual status and progress tracking**

***

### Future Evolution

**Ranks** are informational and visual — used for status and progress tracking. No direct rewards or gameplay advantages are tied to ranks **yet**.

> The rank system will evolve as Salatto grows.

**What's coming next:**

* **Achievements and milestones**
* **Rank-based platform perks** and access to **exclusive games** and **lotteries**
* Enhanced **benefits** for high-rank users
* Advanced **staking** and progression mechanics

Ranks are designed to recognize active users, build long-term reputation, and create a clear progression path within the Salatto ecosystem.

Over time, progressing to higher ranks will become more challenging, reinforcing long-term engagement and rewarding active participants.

***

