## 1) Vision and value proposition

**What it is**: a plug in voting module for DAOs on Aztec that delivers secret ballots with proof of eligibility and verifiable tallies, members vote privately, only the final result is revealed, optional disclosures for audits.

**What it solves**

- Eliminates coercion, vote buying, and herd effects from transparent voting.
- Preserves member privacy while keeping outcomes trustworthy.
- Enables sensitive decisions without reputational blowback.

**Expected customer outcome**

- Higher participation, more honest votes, cleaner governance signals, lower governance risk.

---

## 2) Target users and needs

**Primary personas**

1. **DAO Core Team** wants reliable outcomes and lower manipulation.
2. **Token Holders or Members** want to vote privately, one person or pro rata by stake.
3. **Governance Facilitator** wants smooth setup and clear results.
4. **Auditor or Legal** wants selective proofs that eligibility rules were enforced.

**Jobs to be done**

- As a member, I want to cast a private vote and verify that it was counted.
- As a facilitator, I want to configure eligibility and quorum, then run votes easily.
- As an auditor, I want to confirm rules were applied without reading individual votes.

---

## 3) Core use cases

1. **Constitutional changes** with high stakes and social pressure.
2. **Budget approvals** that could expose strategy if public.
3. **Elections** for stewards or councils, secret ballots by default.
4. **Emergency measures** with rapid, private voting and immediate execution.

---

## 4) User experience

### 4.1 Admin flow

1. **Configure** choose vote type, token or membership proof, quorum, and timing.
2. **Publish** proposal metadata publicly, keep voter identities and weights private.
3. **Run** monitor anonymous turnout and status.
4. **Finalize** reveal tally, auto execute if passed, publish receipts.

### 4.2 Voter flow

1. **Prove eligibility** wallet generates a private proof, no identity leak.
2. **Vote** submit encrypted choice, receive a private receipt.
3. **Verify** after close, verify inclusion in the tally set.

### 4.3 Auditor flow

- Request a proof pack that shows eligibility checks and tally integrity, no vote contents.

---

## 5) Product features

**MVP**

- Eligibility templates, token weight, one person one vote, role based lists.
- Secret ballot with encrypted votes, commit, tally, finalize.
- Quorum and threshold rules, public result, private receipts.
- Anti replay and one vote per eligible unit.
- Admin dashboard, proposal lifecycle, exports.

**Later**

- Delegations with private delegation links and weights.
- Ranked choice and quadratic options.
- Cross platform adapters for Snapshot or governance UIs.

**Not in scope now**

- Forum or discussion features, handled by adjacent tools.

---

## 6) Privacy and disclosure policy

- **Private by default**, voter choices and identities are encrypted.
- **Selective disclosure**, auditor proofs on demand, no raw ballots.
- **Anti correlation**, optional batching windows and randomized timing.

---

## 7) Differentiators

- True secret ballots on chain, not off chain snapshots.
- Eligibility proofs without doxxing wallets.
- One click integration into existing DAO stacks.

---

## 8) Risks and mitigations

- **Bribery markets off platform**, hidden ballots reduce enforceability of bribes.
- **Low UX familiarity**, guided flows and clear receipts.
- **Edge cases in eligibility**, dry runs and simulation mode.

---

## 9) MVP scope

- One network, three eligibility modes, up to 5,000 voters per vote.
- Ten concurrent proposals per DAO in pilot.

---

## 10) Pricing and commercial

- Per vote fee plus DAO subscription.
- Enterprise governance package, SLAs, custom integrations.

---

## 11) Open questions

- Default receipts content voters expect.
- Minimum public metadata for legal defensibility.
- Delegation disclosure norms by community.

---

### **Existing similar projects:**

https://docs.snapshot.box/

https://www.shutter.network/shielded-voting

https://maci.pse.dev/

https://aztec.network/blog/the-time-nounsdao-got-private-voting

https://forum.safe.global/t/sep-x-partial-private-voting-through-shutter/3558

https://ethresear.ch/t/minimal-anti-collusion-infrastructure/5413