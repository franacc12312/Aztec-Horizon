## 1) Vision and Value Proposition

**What it is**

A work contract and escrow platform for clients and contractors, terms are private, funds are secured on Aztec, and payouts are automated upon milestone approval or proof of delivery.

**What it solves**

- Guarantees payment to contractors without exposing rates and scopes publicly.
- Protects clients from non delivery, reduces disputes with verifiable milestones.
- Supports pseudonymous contributors and DAOs with receipts and selective disclosure.

**Expected outcome for the client**

- Faster hires, fewer disputes, predictable cash flow, and confidential pricing.

---

## 2) Target Users and Needs

**Primary personas**

1. **Client PM or Founder** wants milestone based contracts with secure funds and private terms.
2. **Contractor or Studio** wants guaranteed payout and privacy for rates and identity.
3. **DAO Ops** needs repeatable SOW flows and private multi sig approvals.
4. **Arbiter or Compliance** needs scoped access for dispute resolution or audits.

**Jobs to be Done**

- As a client, I want to lock funds and release on delivery with minimal friction.
- As a contractor, I want private receipts and predictable payout windows.
- As DAO ops, I want bulk SOWs with consistent rules and approvals.

---

## 3) Main Use Cases

1. **Milestone SOW** fixed price per milestone, auto release on approval.
2. **Time and materials** capped hourly with weekly approvals.
3. **Bug bounty or micro task** many small escrows, quick settlement.
4. **IP transfer** proof of assignment triggers final payout and rights transfer.

---

## 4) User Experience

### 4.1 Client flow

1. **Create SOW** pick template, define scope, milestones, cap, delivery formats.
2. **Fund escrow** deposit stablecoin privately into contract vault.
3. **Approve** review submissions, approve or request changes, partial releases supported.
4. **Close** final acceptance, IP assignment acknowledgment, auto receipts.

### 4.2 Contractor flow

1. **Accept** review SOW, sign privately, see funded status.
2. **Submit** upload deliverable hash or link, add private notes.
3. **Get paid** on approval, instant private payout and receipt.

### 4.3 Dispute flow

- Either party opens dispute, optional third party arbiter receives selective disclosure, decision executes payout split.

---

## 5) Product Features

**MVP**

- SOW templates, variable and milestone fields, attachments.
- Private escrow on Aztec, per milestone notes and receipts.
- Submission and approval workflow, partial releases, cancellations with rules.
- IP assignment acknowledgments and private certificates.
- Dispute module with role based access and time boxed windows.
- Dashboard for both sides, status and ledger, exports.

**Later roadmap**

- Rate cards, preferred vendor lists, bulk SOW generation.
- On chain reputation badges with privacy preserving proofs.
- Invoicing connectors and tax friendly statement exports.

**Out of scope for now**

- Marketplace matching engine, fiat payouts, complex factoring.

---

## 6) Privacy Rules and Policies

- **Private by default** rates, amounts, scopes, deliverable hashes, and identities.
- **Selective disclosure** for disputes, compliance, or references, scoping and expiry required.
- **Anti correlation** optional batching of payouts and rounded denominations.

---

## 7) Differentiators

- True escrow with private terms, not just public multisig.
- Smooth milestone UX for both sides, built for DAOs and studios.
- Evidence backed approvals and receipts without leaking strategy.

---

## 8) Risks and Mitigations

- **Scope creep** template guardrails and change order flows.
- **Non delivery** staged funding, partial releases, arbitration connectors.
- **Key management** support hardware wallets and org roles with recovery.

---

## 9) MVP Scope

- One stablecoin, up to 20 milestones per SOW, up to 500 concurrent SOWs per org.
- One dispute role and one arbitration partner.
- Exports, CSV and signed JSON receipts.

---

## 10) Commercial Model and Pricing

- Platform fee on released amounts, example 1 to 2 percent, volume discounts.
- Pro plan for org roles, custom templates, and dispute credits.
- Enterprise, SSO, SLAs, private arbitration partner integration.

---

## 11) Open Questions

- Default dispute windows and burdens of proof.
- IP assignment language per jurisdiction, provide templates or partners.
- Refund logic for cancellations, pro rata and fees.

### **Existing similar projects:**

https://help.fiverr.com/hc/en-us/articles/360010560178-Working-with-milestones-Freelancer-guide

https://kleros.io/escrow/

https://docs.openzeppelin.com/contracts/2.x/api/payment

https://support.upwork.com/hc/en-us/articles/211062568-How-Upwork-protects-your-payments