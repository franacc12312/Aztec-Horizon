# RLN Private Messaging for Web3 Communities

## 1) Vision and value proposition

**What it is**: an anonymous messaging layer for Web3 communities that uses rate limit nullifiers, each identity can send limited messages per epoch anonymously, spam reveals the sender cryptographically, communities get private by default chat with built in anti abuse.

**What it solves**

- Enables open yet abuse resistant channels without captchas or invasive KYC.
- Preserves pseudonymity while enforcing per identity quotas.
- Provides immutable accountability for moderation without exposing identities.

**Expected customer outcome**

- Safer community chats, less spam and harassment, more candid participation.

---

## 2) Target users and needs

**Primary personas**

1. **DAO Communities and Protocol Teams** want anonymous town halls that are not spammed.
2. **Developers and Contributors** want to ask questions anonymously with limits.
3. **Moderators** want provable rate limits and simple actions.
4. **Security and Compliance** want verifiable logs with minimal exposure.

**Jobs to be done**

- As a member, I want to send messages anonymously within fair limits.
- As a moderator, I want to mute or ban provably abusive senders.
- As a team, I want to host AMAs with anonymous questions, rate limited.

---

## 3) Core use cases

1. **Anonymous AMA channels** with per epoch quotas.
2. **Support queues**, anonymous but limited submissions.
3. **Private council rooms**, membership gated chat with RLN.
4. **Broadcast mode**, team speaks, members ask with RLN guarded turns.

---

## 4) User experience

### 4.1 Member flow

1. **Join** prove membership, receive RLN identity privately.
2. **Send** message with a per epoch proof, receive delivery and a receipt.
3. **Limits** hit quota and wait for the next epoch, or request elevated limits by role.

### 4.2 Moderator flow

- See message metadata and RLN flags, mute or ban identities, request disclosure only on severe abuse cases.

---

## 5) Product features

**MVP**

- RLN identity issuance from a membership group.
- Per epoch messaging proofs and nullifiers.
- Moderation actions, mute, temporary or permanent ban.
- Logs and exports, no message contents exposed outside the room.
- SDK and widgets for Discord style embeds.

**Later**

- Voice questions with RLN gates.
- Per role quotas, sponsors and speakers.
- Cross room federation and bridges.

**Not in scope now**

- End to end media storage, link to external storage providers.

---

## 6) Privacy and disclosure policy

- **Private by default**, sender identities are hidden, only membership is proven.
- **Selective disclosure**, severe abuse cases, dual approval, time bound access.
- **Anti correlation**, optional batching and delay.

---

## 7) Differentiators

- Cryptography backed anti spam, not heuristics.
- Anonymous UX that still feels safe and moderated.
- Easy drop in for existing communities.

---

## 8) Risks and mitigations

- **Sybil joins**, require deposits or verified credentials for RLN issuance.
- **Epoch gaming**, randomize epoch boundaries and per room tuning.
- **Moderator overreach**, logged actions and appeal path.

---

## 9) MVP scope

- One chain, one epoch preset, up to 100 concurrent rooms and 50k MAU.
- Two membership providers integrated.

---

## 10) Pricing and commercial

- SaaS per community and per room.
- Optional per MAU tier and premium support.
- Enterprise, SLAs and compliance reports.

---

## 11) Open questions

- Best default epoch length and quotas.
- Minimal metadata revealed for moderation.
- Bridges to Web2 chat without privacy loss.

---

# PRD, Stealth Pay Inbox for Creators and Merchants, Ethereum or L2

## 1) Vision and value proposition

**What it is**: a payment inbox where every incoming payment lands on a unique stealth address, the receiver consolidates into a private vault, receipts and payout analytics remain private, works on Aztec as a private L2 and on Ethereum or other L2s with stealth address patterns.

**What it solves**

- Stops graph analysis from revealing client lists and revenue.
- Protects VIP customers and pricing, prevents targeted harassment or copycats.
- Keeps accounting verifiable with private receipts and selective disclosure.

**Expected customer outcome**

- Safer monetization, cleaner books, less leakage of business sensitive data.

---

## 2) Target users and needs

**Primary personas**

1. **Creators and Merchants** want to accept crypto without doxxing revenue or clients.
2. **Studios and Agencies** want many inbound payment links per project, single private vault.
3. **Finance** wants reconciliation and exports without exposing counterparties.
4. **Auditors and Platforms** want scoped access for compliance and revenue share.

**Jobs to be done**

- As a merchant, I want one link or QR per campaign that maps to a fresh address, funds auto consolidate privately.
- As finance, I want private receipts and aggregated reports.
- As a partner, I want a proof of payout share without knowing all buyers.

---

## 3) Core use cases

1. **One time sales and tips**, stealth addresses per payer.
2. **Subscriptions**, recurring charges mapped to rotating stealth addresses.
3. **Client invoices**, private memo and receipt, optional escrow.
4. **Payout splits**, private revenue sharing to collaborators.

---

## 4) User experience

### 4.1 Receiver flow

1. **Create inbox** pick chain and mode, Aztec private or Ethereum or L2 stealth mode.
2. **Generate links** per product or client, QR and button embeds.
3. **Receive** payments arrive at unique addresses, dashboard shows private receipts.
4. **Consolidate** automatic or manual private sweep to vault, schedule windows and fees.
5. **Report** export aggregated revenue and selective disclosure packs.

### 4.2 Payer flow

- Open link, choose amount or plan, pay with any compatible wallet, receive a private receipt.

---

## 5) Product features

**MVP**

- Stealth receive on two modes, Aztec private notes, Ethereum or L2 stealth addresses where supported.
- Auto sweep rules and batching windows, anti correlation padding.
- Private receipts, human readable and JSON, with memos.
- Revenue share splits and partner links.
- Exports, CSV and signed summaries.

**Later**

- Payment pages with branded domains and dynamic pricing.
- Payment intents and partial payments.
- Fiat on ramps and tax friendly statements via partners.

**Not in scope now**

- Custodial holding of user funds, full invoicing suite.

---

## 6) Privacy and disclosure policy

- **Private by default**, payer identity and receiver revenue streams stay hidden.
- **Selective disclosure**, case based, invoice or period, with approvals.
- **Anti correlation**, rotating addresses, batching, denomination strategies.

---

## 7) Differentiators

- Works across Aztec and public L2s, a single inbox experience.
- Private revenue analytics and receipts.
- Built in revenue split without leaking collaborator rosters.

---

## 8) Risks and mitigations

- **Fee management on stealth addresses**, auto sweep and sponsor options.
- **User error in consolidation**, preview and dry run sweeps with guardrails.
- **Jurisdictional concerns**, optional zk KYC presets for regulated merchants.

---

## 9) MVP scope

- One private L2, Aztec, and one public L2 or Ethereum mode, up to 10k inbound links and 100k payments in pilot.
- One recommended wallet integration and web embed kit.

---

## 10) Pricing and commercial

- Per transaction fee and Pro subscription for advanced features.
- Enterprise bundles for platforms and marketplaces.
- Optional white label with volume discounts.

---

## 11) Open questions

- Default sweep schedules and gas sponsor models per chain.
- Minimal public metadata for payer trust, for example hash receipts or none.
- Priority currencies and chains for early adopters.

### **Existing similar projects:**

https://rate-limiting-nullifier.github.io/rln-docs/

https://rfc.vac.dev/waku/standards/core/17/rln-relay

https://pse.dev/blog/rate-limiting-nullifier-rln

https://veridise.com/audits-archive/company/ethereum-pse/rate-limiting-nullifier-2023-09-01

https://signal.org/blog/sealed-sender

https://xmtp.org/
