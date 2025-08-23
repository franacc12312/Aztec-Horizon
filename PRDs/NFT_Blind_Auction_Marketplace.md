# NFT Blind Auction Marketplace

## 1) Vision and value proposition

**What it is**: a privacy native NFT marketplace on Aztec where bids and bidder identities stay private during the auction, and optionally after settlement. Creators run sealed auctions that discover fair prices without reputation bias or last minute sniping.

**What it solves**

- Stops copy trading and bid sniping driven by public mempools and visible leaderboards.
- Removes reputation bias, buyers are not judged by their wallet name or history.
- Protects creators and collectors from exposing strategy, holdings, or budgets.

**Expected customer outcome**

- Higher fairness and price discovery quality, less manipulation, safer participation by high profile collectors, audits and disclosures only when explicitly authorized.

---

## 2) Target users and needs

**Primary personas**

1. **Creators and brands**: want fair price discovery without harassment, want control over what gets revealed and when.
2. **Collectors and whales**: want to bid confidently without revealing identity, strategy, or wallet size.
3. **Traders and market makers**: want a competitive venue without public information leakage, want settlement guarantees.
4. **Curators or auction partners**: want to run themed auctions with their own rules and allowlists.
5. **Compliance and auditors**: need selective disclosure, not a public feed of all bids and identities.

**Jobs to be done**

- As a creator, I want to auction a piece without revealing who is bidding or how much until the end, so I can get a fair outcome.
- As a collector, I want to place and update blind bids that only I and the contract can validate, so I avoid being targeted or outed.
- As a curator, I want to run private allowlist sales that still prove fairness and absence of double bidding.
- As an auditor, I want to validate that rules were followed, and that the winner was computed correctly, without exposing everyone else.

---

## 3) Core use cases

1. **Single piece sealed auction**: one of one NFT, private bids during the window, optional reveal of winner name and amount at close.
2. **Collection drop with blind bids**: multiple pieces, bidders can submit a private bid per token, winners are assigned at close, losers remain anonymous.
3. **VIP allowlist sale**: curated list of addresses can bid, membership is proven privately, the public cannot infer who is on the list.
4. **Charity auction**: the organizer can publish an aggregate report, total funds raised and winner proof, without exposing non winning bidders.
5. **Private OTC style sale**: creator invites a small set of bidders, the winner is revealed only to the seller and the winner.

---

## 4) User experience

### 4.1 Seller flow

1. **Create auction**: connect wallet, select NFT, choose auction type, set reserve price and schedule, decide what to reveal after close.
2. **Deposit NFT**: escrow it in the marketplace vault, get a signed receipt, see the auction preview page.
3. **Run**: monitor aggregate interest, number of bids and time remaining, not the identities or amounts.
4. **Close and settle**: at end time the system computes the winner privately, publishes the minimal agreed data, transfers funds and NFT.
5. **Post sale**: download settlement report, optional public post with redacted data.

### 4.2 Bidder flow

1. **Join**: connect wallet, pass allowlist if required, see auction info and rules, not other bids.
2. **Place blind bid**: enter amount, confirm, get a private receipt in the wallet, option to increase or cancel within rules.
3. **End of auction**: if winner, receive the NFT and a private receipt of payment, if not, automatically reclaim funds, identity remains private.

### 4.3 Observer flow

- See the catalog, creator page, auction schedules and aggregate stats like number of bids, not the bid ladder or wallet names. After settlement, see only what the seller configured for disclosure.

---

## 5) Product features

**MVP**

- Single item sealed first price auction with reserve and time window.
- Private bids and bidder identities by default, no public mempool, no public order book.
- Escrow vault for custody of the NFT during the auction, settlement transfers NFT to winner and funds to seller.
- Allowlist gating with private membership proofs, useful for VIP or brand events.
- Private receipts for bidders and sellers, exportable as human readable PDFs and machine readable JSON.
- Minimal public page with creator info, artwork, rules, and aggregate stats.
- Platform fee on settlement and optional listing fee.

**Later**

- Second price sealed auctions, Dutch with private thresholds, batch and collection wide auctions.
- Royalties and splits, creator revenue share wallets, private by default, with optional public proofs.
- White label storefronts for brands, themeable pages and custom disclosure policies.

**Not in scope now**

- Cross chain settlement, lending or buy now with financing, on chain royalties enforcement across external markets.

---

## 6) Privacy and disclosure policy

- **Private by default**: bids, identities, and bid amounts are not exposed to the public.
- **Selective disclosure**: creators can choose what to reveal after settlement, winner alias only, winner and price, price range, full winner proof for PR, or nothing.
- **Aggregation first**: public pages show only aggregate metrics, number of bids, time left, reserve met flag.
- **Anti correlation**: the platform offers optional padding strategies, denominations, and batch settlement windows to reduce linkage of wallets and bids.

---

## 7) Differentiators

- True sealed bidding in a public blockchain context, buyers and amounts stay private during the auction.
- Fair price discovery without reputation bias or copy trading from whales and bots.
- Creator controlled disclosure, sellers decide the narrative and privacy envelope post sale.

---

## 8) Risks and mitigations

- **Low trust in fairness**: provide clear proofs and audits of winner computation, publish verifiable settlement hashes.
- **Wash trading or collusion**: apply risk controls, reputation scoring for sellers, optional KYC for high value auctions.
- **Thin liquidity at launch**: curate early creators, incentive campaigns, and guarantees like reduced fees in the first months.
- **User confusion about privacy**: in product education with clear banners, what is public and what is private at each stage.

---

## 9) MVP scope

- One auction type, sealed first price, one NFT standard, wrapped ERC 721 on Aztec, one settlement currency, a stablecoin supported on Aztec.
- Up to 100 bidders per auction, one wallet type recommended at launch, Obsidion or compatible.
- Seller dashboard, bidder receipts, public catalog, basic search and filtering.
- Fees configurable, default platform fee, creator can opt to cover bidder fees.

---

## 10) Pricing and commercial

- Platform fee on successful settlement, for example 2.5 percent of sale price.
- Listing fee for premium placement on the catalog, weekly or per slot.
- White label, monthly SaaS for brands and agencies, custom domains and themes.

---

## 11) Open questions

- What default disclosure preset should new auctions use, winner only or winner and price.
- What royalty model do creators expect, do they need private revenue splits.
- Will high value auctions require KYC for sellers and or bidders.
- How much aggregate market data should be public for discovery without harming privacy.

### **Existing similar projects:**

https://www.sothebys.com/en/calendar?locale=en

https://www.christies.com/

https://docs.soliditylang.org/en/latest/solidity-by-example.html#simple-open-auction