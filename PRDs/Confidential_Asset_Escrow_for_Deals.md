## 1) Vision and Value Proposition

**What it is**

A programmable escrow platform on Aztec for private deals, for example M and A deposits, real estate, OTC token sales, IP transfers. Funds are locked privately, terms are committed privately, release is automated on verified conditions. Selective disclosure supports legal and audit needs.

**What it solves**

- Enables deal certainty without exposing counterparties, prices, or milestones to public explorers.
- Reduces counterparty risk and back and forth, conditions are codified and auto enforced.
- Provides clean evidence for counsel and regulators without leaking strategy.

**Expected outcome for the client**

- Faster closings, fewer disputes, lower information leakage, and trusted settlement for sensitive transactions.

---

## 2) Target Users and Needs

**Primary personas**

1. **Buyer or Acquirer** wants certainty of delivery before releasing funds, while keeping price and identity private.
2. **Seller** wants guaranteed payout on condition fulfilment, and confidentiality for terms and counterparties.
3. **Deal Counsel or Notary** needs scoped visibility to validate documents and milestones.
4. **Escrow Agent or Arbiter** needs a guided dispute path with minimal disclosure.
5. **Compliance Officer** needs proof that checks were performed for high value deals.

**Jobs to be Done**

- As a buyer, I want to lock funds and release when the deed or asset is delivered.
- As a seller, I want private guarantees that funds are real and will release on condition.
- As counsel, I want to validate conditions without exposing full agreements publicly.

---

## 3) Main Use Cases

1. **M and A deposit escrow** funds locked privately, release on signed closing pack or regulator approval.
2. **Real estate sale** price and identities private, release on deed registration attestation.
3. **OTC token sale** tokens and cash leg settle atomically, terms remain confidential.
4. **IP transfer** final payout releases when assignment agreement hash and delivery key are validated.
5. **Milestone deal** staged releases tied to agreed checklist items.

---

## 4) User Experience

### 4.1 Seller flow

1. **Create deal** define asset, conditions, deadlines, who can attest, disclosure preset.
2. **Invite counterparty** send private link, share a redacted term sheet preview.
3. **Deliver** upload or reference evidence, document hashes, oracles, keys.
4. **Settle** receive private payout upon condition verification, get receipts.

### 4.2 Buyer flow

1. **Review** see escrow terms and disclosure policy, verify funds preview and timelines.
2. **Fund escrow** deposit privately to the deal vault, see proof of funds locked.
3. **Approve** confirm each condition as met, or request changes.
4. **Close or cancel** on success, receive the asset, on fail, receive refund per rules.

### 4.3 Counsel and escrow agent flow

- Open a **verification session**, decrypt scoped artifacts, sign attestations, or trigger dispute workflow.

---

## 5) Product Features

**MVP**

- Private escrow vaults per deal, stablecoin at launch, atomic two leg settlement for OTC.
- Term sheet commit and private storage for document hashes, optional encrypted attachments.
- Condition engine, checklists, timeouts, and required attestors or oracle checks.
- Selective disclosure sessions for counsel, notaries, or regulators, dual approval and expiry.
- Dispute module with time boxed windows and arbiter actions, payout split rules.
- Receipts, human readable and JSON, including settlement audit logs.

**Later roadmap**

- Multi asset support and baskets, equity, NFTs, and fiat connectors via partners.
- Streaming escrows and holdbacks, earn and release schedules.
- Syndicated deals and club escrows with many buyers, pro rata rules.
- Bank and trust company partnerships, white label portals.

**Out of scope for now**

- Native fiat custody, brokerage or exchange functions, full legal document editing.

---

## 6) Privacy Rules and Policies

- **Private by default** counterparties, prices, schedules, and documents are encrypted.
- **Selective disclosure** scoped data, role based access, time bound links, audit logs.
- **Anti correlation** optional batching of releases and rounded denominations for large deals.
- **Data minimization** only necessary metadata is collected.

---

## 7) Differentiators

- Confidential terms with programmable enforcement, not just a public multisig.
- Enterprise friendly workflows for counsel and notaries, built in.
- Atomic settlement options for complex deals, without market signaling.

---

## 8) Risks and Mitigations

- **Oracle or attestor risk** multiple attestors and quorum options, clear fallback flows.
- **Key loss** recovery contacts and org roles, hardware wallet support.
- **Regulatory triggers** policy presets for KYC and reporting at size thresholds, selective disclosures.
- **Disputes** time boxed windows, third party arbitrators, evidence checklists.

---

## 9) MVP Scope

- One stablecoin, one oracle connector, one arbitration partner.
- Up to 500 active escrows, up to five conditions per deal.
- One counsel role per deal for verification sessions.

---

## 10) Commercial Model and Pricing

- Fee per escrow and percentage on released amounts, volume discounts.
- Pro plan for role based access, custom conditions, and partner connectors.
- Enterprise, SLAs, white label, bank and trust integrations.

---

## 11) Open Questions

- Priority jurisdictions and notary partners for launch.
- Default dispute timelines and refund policies.
- Which events to make public for market communication, if any.
- KYC thresholds and required issuer list for high value deals.

### **Existing similar projects:**

https://www.escrow.com/support/faqs/how-does-online-escrow-work

https://kleros.io/escrow/

https://copper.co/en/products/clearloop

https://www.qualia.com/

https://www.fireblocks.com/platforms/fireblocks-network/