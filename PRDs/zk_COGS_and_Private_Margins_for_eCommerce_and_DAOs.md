# zk-COGS and Private Margins for eCommerce and DAOs

## 1) Vision and value proposition

**What it is**: a privacy native proof layer on Aztec where organizations attest to cost of goods sold, discounts, and margin ranges, counterparties and auditors verify compliance and fairness with zero knowledge proofs, no raw costs or price lists are exposed.

**What it solves**

- Proves margin compliance for grants, partnerships, or procurement without leaking supplier prices or internal costs.
- Reduces negotiation and copycat risk from public disclosures of COGS and discounts.
- Streamlines audits with range proofs and selective evidence, not full spreadsheets.

**Expected customer outcome**

- Faster partner onboarding, fewer audit cycles, trusted commercial claims, competitive information stays confidential.

---

## 2) Target users and needs

**Primary personas**

1. **Brand or DAO Treasury** wants to prove margins or price floors to funders and partners without exposing internals.
2. **Retailer or Marketplace** wants assurance that listed margins and promotions follow agreed bands.
3. **Supplier and Finance** want reusable proofs across multiple counterparties, minimal manual work.
4. **Auditor or Regulator** wants scoped access and verifiable evidence on demand.

**Jobs to be done**

- As a brand, I want to prove my margin is within agreed bounds without disclosing my BOM or vendor quotes.
- As a marketplace, I want to enforce discount rules and price integrity with cryptographic receipts.
- As an auditor, I want to check random samples and receive a redacted proof pack with approvals and logs.

---

## 3) Core use cases

1. **Partner margin certification**, prove product or category margin in a pre agreed band.
2. **Promo and discount guardrails**, prove a discount ratio did not exceed policy.
3. **Grant or rebate programs**, prove spend split, marketing to COGS to overhead, matches rules.
4. **Price floor enforcement**, prove net price stayed above a threshold after fees and coupons.

---

## 4) User experience

### 4.1 Organization flow

1. **Define policy** select bands and thresholds per category or SKU.
2. **Ingest inputs** upload private cost components and price events, compute commitments locally.
3. **Prove** generate zk proofs per batch or period, publish a verifiable certificate.
4. **Share** send verification links or API responses to partners, no raw data exposure.
5. **Audit** open a time bound disclosure session for specific SKUs or time ranges if required.

### 4.2 Partner and auditor flow

- Verify a certificate for a SKU or time window, see pass or fail with reason codes, optionally request a scoped disclosure pack.

---

## 5) Product features

**MVP**

- Policy builder for bands and thresholds, per SKU or category.
- Range proofs and ratio proofs over private cost and price notes.
- Certificate registry, batch binding, expiry, revocation.
- Verifier widget and API, pass or fail with codes.
- Selective disclosure sessions, dual approval and audit logs.

**Later**

- BOM attestation chaining from suppliers, reusable upstream proofs.
- Time weighted margin proofs for dynamic pricing.
- Consumer facing trust badges with aggregate only signals.

**Not in scope now**

- Public storage of invoices or BOMs, full ERP replacement.

---

## 6) Privacy and disclosure policy

- **Private by default**, costs, fees, and supplier identities stay encrypted.
- **Selective disclosure**, scoped by SKU, period, and fields, time bound access with approvals.
- **Aggregation first**, certificates reveal only compliance signals and reason codes.

---

## 7) Differentiators

- Verifiable margin compliance without revealing COGS.
- Reusable proofs across counterparties, fewer bespoke audits.
- Works for brands, suppliers, DAOs, and marketplaces.

---

## 8) Risks and mitigations

- **Garbage in, garbage out**, signer allowlists and random audits, attestations by finance.
- **Stale inputs**, expiries and proof freshness checks.
- **User confusion**, plain language policies and reason codes.

---

## 9) MVP scope

- Three proof types, margin band, discount ratio, price floor, one verifier API, one marketplace plugin.
- Pilot with up to 100 organizations and 10,000 certified SKUs.

---

## 10) Pricing and commercial

- SaaS per org seat plus per certificate fee.
- Partner bundles for marketplaces and procurement networks.
- Enterprise, SLAs and custom policy mapping.

---

## 11) Open questions

- Default band templates per vertical.
- Minimal public metadata on certificates for trust without leaks.
- Evidence retention windows and legal posture per region.

---

# PRD, Private Proof of Funds for OTC and Launchpads

## 1) Vision and value proposition

**What it is**: a proof and settlement layer on Aztec where buyers and participants attest to solvency or balance ranges, counterparties and launchpads verify eligibility, and deals settle privately with optional escrow and atomicity.

**What it solves**

- Enables OTC and token sale participation without revealing exact balances or wallet graphs.
- Reduces fraud and time to close by replacing manual screenshots and KYC over sharing with zk proofs.
- Supports selective disclosures for compliance and post trade audits.

**Expected customer outcome**

- Faster closings, cleaner compliance, lower information leakage, predictable settlement.

---

## 2) Target users and needs

**Primary personas**

1. **OTC Desks and Brokers** want fast solvency checks and private settlement.
2. **Launchpads and Issuers** want eligibility gating by balance band or lockup, no PII.
3. **Buyers and Funds** want to prove capacity without exposing portfolio strategy.
4. **Compliance** wants scoped evidence for large tickets.

**Jobs to be done**

- As a buyer, I want to prove I hold at least X in approved assets without revealing exactly how much or where.
- As a desk, I want atomic two leg settlement once conditions are met.
- As compliance, I want a minimal proof pack for tickets above a threshold.

---

## 3) Core use cases

1. **Balance band proof** for allowlists or tiers, for example 100k to 500k.
2. **Asset composition proof**, at least N percent in stablecoins or whitelisted tokens.
3. **Lockup and vesting control**, proofs bound to escrow and cliff events.
4. **Atomic OTC**, tokens for cash leg settle privately with conditions and timeouts.

---

## 4) User experience

### 4.1 Participant flow

1. **Link assets** deposit or attest holdings into private notes, choose policy.
2. **Prove** generate a reusable proof, receive a private eligibility receipt.
3. **Join** present proof to desk or launchpad, no balance or address leakage.
4. **Settle** if accepted, settle via private escrow and atomic swap if required.

### 4.2 Desk or launchpad flow

- Configure policy, review incoming proofs, approve or reject, monitor escrow, finalize and export receipts.

---

## 5) Product features

**MVP**

- Range and composition proofs over private asset notes.
- Eligibility receipts with expiry and revocation.
- Deal escrow, single or two leg, with timeouts and dispute rules.
- Selective disclosure packs for large tickets.
- Admin console and SDK for integrators.

**Later**

- Oracle adapters for off chain attestations, custodians and banks.
- Multi party club deals and pro rata allocations.
- Programmatic vesting and transfer restrictions.

**Not in scope now**

- Fiat custody, brokerage licensing, public order books.

---

## 6) Privacy and disclosure policy

- **Private by default**, balances, addresses, and allocations stay encrypted.
- **Selective disclosure**, case based, dual approval, full audit logs.
- **Anti correlation**, optional batching of receipts and delayed windows.

---

## 7) Differentiators

- Reusable solvency proofs across desks and sales.
- Atomic settlement with confidential terms.
- Compliance ready without centralizing user PII.

---

## 8) Risks and mitigations

- **Oracle or price manipulation**, use TWAP feeds and conservative haircuts.
- **Expired proofs**, short lived receipts and freshness checks.
- **Deal disputes**, clear timeouts, mediators, and payout splits.

---

## 9) MVP scope

- One stablecoin, three policy templates, one escrow template.
- Up to 500 active deals, up to 50k proofs per month.

---

## 10) Pricing and commercial

- Per proof fee and per settled deal fee, volume discounts.
- Enterprise launchpad plan, SLAs and custom policies.
- Referral share with custody or fiat partners later.

---

## 11) Open questions

- Priority assets and chains for supported holdings.
- Default thresholds for enhanced compliance.
- Legal language in receipts that counterparties expect.

### **Existing similar projects:**

https://www.gs1.org/standards/epcis

https://www.ibm.com/think/insights/driving-value-the-untapped-potential-of-fsma-rule-204d-data