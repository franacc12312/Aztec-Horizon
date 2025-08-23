- Stops competitive intelligence leaks that happen on public chains, buyer and seller strategies stay private.

## 1) Vision and value proposition

**What it is**: a privacy native marketplace on Aztec where organizations and individuals buy and sell datasets and insights, payments and identities are private by default, delivery and entitlements are proven with zero knowledge proofs and cryptographic receipts.

**What it solves**

- Reduces legal and reputational risk, no public lists of who bought what or for how much.
- Enables trust without custodians, private settlement, auditable entitlements, selective disclosures only when required.

**Expected customer outcome**

- Faster, safer data deals, predictable fulfillment, clean audit trails, higher conversion from cautious buyers and reputable sellers who demand confidentiality.

---

## 2) Target users and needs

**Primary personas**

1. **Data sellers, companies or researchers**: want to monetize datasets, protect IP, control licenses and disclosures, avoid doxxing of clients.
2. **Data buyers, funds, product teams, analysts**: want to discover and buy quality data, keep strategy and budgets private, receive verifiable access quickly.
3. **Compliance and legal**: want to enforce allowed use and jurisdictions, handle case based disclosures, avoid publishing full ledgers.
4. **Auditors and partners**: want proofs that deliveries match invoices and licenses, without exposing counterparties.

**Jobs to be done**

- As a seller, I want to list and deliver a dataset, the buyer pays privately, I get a receipt and funds, my client list stays confidential.
- As a buyer, I want to verify integrity and sample quality before purchase, then get the key or API access privately, finance cannot tie the purchase back to my strategy.
- As compliance, I want to answer a lawful request with the minimum necessary evidence, with approvals and logs.

---

## 3) Core use cases

1. **One time dataset sale**: encrypted file delivery, buyer gets a private license receipt and decryption key after payment.
2. **Subscription data feed**: recurring private payments, rotating keys or API tokens, access auto renews until cancelled.
3. **Insight report with attachments**: seller provides a redacted preview, full report unlocks after settlement, buyer identity remains private.
4. **Cohort or query service**: buyer submits a private query against a seller’s data, receives an aggregated result, raw rows never leave the seller.
5. **Joint research grant**: sponsor funds a dataset collection, milestone based private releases, public page shows only aggregate progress.

---

## 4) User experience

### 4.1 Seller flow

1. **Create listing**: title, abstract, schema or sample preview, license terms, price, disclosure preset, delivery method, encrypted file or API.
2. **Deposit proofs**: upload integrity hash and small sample, store encrypted payload off chain, publish only the checksum and metadata.
3. **Go live**: listing appears with aggregate stats, no public waitlist of wallets.
4. **Fulfill**: after private payment, the system releases a decryption key or issues a private access token, seller sees funds and a private receipt.
5. **After sale**: handle updates, revoke or rotate keys if terms require it, respond to dispute requests through a guided, private workflow.

### 4.2 Buyer flow

1. **Discover**: browse catalog, search by domain and schema, view previews and quality signals, see price and license, no public watchlist.
2. **Purchase**: pay privately, receive a private license receipt and delivery, verify integrity locally.
3. **Manage**: view entitlements, keys, renewal dates, download receipts for internal accounting, request selective disclosure certificates if needed.

### 4.3 Auditor and compliance flow

- Request a period report or a case, receive proofs for totals, deliveries and license enforcement, specific identities are disclosed only if an approved request covers them.

---

## 5) Product features

**MVP**

- Private settlement for listings, one settlement currency at launch, wrapped stablecoin on Aztec.
- Encrypted delivery, off chain storage managed by the seller or a neutral bucket, on chain records keep only content hash and license ID.
- Private license receipts for buyers and sellers, machine readable JSON and human readable PDF.
- Preview and integrity, hash based integrity proofs, small redacted samples, optional third party attestations.
- Subscription mode, monthly renewals with key rotation and late payment grace windows.
- Dispute and refund workflow with selective disclosure, dual approval, time bound access for case reviewers.
- Catalog and search, categories, tags, schema hints, aggregate stats only, number of sales, rating ranges.
- Compliance presets, allowed jurisdictions, data classes, retention notices, all enforced through policy checks at purchase time.

**Later**

- Auctions and negotiated deals, private bids and counter offers, sealed until settlement.
- Clean room queries, buyers run approved queries, receive aggregates, raw data never leaves the seller perimeter.
- Watermarked delivery, privacy preserving watermarking and trap records for leak tracing, visible only to the seller.
- Partner marketplace, white label storefronts for data vendors, custom domains and themes.
- Multi asset and multi chain bridges, multiple currencies, fiat on ramp via partners.
- API key metering with ZK counters, prove usage without leaking endpoints or volumes.

**Not in scope now**

- Hosting raw PII on chain, DRM that edits buyer devices, cross chain settlement beyond standard portals at launch.

---

## 6) Privacy and disclosure policy

- **Private by default**: buyer and seller identities, amounts, and items are not exposed publicly, public pages show only listing metadata and aggregates.
- **Selective disclosure**: case based reveals with explicit approvals and audit trail, for example a specific invoice for a regulator or a court order.
- **Aggregation first**: catalogs show sales counts, rating ranges, update cadence, never client rosters.
- **Anti correlation**: optional batching windows, rounded pricing tiers, delayed public stats reduce timing analysis and linkability.

---

## 7) Differentiators

- Confidential commerce for data, private settlement combined with verifiable delivery and entitlements.
- Trust without custodians, proofs of integrity and receipt replace centralized clearinghouses.
- Compliance friendly, selective evidence replaces spreadsheets of sensitive buyer and seller data.

---

## 8) Risks and mitigations

- **Illegal or restricted data**: enforce category and jurisdiction presets, optional private KYC for sensitive classes, takedown process with selective disclosure.
- **Low data quality or bait and switch**: preview rules, verified attestations, escrowed payouts with auto release on buyer confirmation or timeout.
- **Leakage and redistribution**: watermarking options, license keys per buyer, selective disclosure for enforcement, trap records for forensic confirmation.
- **Deanonimization by timing and price**: batching, rounded tiers, delayed public stats, optional private negotiations.
- **Trust at launch**: seed with reputable vendors and design partners, independent audits of preview and integrity paths.

---

## 9) MVP scope

- One settlement currency, one recommended wallet at launch, Obsidion or compatible.
- File based listings, encrypted archives up to a defined size, API access as a gated URL with private keys.
- Up to 500 sellers and 2,000 buyers in pilot, catalog, search, filters, watchlist in the user dashboard only.
- Seller portal, buyer portal, auditor request inbox, public catalog with tags and basic SEO.

---

## 10) Pricing and commercial

- Platform fee per transaction, for example 10 percent of sale price, volume discounts for large vendors.
- Subscription fee for data vendors who need white label storefronts, custom domains and themes.
- Featured placement in catalog, sold by slot, optional co marketing packages.
- Grants and discounted pricing for academic research and public goods data.

---

## 11) Open questions

- Which verticals to seed first, finance, e commerce, geospatial, cybersecurity, scientific research.
- What default disclosure preset suits most listings, aggregates only, or aggregates plus price bands.
- Do vendors prefer escrowed payouts with auto release, or instant release with higher dispute fees.
- What watermarking approach is acceptable to buyers, subtle record tags, per buyer file variants, or none by default.
- Which data classes require private KYC or attestation at purchase time, and how strict should the presets be.

### **Existing similar projects:**

https://aws.amazon.com/data-exchange/

https://other-docs.snowflake.com/en/collaboration/collaboration-marketplace-about

https://learn.microsoft.com/en-us/azure/databricks/marketplace/

https://oceanprotocol.com/build/data-marketplaces/

https://streamr.network/discover/marketplace