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

| Status         | What it means                                                                 |
| -------------- | ----------------------------------------------------------------------------- |
| **Active**     | The game is live and selling tickets. You can still buy or sell tickets.      |
| **Finished**   | Draw is done. Prizes have been distributed to winner wallets. You didn't win. |
| **Wins**       | The game is over and you have **won**. VRF has determined you the winner.     |
| **Refunded**   | The game did not meet minimum requirements. Your money refunded.              |
| **Processing** | Ticket sales have ended. The VRF draw is being executed on-chain.             |

You can view all your tickets grouped by status in the **My Tickets** dashboard.

***

#### Early Exit (Selling Tickets)

You can sell a ticket back before the draw is completed, but a **15% early exit fee** applies.

Why the fee exists:

* Early exits remove liquidity from the game
* They can prevent games from completing, potentially causing refunds for all remaining players
* The fee discourages impulsive exits and protects game integrity

The fee is clearly shown before confirming any sale transaction. If a game is refunded (not completed), you receive a full refund — no exit fee applies.

{% hint style="info" %}
Buy tickets thoughtfully. DYOR before participating.
{% endhint %}

***

#### Refunds Policy

If a lottery fails to meet its requirements (e.g., minimum participants not reached), the game status changes to **Refunded** and funds are returned to all participants automatically. A small Solana network fee may apply.

* **Game refunded** — full refund of ticket price (minus minimal Solana gas fees)
* **Early exit** — ticket price minus 15% fee
* **Game completed, you lost** — no refund (this is normal lottery behavior)
* **Game completed, you won** — prize sent directly to your wallet

Refunds for failed games are processed automatically by the smart contract.

***

#### Evaluating Creators (soon)

Before joining any lottery, check the creator's reputation:

**Creator Rating (CR)** — overall trust score based on completed games, total volume, and consistency. Higher is better.

**Dead Game Rate (DG)** — percentage of the creator's games that ended in refund rather than completion. Lower is better.

A creator with many completed games, high total volume, and DG below 10–15% is generally trustworthy. A creator with 95%+ DG means almost all their games fail — avoid them.

Both metrics are visible on the creator's profile and on every game page. (coming soon)

***

#### &#x20;Rank System&#x20;

Salatto uses a **rank progression system** to reflect a user’s activity on the platform.\
Your rank is based on **how many games you have participated in** (not individual tickets purchased), and is currently displayed in the **My Tickets** section.

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

{% hint style="info" %}
Your rank updates automatically as you participate in more games.&#x20;
{% endhint %}

***

### Current Rank (v1)

**Ranks** —  are displayed on your profile as a visual indicator of experience, and progress tracking. No direct rewards or gameplay advantages are tied to ranks **yet**.

> The rank system will evolve as Salatto grows.

**What's coming next:**

* **XP-based progression**
* **Exclusive games** **and** **lotteries access**
* **Achievements and milestones**
* **Daily/weekly quests**&#x20;
* **Leaderboard visibility**
* **Advanced staking and progression mechanics**

> Ranks are designed to recognize active users, build long-term reputation, and create a clear progression path within the Salatto ecosystem.

{% hint style="info" %}
Over time, progressing to higher ranks will become more challenging, reinforcing long-term engagement and rewarding active participants.
{% endhint %}

***

#### Tips for New Players

* **Start small** — try games with low ticket prices to understand the flow
* **Check creator reputation** — always review CR and DG before buying
* **Read game rules** — every game has its full economics displayed
* **Don't spend more than you can afford to lose** — lotteries are entertainment, not investment
* **Use flexible lotteries** — they complete more reliably than standard ones
* **Share and promote** — found a great game? Sharing helps creators and grows the community

***
