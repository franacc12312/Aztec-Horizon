## 1) Vision and value proposition

**What it is**: a privacy native membership and subscriptions platform on Aztec, where fans support creators or communities with recurring payments, identities and amounts stay private by default, creators publish only the minimum needed for social proof and compliance.

**What it solves**

- Ends public doxxing of supporters and whales, avoids wallet based profiling.
- Stops parasitic copycats who scrape on chain payments to target top fans.
- Gives creators clean aggregates and selective disclosure, no public spreadsheets of patrons.

**Expected customer outcome**

- Higher conversion and retention for sensitive or premium communities, safer experience for supporters, credible public totals without leaking member lists, simple private receipts for taxes and accounting.

---

## 2) Target users and needs

**Primary personas**

1. **Creator or brand**: wants predictable recurring revenue, control over what is shown publicly, easy perks by tier, simple reporting.
2. **Supporter or member**: wants to subscribe privately, get access, manage plan and payments, receive a private receipt.
3. **Community manager**: wants to gate content and perks, handle upgrades and pauses, run campaigns, see aggregates only.
4. **Compliance and legal**: wants selective disclosure for specific cases, with approvals and audit trail.
5. **Auditor or partner**: wants proof that totals and payouts reconcile, without a dump of member identities.

**Jobs to be done**

- As a creator, I want to monetize memberships without exposing my patrons.
- As a supporter, I want to subscribe and upgrade privately, and get a receipt for my records.
- As compliance, I want to reveal only what a lawful request requires, with signatures and logs.

---

## 3) Core use cases

1. **Private recurring memberships**: monthly or yearly plans, tiers like bronze, silver, gold, perks mapped to each tier, no public member list.
2. **Backer only drops**: private posts, files, livestream keys, discount codes, all gated by private credentials.
3. **Founder tier**: limited seats, higher price, optional public badge with alias, never a full roster.
4. **Corporate sponsorship**: brands support a creator, public page shows sponsor logo only if they opt in, private receipts and contracts.
5. **Anonymous benefactor**: single high value support, proof of contribution shown to the creator, identity remains private.

---

## 4) User experience

### 4.1 Creator flow

1. **Create space**: set brand, tiers, prices, cadence, disclosure preset, what the public page will show after payouts.
2. **Publish**: add posts, files, perks, invite links, optional allowlist for pre release phases.
3. **Monetize**: open subscriptions, see aggregate metrics, subscriber count and MRR, not individual identities.
4. **Payouts**: withdraw privately on Aztec or bridge out if desired, export private statements, run selective disclosure when required.

### 4.2 Supporter flow

1. **Join**: connect wallet, read disclosure policy and perks, select a tier, confirm.
2. **Access**: receive a private membership credential, unlock content, claim perks, manage plan, upgrade or pause.
3. **Receipts**: view private receipts and annual summaries, opt in to a public alias badge if desired.

### 4.3 Auditor flow

- Request specific evidence, for example total paid to a creator in a period, or proof of a single supporter payment, receive proofs and redacted statements, identities revealed only if approved.

---

## 5) Product features

**MVP**

- Private recurring payments, monthly and yearly, one settlement currency at launch, wrapped stablecoin on Aztec.
- Tiered memberships, creator sets perks, limits, and disclosure preset.
- Private membership credentials, used to gate content and perks, no public member directory.
- Creator dashboard with aggregates, MRR, churn, payout history, never raw supporter lists by default.
- Supporter portal with plan management, private receipts, annual summary download.
- Selective disclosure workflow, dual approval, time bound access for case reviews.
- Public landing pages with creator profile, tier descriptions, aggregate supporter count, progress bars.

**Later**

- Multi currency, coupons and trials, bundles and pay what you want ranges.
- Team roles for creators, white label storefronts for agencies and brands, custom domains and themes.
- Private NFT badges and token gated chats, mobile notifications, referral attribution without public links to wallets.
- Webhooks and API for private perk delivery, digital downloads, live events, and gated communities.

**Not in scope now**

- Cross chain subscriptions, fiat on ramps managed by us, secondary markets for memberships.

---

## 6) Privacy and disclosure policy

- **Private by default**: supporter identity, amount, and plan are not public, creator sees aggregates and tier counts, not names by default.
- **Selective disclosure**: case by case, with explicit approvals and audit trail, a single receipt or a defined period, encrypted delivery.
- **Aggregation first**: public shows supporter count, MRR range and milestone progress, never individual payments.
- **Anti correlation**: optional batching windows, rounded denominations, delayed public updates reduce timing analysis and linkability.

---

## 7) Differentiators

- True private memberships on a public blockchain context, creators can prove success without exposing patrons.
- Clean, auditable payouts and statements, selective evidence replaces public payment trails.
- Brand and agency friendly, white label and disclosure presets fit different risk profiles.
- Recurring on chain payments using smart accounts.

---

## 8) Risks and mitigations

- **Regulatory expectations**: optional private KYC for high ticket or restricted markets, clear disclosure templates per jurisdiction.
- **Chargebacks or disputes**: transparent refund policy, dispute inbox, selective disclosure for case handling.
- **Leaked perk content**: private watermarking for files, access tokens with rotation, revoke on abuse.
- **Low early adoption**: seed with known creators, reduced fees, co marketing and case studies.

---

## 9) MVP scope

- One wrapped stablecoin on Aztec, one recommended wallet at launch, Obsidion or compatible.
- Up to 5 tiers per creator, up to 10,000 supporters in pilot, monthly and yearly plans.
- Creator dashboard, supporter portal, public directory with search and tags.
- Configurable platform fee and creator choice to absorb or pass supporter processing fees.

---

## 10) Pricing and commercial

- Platform fee on processed subscription volume, for example 5 to 10 percent depending on tier, volume discounts at scale.
- White label SaaS for brands and agencies, monthly fee, setup cost, custom domain and theme.
- Featured placements in the public directory and campaigns, sold by slot.

---

## 11) Open questions

- Default disclosure preset for new creators, aggregate supporter count only, or count plus MRR range.
- Which ticket sizes and jurisdictions should trigger private KYC gates by default.
- Preferred perk gating methods by vertical, files, livestreams, chats, discount codes.
- Refund policy defaults for monthly and yearly plans, and whether creators can override them.

### **Existing similar projects:**

https://support.patreon.com/hc/en-us

https://blog.onlyfans.com/ultimate-guide-to-onlyfans-features/

https://help.guild.xyz/en/articles/6934383-introduction-to-guild

https://unlock-protocol.com/