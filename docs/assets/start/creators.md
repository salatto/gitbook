---
description: Creator Guide
icon: user-group-crown
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
    - https://app.gitbook.com/s/yE16Xb3IemPxJWydtPOj/basics/integrations
---

# For Creators (Operators)

> **Creators** are independent users who design, launch, and promote lotteries and games on Salatto. They define the rules and economics — the platform handles execution, fairness, and payouts.

{% hint style="info" %}
**Creators** are not employees or partners of Salatto. They are **independent game publishers**.
{% endhint %}

***

#### Who Can Become a Creator

Anyone who:

* Connects a Solana wallet
* Passes basic platform requirements
* Agrees to platform rules and transparency standards

> There is no minimum audience size. Whether you have 100 followers or 1,000,000 — you can create a game.

***

### Creator Guide

Creating a game on Salatto is designed to be simple, transparent, and fully creator-controlled. You define the idea and economics — the platform handles execution, fairness, and payouts.

**Step 1 — Connect Your Wallet**

Connect your Solana wallet to access creator features.

* Click **Log in** in the top-right corner
* Approve the wallet connection

Your wallet acts as your creator identity and payout destination.

**Step 2 — Open the Game Creator**

Navigate to the game creation interface.

* Click **Create Game**
* Choose the type of game you want to launch

This is where your lottery or instant game is configured.

**Step 3 — Define Game Rules**

Configure the core parameters of your game:

* **Prize type and amount** — what winners receive
* **Ticket price** — cost per entry (shown in SOL with USD equivalent)
* **Total number of tickets** — how many participants the game supports
* **Game duration** — time limit or sell-out condition
* **Prize distribution** — how winnings are split across winners (one or more winners)
* **Creator margin** — your earnings percentage from the game
* **Flexible option** — whether the lottery can complete before 100% fill (optional) (soon)
* **Jackpot participation** — whether to opt into the monthly Jackpot Pool (optional, +5% commission)

The prize pool must be at least **5% of total game revenue** — ensuring meaningful prizes for players.

{% hint style="info" %}
All rules are locked before launch and cannot be changed once the game is live.
{% endhint %}

**Step 4 — Customize Your Game Card Button (Optional)**

Personalize how your game appears in the marketplace:

* **Default** — Free standard game card
* **Tier 1** — Custom color + name styling (\~$2 in SOL)
* **Tier 2** — Gradient + name + emoji styling (\~$10 in SOL)

Better-looking game cards attract more attention and ticket purchases.

**Step 5 — Publish and Promote**

**Once published**, your game becomes immediately available to players. Share the link to attract participants — every lottery is a standalone shareable product. The platform displays "Share your lottery to earn more" to encourage viral distribution.

***

#### Promote (Upgrade) System

Creators can boost their lottery's visibility through the Promote system on the platform:

* **Scrolling text** — your lottery appears in the scrolling banner with custom text and display duration
* **Ad blocks** — banner placement in high-visibility areas of the platform
* **Sticker frames** — decorative frames around your game card

Each promotion type has configurable duration and pricing. Promotion is purchased in SOL during or after game creation.

**Burning mechanics (soon):** Instead of paying upfront for promotion, eligible creators (those meeting minimum CR and rank requirements) will be able to "burn" part of their creator commission to boost their lottery for free. The platform takes 50% of creator fees - burned fees as an upgrade cost. New creators are not eligible — this feature requires proven track record.

***

#### What Creators Control

Creators define:

* Game type and format
* Ticket price and total supply
* Prize pool distribution
* Creator margin (earnings percentage)
* Flexible completion option
* Jackpot Pool participation
* Game card appearance

Creator does NOT control:

* Randomness or winner selection
* Payout execution
* Game outcome in any way

{% hint style="info" %}
This separation ensures that every game is fair regardless of who created it.
{% endhint %}

***

#### Game Statuses

| Status         | What it means                                                                                                        |
| -------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Active**     | Your game is live and selling tickets. Users can still buy or sell tickets.                                          |
| **Completed**  | Draw is done. Prizes have been distributed to winner wallets.                                                        |
| **Cencelled**  | The game did not meet minimum requirements. All ticket funds are refunded. You don't earn anything. CR is downgrade. |
| **Processing** | Ticket sales have ended. The VRF draw is being executed on-chain.                                                    |

***

#### How Creators Earn

Creators earn their configured margin from each successfully completed game. The exact percentage is set during game creation and is visible to all participants before they buy tickets.

Creators **do not earn** if:

* The game fails to reach minimum participation (refunded)
* Platform rules are violated

{% hint style="info" %}
The creator is solely responsible for promoting their lottery and undertakes to promote it.
{% endhint %}

**Flexible lotteries:** If a creator enables the flexible option, the lottery can complete even without 100% ticket sales. In this case, the creator's commission is reduced proportionally — they earn less, but the game still completes rather than being refunded. This is often preferable to a full refund where the creator earns nothing, which also leads to a lower rating.

#### Creators are users who:

* create lotteries or games
* define prize structures
* attract audiences
* earn from successful games up to 90% of successful game.

{% hint style="info" %}
Each creator independently determines their own game, but no less than 5% for the prize pool.
{% endhint %}

***

#### Creator Reputation System

Every creator has a public profile with two key metrics that help players make informed decisions:

**Creator Rating (CR)**

An overall trust score based on:

* Number of successfully completed games
* Total revenue volume processed
* Game completion rate
* Player satisfaction

Higher CR means more trust. Creators with high CR appear higher in search results and discovery rankings, which directly translates to more players and more revenue.

**Death Game Rate (DG)**&#x20;

> Count starts with 10th game. (soon)

The percentage of a creator's games that ended in a refund rather than a successful draw. DG matters because:

* Refunded games waste players' time (games can run for weeks before failing and refunded)
* Players selling tickets early from likely-to-fail games lose 15% to the exit fee
* A creator with 95–99% DG is essentially creating games that never complete

**The relationship:** More completed games + higher total volume + lower DG = higher CR = better visibility = more money.

{% hint style="info" %}
A high CR and low DG indicate a reliable creator. Players are encouraged to check these metrics before participating.
{% endhint %}

***

#### Creator Verification

Creators can apply for a **Verified** badge that appears on their profile and game cards:

* Apply via [**verified@salat.to**](mailto:verified@salat.to) with your social media profiles
* The team evaluates your reach, authenticity, and content quality
* An automated application form is also planned

Verified status builds trust with players and can improve conversion rates.

***

#### Creator Rank & Progression (Planned)

In future versions, creators will have a rank-based progression system:

* New creators start with lower maximum commission percentages
* As rank increases through completed games, higher commission tiers unlock
* This prevents brand-new creators from setting exploitative margins
* Proven creators with high CR and low DG get the most earning potential

***

#### Anti-Fraud Rules

Salatto enforces strict rules to protect players:

* Creators cannot manipulate randomness or outcomes
* Game parameters are immutable once published
* Suspicious patterns (self-play, coordinated abuse) are detected and flagged
* Violations result in penalties up to permanent platform ban
* CR and DG metrics provide transparent accountability

***

#### Creator FAQ

**Can I edit a game after publishing?** No. All game rules are locked at launch to ensure fairness and trust.

**What happens if my game doesn't sell out?** If minimum participation isn't reached, the game is refunded. All player funds are returned, and you earn nothing, and your **CR is dropping**.&#x20;

**How much can I earn?** Your earnings depend on the creator margin you set (up to 90%) and the number of tickets sold. The platform takes a 5% fee from successful games. Your margin is fully transparent to your players, and your efforts to promote the lottery.

**Do I need a large audience?** No. Games are discoverable on the Salatto marketplace through search, trending, and category listings. However, creators who actively promote their games in social media and share their games consistently perform better.

**How do I improve my Creator Rating?** Complete more games successfully, avoid refunds (low DG), grow your total volume, and maintain consistent participation. The more reliable you are, the higher you rank in discovery.

**Can I create repeated lotteries?** A feature for automatic lottery repetition (creating a new game when the previous one completes) is planned for a future release.

**Can I add social links to my lottery?** Yes, you can add social media links — Twitter/X, Telegram, Discord, Site and other channels — directly on the lottery page. But keep in mind that you can only add them **once** when creating the lottery.

***
