---
description: Frequently Asked Questions
icon: comments-question-check
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

# FAQ

#### General

**What is Salatto?** Salatto is a decentralized lottery and gaming platform on Solana. Anyone can create or participate in provably fair lotteries and games with transparent rules and instant payouts. Salatto is a community-run lotto marketplace — a new category called LottoFi.

**Is Salatto a gambling platform?** Salatto provides entertainment-based games and lotteries built on blockchain technology. Availability and participation may depend on local regulations in your jurisdiction.&#x20;

**Do I need crypto knowledge to use Salatto?** No. Salatto is designed to be accessible to both crypto-native and non-crypto users. You need only a Solana wallet to participate, but no advanced blockchain knowledge is required.

**Who can use Salatto?** Salatto is available to users who meet the minimum age requirement (18+) and are legally allowed to participate according to their local laws. Some jurisdictions may be restricted — a notice is displayed in 'Terms of use' if restrictions apply to your region.

**Can I play anonymously?** Yes. Salatto uses wallet-based authentication. No personal information, email, or KYC is required to participate. Your identity is your wallet address.

**Is Salatto available in my country?** Salatto may display a restriction notice if your region has specific legal limitations on lottery or gaming participation. Users are responsible for ensuring compliance with their local laws.

{% hint style="info" %}
Jurisdiction Notice By accessing or using Salatto, you confirm that you are not a resident of, located in, or accessing the platform from any restricted jurisdiction where participation in lotteries or similar activities may be prohibited by law. Restricted jurisdictions include, but are not limited to: United States, United Kingdom, Germany, France, Netherlands, Cyprus, Australia, and any other jurisdiction where such activities are restricted or illegal. It is the user’s sole responsibility to ensure that accessing and using Salatto is lawful in their country of residence.
{% endhint %}

***

#### Tickets & Participation

**How do tickets work?** Each game has a fixed number of tickets at a set price. Buying a ticket enters you into the draw. When the game completes (either all tickets are sold or the timer/conditions are met), winners are selected using on-chain VRF randomness.

**Can I buy more than one ticket?** Yes. You can purchase multiple tickets in a single lottery to increase your chances. However, the platform limits total purchases so that you cannot buy tickets whose total cost exceeds the prize pool value — because spending more than you can possibly win makes no economic sense. This protection exists for your benefit.

**Is there a maximum number of tickets I can buy?** The limit is based on the prize pool, not a fixed number. You cannot purchase tickets whose total cost exceeds the potential prize pool. For example, if the prize pool is 100 SOL, you cannot buy tickets worth more than 100 SOL total.

**What types of games are available?** Currently, Salatto supports classic lotteries, flexible lotteries. Jackpot monthly pools, and instant games are planned for future releases.

**What happens if a lottery doesn't sell out?** If a game fails to meet its minimum participation requirements, it is automatically **refunded**. All funds are returned to participants. The creator earns nothing.

**Can I get a refund after buying a ticket?** You can sell your ticket back before the draw, but a **15% early exit fee** applies. This fee compensates for the disruption to the game's liquidity and economics. If the game is refunded due to insufficient participation, you receive a full refund (minus minimal Solana network fees).

**What is the game lifecycle?** Creator publishes → tickets go on sale → game fills or timer expires → VRF selects winner → prizes distributed automatically.

**What happens if a lottery doesn't sell out?** This depends on the game configuration:

* **Standard lottery:** If minimum participation is not reached by the deadline, the game is refunded and all funds are returned.
* **Flexible lottery:** If the creator enabled the flexible option, the lottery can complete even without 100% ticket sales. The creator's commission is reduced proportionally, while the prize pool and platform fee remain intact.

**What is a flexible lottery?** A flexible lottery is a game where the creator agreed (before launch) that the lottery can end before all tickets are sold. The creator sacrifices part of their commission to ensure the game completes. This is set during game creation and cannot be changed after launch. Flexible lotteries reduce the chance of refunds and improve player experience.

***

#### Fairness & Trust

**Is this rigged? Can anyone manipulate the outcome?** No. All outcomes are determined by on-chain Verifiable Random Function (VRF) technology. The process works in two phases:

1. **Commit phase** — when the game is ready for a draw, the contract requests a random number from the VRF oracle and stores the request ID
2. **Reveal phase** — the VRF oracle returns a verifiable random number, which the contract uses to deterministically select the winner

{% hint style="info" %}
Neither Salatto, creators, nor any third party can predict or influence results. Every draw is publicly verifiable on the Solana blockchain.
{% endhint %}

**How does VRF work in simple terms?** VRF (Verifiable Random Function) is a cryptographic method that produces a random number along with a mathematical proof that the number was generated fairly. Think of it like a sealed envelope with a random number inside — anyone can verify the envelope was sealed correctly, but no one could have known the number in advance. On Salatto, VRF generates the randomness for every draw, and the proof is stored on-chain for anyone to inspect.

**Can creators scam users?** No. Creators define game parameters before launch, but all rules are locked and immutable once the game goes live. Creators cannot change odds, manipulate randomness, or interfere with payouts. Every creator has public reputation metrics — Creator Rating (CR) and Death Game Rate (DG) — that help players assess reliability before participating.

**What is Creator Rating (CR)? (soon)** Creator Rating is an overall trust score based on game history — how many games successfully completed, total volume processed, and completion rate. Higher CR means a more reliable creator. Creators with high CR appear higher in the platform's search and discovery rankings.

**What is Death Game Rate (DG)? (soon)** Death Game Rate shows the percentage of a creator's games that ended in a refund rather than a successful draw. A high DG (e.g., 95–99% of games refunded) is a strong warning signal. Players should check both CR and DG before participating — a creator with many completed games, high total volume, and low DG is the most trustworthy.

{% hint style="info" %}
Death Game rate starts with 10th game.
{% endhint %}

**Can Salatto block my funds or withdrawals?** No. Salatto is non-custodial. Funds in active games are held in on-chain contracts, and payouts are automated. Salatto cannot freeze, block, or redirect your winnings.

**What happens if Salatto shuts down?** Funds in active game contracts remain on-chain. Completed games have already distributed payouts. Active games would follow their programmed logic (completion or refund).

***

#### Economics & Fees

**Why did I lose?** Lotteries are probability-based. Each ticket has a known chance of winning, clearly disclosed before purchase. Not every ticket wins — that's the nature of a lottery. Unlike casinos where you play against the house, in Salatto you play against other participants in a transparent pool.

**Can I lose more than I spend?** No. Your maximum loss is the price of the ticket(s) you purchased. There is no leverage, margin, or additional risk.

**Can RTP change after I buy a ticket?** No. RTP and all game economics are locked at the time of game publication. No retroactive changes are possible.

**What is the platform fee?** Salatto takes a 5% fee from the prize pool of successfully completed games. There are **no fees** on failed/refunded games, and no withdrawal fees.

| Fee Type        | Amount       | Details                                   |
| --------------- | ------------ | ----------------------------------------- |
| Platform fee    | 5%           | From prize pool of successful games only  |
| Early exit fee  | 15%          | When selling a ticket before the draw     |
| Gas fees        | Variable     | Standard Solana fees, typically < $0.0001 |
| Withdrawal fees | None         | No platform fee on withdrawals            |
| Game creation   | Free or paid | Depends on game card customization tier   |
| Hidden fees     | None         | What you see is what you pay              |

**Are there paid features for game creation?** Yes. Creators can optionally customize their game card appearance:

* **Default** — Free (standard game button)
* **Tier 1** — Custom color + name styling (\~$2 in SOL)
* **Tier 2** — Gradient + name + emoji styling (\~$10 in SOL)

These are optional cosmetic upgrades that help games stand out in the marketplace.

**What is the Promote system?** Creators can boost the visibility of their lotteries through the Promote (Upgrade) system. Options include **scrolling text banners, ad blocks, and sticker frames.** Promotion is purchased in SOL and gives the lottery higher visibility on the platform.

**How does the prize pool work?** The prize pool is funded by ticket purchases. Revenue from each game is split between:

* **Prize pool** — the amount distributed to winners (set during game creation — by creator)
* **Creator margin** — the creator's earnings (set during game creation)
* **Platform fee** — 5% to Salatto infrastructure

The creator must set a prize pool of at least 5% of the total game revenue. All splits are visible before participation.



***

#### Games & Features

**What types of games are available now?** Currently, Salatto supports **classic lotteries** — buy tickets, wait for the draw, win based on VRF randomness.

**What types of games are coming soon?**

* **Jackpot Pool** — monthly shared prize pool across participating lotteries
* **No-Loss Lotteries** — participate with guaranteed partial cashback (25%, 50%, or 75%)
* **Scratch Cards (Heart Stoppers)** — instant-win VRF-based scratch mechanics
* **Sweepstakes** — giveaway-style draws verified by VRF
* **Mini-Games** — fast VRF-powered games (Flip, Pump/Rocket, Plinko, Snake, CoinFlip, etc.)
* **Flip Tournaments** — bracket-style elimination coin flip tournaments (16 to 1024 players)
* **Non-monetary prize lotteries** — physical goods, NFTs, courses, experiences

**What is the Jackpot Pool? (soon)** Creators can opt their lotteries into the monthly Jackpot program (+5% commission). All tickets from participating lotteries automatically enter the monthly Jackpot draw. The more games you play that month, the higher your chances. Jackpot lotteries are marked with a badge and get priority placement on the homepage.&#x20;

{% hint style="info" %}
All games that ended within one calendar month participate in the jackpot pool (if they chose to participate).
{% endhint %}

**What are No-Loss Lotteries?** No-Loss lotteries return a percentage of the ticket price to all losing participants:

* **Medium risk** — 25% cashback on losing tickets
* **Low risk** — 50% cashback
* **Very low risk** — 75% cashback

Higher cashback means a smaller prize pool, but lower risk for players.

**Can lotteries offer non-monetary prizes?** Yes (coming soon). Creators will be able to offer physical goods, NFTs, online courses, mentorship sessions, exclusive content, collectibles, or meet-and-greet experiences. The VRF mechanism works the same regardless of prize type.

**Can I comment on a lottery?** Yes. Each lottery page has a comments section where players can discuss the game or ask questions.

**How does sharing work?** Every lottery has a Share button that generates a shareable link with a preview image. For creators, the platform encourages sharing with the message "Share your lottery to earn more." Each lottery is a standalone shareable product designed for viral distribution.

**What is the Trending section?** The homepage features a Trending section highlighting popular lotteries based on participation rate, speed of ticket sales, and community engagement.

***

#### Account & Rank

**How does the rank system work?** Salatto uses a rank progression system based on the number of **lotteries** you've participated in (not individual tickets). Ranks are displayed in the My Tickets section.







#### Technical

**What blockchain does Salatto use?** Salatto runs on Solana — chosen for its low transaction costs, fast confirmation times, and native VRF support.

**Which wallets are supported?** Phantom, Solflare, Backpack, and other Solana-compatible wallets.

**What tokens can I use?** SOL and select SPL tokens, depending on the game. Supported tokens are shown on each game page.



