---
description: Provably Fair
icon: shield-check
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

# Security & Trust

Trust is the foundation of any lottery platform. Salatto is built so that trust is not required — it is **verifiable**.

***

#### Provably Fair Draws

{% hint style="info" %}
Every draw on Salatto is on-chain and verifiable. This ensures that no one — including platform developers, lottery creators, or any third party — can predict or manipulate the result of a draw.
{% endhint %}

**VRF Technology:** Salatto uses a **Verifiable Random Function (VRF)** to generate randomness for all game outcomes. VRF is a cryptographic primitive that produces a random output along with a mathematical proof that the output was generated correctly.

**The Two-Phase Process:**

**Phase 1 — Commit** When a lottery is ready for a draw (all tickets sold or deadline reached):

1. The smart contract accepts the final game state
2. The contract calls the VRF oracle and requests a random number
3. A `requestId` is stored on-chain, locking the request

At this point, no one knows what the random number will be — not the platform, not the creator, not the oracle itself.

**Phase 2 — Reveal** The VRF oracle generates the random number and returns it to the contract:

1. The oracle returns a `randomWord` — a cryptographically random value
2. The contract converts this value into a usable range (e.g., `randomWord % totalTickets`)
3. The resulting number maps directly to a winning ticket
4. The winner is selected deterministically — the same random number always produces the same winner
5. Prizes are distributed automatically to the winner's wallet

**Why this is trustworthy:**

* The random number is generated **after** all tickets are purchased — no one can game the system
* The VRF proof is stored on-chain and can be independently verified by anyone
* The mapping from random number to winner is deterministic and transparent
* Even if you could see the VRF oracle's internal state, you couldn't predict the output for a specific request

***

#### How to Verify a Draw Result

You don't have to trust Salatto — you can verify every draw yourself.

**Step-by-step verification:**

1. **Open the completed game** on Salatto
2. **Click the transaction link** — this opens the Solana blockchain explorer (e.g., Solscan or Solana Explorer)
3. **Find the VRF request transaction** — this shows when the randomness was requested and the `requestId`
4. **Find the VRF fulfillment transaction** — this shows the random number returned by the oracle
5. **Check the winner selection** — the random number modulo the total number of tickets gives you the winning ticket index
6. **Verify the payout** — confirm that the prize was sent to the correct wallet address

The entire chain of events — from request to random number to winner to payout — is visible on the public blockchain.

A dedicated **Provably Fair** verification page is planned for the platform footer, making this process even more accessible for non-technical users.

{% hint style="info" %}
The math is public. The results are deterministic. Anyone can verify.
{% endhint %}

***

#### Automated, Immutable Execution

* **Automated payouts** — winners receive funds directly to their wallets without manual intervention
* **Immutable game logic** — once a game is published, its rules cannot be changed
* **No manual overrides** — Salatto cannot alter outcomes, block payouts, or modify game parameters after launch
* **Transparent rules** — every game's mechanics, odds, and prize structure are visible before participation
* **Real-time visibility** — prize pools, ticket sales, and participant counts update live via WebSocket connections

***

#### Non-Custodial by Design

Salatto does not hold user funds outside of active game participation.

* Your wallet remains under your control at all times
* Funds are locked in game contracts only during active participation
* Winnings are distributed directly to your wallet
* Refunds are processed automatically if a game fails

**Salatto will never ask for:**

* Your private keys or seed phrase
* Direct token transfers outside the platform interface
* Access to your wallet beyond standard transaction approvals

{% hint style="info" %}
If anyone asks for these — it is a scam.
{% endhint %}

***

#### Creator Reputation System

Not all creators are equal. Salatto provides tools to help players assess creator reliability:

*   **Creator Rating (CR) Soon!**&#x20;

    An overall trust score based on:

    * Number of successfully completed games
    * Total revenue volume processed
    * Completion rate (successful games / total games)
    * Consistency over time

    Higher CR = higher visibility in search and discovery = more players = more revenue. \
    CR incentivizes creators to build fair, well-structured games.<br>
*   **Death Games Rate (DG) Soon!** &#x20;

    The percentage of a creator's games that ended in refund. DG is critical because:

    * Games that fail can run for days or weeks before being refunded
    * Players who exit early from failing games pay a 15% fee
    * A high DG (e.g., 95%+) means the creator consistently creates games that don't attract enough players

> A high CR and low DG indicate a reliable creator. Players are encouraged to check these metrics before participating.

**How to use these metrics:** Before joining any lottery, check the creator's profile. A creator with many completed games, high total volume, and a DG below 10–15% is generally trustworthy.

***

#### Odds, RTP & Economics

Salatto operates with full economic transparency:

* **RTP per game type** — disclosed before participation, locked at launch
* **Expected odds** — calculated from total tickets and winning tickets, clearly shown
* **Platform fee** — 5% from successful games only
* **Creator margin** — set by the creator and visible
* **Prize pool split** — exact distribution shown before ticket purchase

{% hint style="info" %}
There is no hidden house edge. The economics of every game are visible and auditable.
{% endhint %}

***

#### Smart Contract Security

Smart contract security is Salatto's highest priority. The team's position:

> "You can fix a product, but you can't fix a reputation. If we compromise on security once, we lose trust forever."

**Current security measures:**

* Rigorous internal testing of all smart contract functions
* Testing across all game state transitions (Create, Active, Processing, Completed, Refunded)
* Transaction history verification on dev chain before production deployment

**Planned security measures:**

* Professional smart contract audit (evaluating firms and tools)
* Open-source security tool scanning
* Formal security audit report published publicly (details will be published when completed)
* Bug bounty program for responsible vulnerability disclosure — coming soon
* Vulnerability reporting — contact the team via Support

***

#### What Salatto Cannot Do

* Manipulate draw outcomes
* Block or delay legitimate payouts
* Change game rules after publication
* Access your wallet or private keys
* Reverse completed transactions
* Override VRF randomness
* Selectively favor certain participants

The platform is designed so that even Salatto itself cannot interfere with fair game execution. The code is the only authority.

***
