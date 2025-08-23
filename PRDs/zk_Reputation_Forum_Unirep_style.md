# zk-Reputation Forum, Unirep style

## 1) Vision and value proposition

**What it is**: an anonymous forum and contribution system on Aztec, users post and vote with private identities, reputation is accrued privately and enforced with zk proofs and checkpoints, only policy signals are public.

**What it solves**

- Encourages candid participation without fear of retaliation, while still deterring abuse.
- Provides tamper proof moderation and strike systems without doxxing.
- Enables communities and DAOs to reward or penalize behavior with privacy preserved.

**Expected customer outcome**

- Higher quality discussions, less brigading, accountable yet anonymous participation.

---

## 2) Target users and needs

**Primary personas**

1. **Community Managers and DAO Mods** want enforceable norms without identity leaks.
2. **Contributors and Members** want to post, vote, and build reputation privately.
3. **Foundation or Grants Committee** wants private scoring with verifiable outcomes.
4. **Auditors** want scoped logs of moderation actions.

**Jobs to be done**

- As a member, I want a private handle with verifiable karma and strikes.
- As a mod, I want to apply penalties and know they will be enforced by proofs.
- As a committee, I want to gate perks by reputation thresholds without exposing lists.

---

## 3) Core use cases

1. **Anonymous posting with persistent private identity.**
2. **Karma and strike system**, weekly checkpoints, no raw scores on chain.
3. **Gated perks**, access to channels, bounties, or votes based on reputation.
4. **Appeals and disclosures**, member can selectively prove standing to a reviewer.

---

## 4) User experience

### 4.1 Member flow

1. **Join** prove membership privately, mint a private handle.
2. **Participate** post and vote, receive private receipts and reputation deltas.
3. **Checkpoint** consolidate reputation weekly, one proof replaces many events.
4. **Prove standing** share a one time proof to access perks or apply for grants.

### 4.2 Moderator flow

- Apply positive or negative reputation events, review appeals, request scoped disclosures when necessary.

---

## 5) Product features

**MVP**

- Private handles bound to membership proofs.
- Reputation events, upvotes, downvotes, strikes, with private accumulators.
- Weekly checkpoint proofs, reduce costs and spam.
- Threshold proofs to gate perks, pass or fail only.
- Admin panel, logs, exports.

**Later**

- Topic specific reputations and decay.
- Cross community reputation bridges.
- Integration to Discord and DAO tools.

**Not in scope now**

- Public identity graphs, doxxing tools.

---

## 6) Privacy and disclosure policy

- **Private by default**, posts can be public or private, identities and scores are encrypted.
- **Selective disclosure**, case based, member consent, full audit trail.
- **Anti linking**, optional timing jitter and batch posting.

---

## 7) Differentiators

- True anonymous yet accountable identities, enforced by proofs.
- Low overhead via checkpointing and aggregation.
- Drop in perk gating for DAOs and communities.

---

## 8) Risks and mitigations

- **Sybil attacks**, require membership proofs or deposits.
- **Collusive moderation**, dual approval and transparent policies.
- **Reputation grinding**, per epoch limits and diminishing returns.

---

## 9) MVP scope

- One community, up to 50k members, 1 million events per week aggregated into checkpoints.
- Five perk gates, two moderation roles.

---

## 10) Pricing and commercial

- SaaS per community and per active member.
- Add ons for perk gating and integrations.
- Enterprise governance package, SLAs.

---

## 11) Open questions

- Default strike thresholds and decay schedules.
- Minimum public telemetry the community expects.
- Appeal flows and oversight design.

### **Existing similar projects:**

https://developer.unirep.io/

https://docs.semaphore.pse.dev/

https://sismo.mirror.xyz/MimvqFv45hohMwDBD9rGqY4XGZIHRR8On7nx6q9YFRc

https://www.gitcoin.co/blog/gitcoin-passport-onchain-stamps

https://ethresear.ch/t/anonymous-reputation-risking-and-burning/3926