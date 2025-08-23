## 1) Vision and value proposition

**What it is**: a privacy native certification layer on Aztec where manufacturers, suppliers, and auditors issue encrypted attestations about origin, quality, or standards, buyers verify compliance with zero knowledge proofs, sensitive supplier data never leaks.

**What it solves**

- Proves provenance and compliance without exposing supplier lists, prices, or routes.
- Reduces vendor lock in and copycat risk from public disclosures.
- Streamlines audits with selective evidence rather than full data dumps.

**Expected customer outcome**

- Faster certifications, fewer audit cycles, trusted claims at point of sale, competitive information stays confidential.

---

## 2) Target users and needs

**Primary personas**

1. **Brand or Manufacturer** wants to prove standards, origin, or ESG without revealing supply chain structure.
2. **Supplier** wants to provide proofs to customers, keep pricing and sub suppliers private.
3. **Retailer or Marketplace** wants verifiable badges, low friction checks at listing time.
4. **Auditor or Regulator** wants scoped access to underlying attestations with approval trails.

**Jobs to be done**

- As a brand, I want to prove compliance to a retailer without handing over my supplier roster.
- As a supplier, I want to share attestations once, then reuse them across buyers.
- As an auditor, I want to inspect evidence for a sample batch, with a clear chain of approvals.

---

## 3) Core use cases

1. **Origin and material proof**, organic, fair trade, conflict free, region of origin.
2. **Process compliance**, GMP, ISO, temperature chain, environmental thresholds.
3. **Batch specific COA**, certificates of analysis tied to lots, sealed and reusable.
4. **Retail listing checks**, instantaneous proof of claim, no supplier data leakage.

---

## 4) User experience

### 4.1 Brand flow

1. **Create product profile** define claims, standards, and disclosure preset.
2. **Collect proofs** request encrypted attestations from suppliers and labs.
3. **Mint certificate** generate a private certificate bound to batch or SKU.
4. **Share** send a verification link or on chain proof to retailer or consumer app.
5. **Audit** open a time bound disclosure session for an auditor, scope by batch.

### 4.2 Supplier and lab flow

- Receive request, upload signed attestation and optional evidence, store encrypted, reuse across brands under permission.

### 4.3 Retailer and consumer flow

- Verify badge at listing or POS, see compliant or not, optionally view a redacted summary.

---

## 5) Product features

**MVP**

- Private attestations registry, batch level bindings, expiries, and revocations.
- Certificate composer, aggregate proofs into a single verifiable claim.
- Verifier widget and API for retailers, yes or no with reason codes.
- Selective disclosure sessions, dual approval, audit logs.
- Role and org management for brands, suppliers, labs, auditors.

**Later**

- IoT bridge for telemetry commitments, cold chain, energy use.
- Consumer facing app with QR receipts and anti counterfeit checks.
- Multi jurisdiction standards library and mapping.

**Not in scope now**

- Public storage of raw documents, logistics execution or TMS features.

---

## 6) Privacy and disclosure policy

- **Private by default**, attestations and supplier identities remain encrypted.
- **Selective disclosure**, batch scoped, time bound, approval trails.
- **Aggregation first**, public badges and counts, not raw supplier data.
- **Revocation**, immediate propagation of revoked attestations.

---

## 7) Differentiators

- Verifiable compliance without exposing the supply chain.
- Reusable attestations across counterparties, fewer repeated audits.
- Auditor ready workflows with minimum necessary evidence.

---

## 8) Risks and mitigations

- **Fraudulent attestations**, issuer allowlists, signatures, and random audits.
- **Stale proofs**, expiries and automated reminders.
- **User confusion**, simple badges with reason codes and documentation.

---

## 9) MVP scope

- Three claim types, origin, process, COA, one verifier API, one retailer plugin.
- Up to 200 brands, 1,000 suppliers, 10,000 certificates in pilot.

---

## 10) Pricing and commercial

- SaaS per brand seat plus per certificate fee.
- Supplier tier with volume discount, auditor seats billed monthly.
- Enterprise, SLA, custom standards mapping.

---

## 11) Open questions

- Which standards and jurisdictions to seed first.
- Default disclosure presets retailers accept by industry.
- Evidence retention windows per vertical.

### **Existing similar projects:**

https://www.ibm.com/solutions/blockchain-supply-chain

https://tech.walmart.com/content/walmart-global-tech/en_us/blog/post/blockchain-in-the-food-supply-chain.html

https://everledger.io/

https://www.provenance.org/news-insights/blockchain-certification

https://www.blockchain-council.org/blockchain/vechain-thor

https://www.imda.gov.sg/how-we-can-help/digital-utilities/tradetrust

https://x.com/Franacc_