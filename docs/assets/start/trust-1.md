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

***

#### Non-Custodial by Design

Salatto does not hold user funds outside of active game participation.

* Your wallet remains under your control at all times
* Funds are locked in game contracts only during active participation
* Winnings are distributed directly to your wallet

**Salatto will never ask for:**

* Your private keys or seed phrase
* Direct token transfers outside the platform
* Access to your wallet beyond standard transaction approvals

If anyone asks for these — it is a scam.

***

#### Creator Reputation System

Not all creators are equal. Salatto provides tools to help players assess creator reliability:

* **Creator Rating (CR) Soon!** — an overall trust score based on a creator's history, completion rates, and player feedback
* **Death Games Rate (DG) Soon!**  — the percentage of a creator's games that ended in refund rather than a successful draw

A high CR and low DG indicate a reliable creator. Players are encouraged to check these metrics before participating.

***

#### Odds, RTP & Economics

Salatto operates with full economic transparency:

* **RTP per game type** — disclosed before participation and locked at launch
* **Expected odds** — clearly shown for every game
* **Platform fee** — 5% from successful games only
* **Creator margin** — set by the creator and visible

There is no hidden house edge. The economics of every game are visible and auditable.

***

#### Security Practices

* Smart contract audits — planned (details will be published when completed)
* Bug bounty program — coming soon
* Vulnerability reporting — contact the team via Support

***

#### What Salatto Cannot Do

* Manipulate draw outcomes
* Block or delay legitimate payouts
* Change game rules after publication
* Access your wallet or private keys
* Reverse completed transactions

The platform is designed so that even Salatto itself cannot interfere with fair game execution.
