# Private On-chain Lottery and Betting Games

## 1) Vision and value proposition

**What it is**: a privacy native lottery platform on Aztec where players place wagers and receive payouts without exposing identities or bet sizes to the public, with provably fair games and selective, audit ready disclosures for regulators and partners.

**What it solves**

- Eliminates public doxxing of players and high rollers, stops targeting based on visible bankrolls.
- Reduces copycat and collusion risks that come from transparent bet streams and predictable behaviors.
- Enables fair play proofs, compliance friendly reporting, and brand safety, without public leaderboards of who won or lost.

**Expected customer outcome**

- Higher willingness to play from privacy sensitive users and VIPs, better trust due to verifiable fairness, lower support load due to clear receipts and settlements.

---

## 2) Target users and needs

**Primary personas**

1. **Players, casual and VIP**: want fun, fast games, strong privacy, transparent house rules, clear receipts, fast cash in and cash out.
2. **Platform operator**: wants a compliant, scalable venue with predictable margins, configurable house edge, and low fraud.
3. **Partners and affiliates**: want themed rooms and private tournaments for their communities, want revenue share dashboards without leaking player data.
4. **Regulators and auditors**: want selective disclosures of aggregate volumes, payout ratios, and specific case evidence, without open access to player activity.

**Jobs to be done**

- As a player, I want to place private bets and receive instant private payouts, so I can enjoy games without exposing my wallet.
- As an operator, I want provably fair games, built in risk controls, and configurable margins, so I can run a sustainable business.
- As a regulator, I want proof of fairness and settlement without a public firehose of player data.

---

## 3) Core use cases

1. **Private lottery draws**: buy private tickets for a scheduled draw, numbers are committed privately, winner proofs are published, losers remain anonymous.
2. **Instant games**: dice, coin flip, roulette, player places a private bet, receives a private result and payout, the public sees only aggregate stats.
3. **Private tables**: VIP rooms with allowlists and custom limits, member lists are not public, fairness proofs are still public.
4. **Tournaments and raffles**: community events with private entries, public proof of winners, optional sponsor funded prize pools.
5. **Responsible gaming mode**: per player opt in limits, private by default, operator can prove that limits are enforced without revealing player identities.

---

## 4) User experience

### 4.1 Player flow

1. **Join**: connect wallet, accept terms, optional allowlist check for VIP rooms, learn what is private and what is not.
2. **Deposit**: move funds into a private casino balance, see clear fee and limit information.
3. **Play**: choose a game, place a private bet, confirm, receive a private receipt and a real time result.
4. **Cash out**: withdraw privately inside Aztec or bridge out to a public chain if desired, export a private play history for personal records.
5. **Limits and controls**: set optional daily or weekly limits, pause account privately, receive reminders and play time indicators.

### 4.2 Operator flow

1. **Configure**: set house edge ranges per game, min and max bet sizes, VIP allowlists, disclosure presets.
2. **Fund house**: provide bankroll, monitor risk exposure with privacy safe aggregates.
3. **Monitor**: see game volumes, payout ratios, liquidity health, dispute queue, not individual player bet streams.
4. **Compliance**: respond to selective disclosure requests with dual approval and audit trail.
5. **Partners**: create themed rooms, revenue share splits, private affiliate dashboards.

### 4.3 Auditor and regulator flow

- Request a specific report, for example payout ratio in a period or proof that a given jackpot was paid, receive proofs and redacted statements, identities are disclosed only if an approved request covers them.

---

## 5) Product features

**MVP**

- Private lottery, scheduled draws, sealed number commitments, public proof of the winning combination and payouts.
- Private instant games, dice and coin flip at launch, transparent house edge, per game fairness proofs.
- Casino vault, private player balances and private payout receipts, aggregate public stats only.
- Anti sniping and time extension for draws, no exposure of who triggered extensions.
- Responsible gaming controls, optional per player limits, private enforcement proofs.
- Selective disclosure workflow, dual approval, time bound access for case reviews.
- Partner rooms, allowlist gating, private revenue share statements.
- Basic discovery site, game catalog, odds and rules, aggregate volumes, no public leaderboards.

**Later**

- Roulette and blackjack with provable shuffle and seating, tournaments and jackpots, NFT based private passes, mobile notifications, white label skins for partners.

**Not in scope now**

- Cross chain liquidity, sports betting, leveraged products, custody integrations beyond standard portals.

---

## 6) Fairness, privacy, and disclosure policy

- **Private by default**: player identities, bet sizes, and outcomes are not public, individual win announcements are opt in.
- **Provably fair**: every game exposes a clear fairness proof path, seed commitments, reveal verification, payout reconciliation.
- **Selective disclosure**: case by case, with dual approval, for example a jackpot verification, a chargeback dispute, or a regulator request.
- **Aggregation first**: public shows volumes, payout ratios, house edge ranges, game uptime.
- **Anti correlation**: batching, settlement windows, rounded denominations, delayed public updates reduce timing analysis and linkage.

---

## 7) Differentiators

- Real privacy for players and VIPs, combined with provable fairness and operator accountability.
- Creator and partner friendly, private rooms with configurable rules and revenue sharing.
- Compliance ready, selective evidence replaces public bet streams and doxxing.

---

## 8) Risks and mitigations

- **Regulatory complexity**: support jurisdiction based allowlists, optional private KYC for high stakes, legal review of disclosure templates.
- **RNG trust**: use seed commit and reveal with public verification, independent audits, publish deterministic verification scripts.
- **Abuse and laundering**: per game limits, velocity controls, anomaly detection on aggregates, selective KYC triggers for edge cases, never publish player lists.
- **Liquidity stress**: manage bankroll thresholds, pause rules for extreme volatility, publish house solvency proofs in aggregate.

---

## 9) MVP scope

- One stablecoin wrapped on Aztec, one wallet recommended at launch, Obsidion or compatible.
- Lottery draws and two instant games, dice and coin flip, VIP room template.
- Up to 10,000 active players in pilot, per player daily limit configuration, partner room beta.
- Operator dashboard, player portal, auditor request inbox, public catalog with rules and odds.

---

## 10) Pricing and commercial

- House edge per game, configurable within safe bounds, example 1 to 2 percent for dice, variable for lottery.
- Platform fee for partner rooms, percentage of net gaming revenue, tiered by volume.
- White label for brands and DAOs, monthly SaaS and setup fee, custom domains and themes.

---

## 11) Open questions

- Default disclosure preset after jackpots, announce amount only, alias and amount, or nothing.
- Jurisdictions and ticket sizes that should trigger private KYC gates by default.
- Preferred limit presets for responsible gaming, daily caps, time caps, cool off periods.
- Partner revenue share ranges and reporting cadence that communities expect.

### **Existing similar projects:**

https://pooltogether.com/es

https://docs.chain.link/vrf

https://dappradar.com/dapp/etheroll