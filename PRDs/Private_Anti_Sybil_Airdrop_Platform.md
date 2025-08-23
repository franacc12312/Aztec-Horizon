## 1) Vision and value proposition

**What it is**: a privacy native airdrop and claim platform on Aztec that lets projects distribute tokens or NFTs without exposing who claimed, while stopping multi wallet abuse with zero knowledge proofs and single use claim rules.

**What it solves**

- Prevents Sybil farming without forcing full KYC for everyone.
- Protects claimants from public wallet doxxing, balances and claim amounts stay private.
- Gives teams clean, audit friendly summaries, totals and compliance evidence, without public spreadsheets of addresses.

**Expected customer outcome**

- Run fair distributions with high claim rates, low abuse, predictable cost and clear, private receipts for claimants.

---

## 2) Target users and needs

**Primary personas**

1. **Protocol or DAO core team**: wants to run drops that are fair, efficient, and free of drama, needs aggregate reporting for the community and investors.
2. **NFT collections and brands**: want allowlist or loyalty drops without leaking customer data or wallets.
3. **Claimants, users and contributors**: want to verify eligibility and claim once, privately, with a simple guided experience.
4. **Compliance and legal**: want a selective disclosure path to satisfy jurisdictional requests, without opening the full claim list.
5. **Analysts and auditors**: want proofs that the distribution rules were followed, and that totals reconcile.

**Jobs to be done**

- As a core team, I want to upload an eligibility set and rules, fund the pool, and let eligible users claim privately and only once.
- As a claimant, I want to prove I am eligible and claim my reward, without revealing my identity or linking my wallets.
- As compliance, I want to answer regulators with targeted evidence, not with a full dump of addresses and amounts.

---

## 3) Core use cases

1. **One time token airdrop**: a single claim per identity, private by default, unclaimed funds return to the treasury after the window closes.
2. **Retroactive rewards**: reward early users, contributors or governance participants, using private membership proofs, no public lists.
3. **Tiered loyalty drop**: gold, silver, bronze tiers, proof that a claimant belongs to a tier, the exact tier can remain private if the project requires it.
4. **Partner or collab claims**: two projects share an allowlist, membership in either or both can be proven privately.
5. **NFT mint with sealed allowlist**: claim is private, the final owner can choose to reveal or keep the mint anonymous.

---

## 4) User experience

### 4.1 Team flow

1. **Create campaign**: pick asset type and supply, upload eligibility root or connect a data source, define rules, time window, and disclosure preset.
2. **Fund pool**: deposit tokens or NFTs into the vault, see a preview of costs and expected gas.
3. **Publish page**: get a branded claim page, link it from social channels and the website.
4. **Monitor**: see aggregate stats only, claims per hour, percent claimed, geographic compliance flags if enabled.
5. **Close and reconcile**: at window end, settle totals, export reports, optionally roll unclaimed funds to a follow up wave.

### 4.2 Claimant flow

1. **Check eligibility**: connect wallet, verify membership privately, no public logs of failed checks.
2. **Claim once**: confirm the claim, receive a private receipt and the asset in a private balance.
3. **After claim**: keep the asset private inside Aztec, or withdraw to a public chain if desired, the choice belongs to the user.

### 4.3 Auditor flow

- Request an aggregate report, receive proofs for total supply, total claimed, and single use claims, along with a signed statement of rules applied, without identities of claimants unless a selective disclosure is approved.

---

## 5) Product features

**MVP**

- One asset type at a time, wrapped ERC 20 on Aztec, or wrapped ERC 721 for NFTs, one campaign template.
- Private eligibility proofs, Merkle style lists or score based sets, no public allowlist dump.
- Single use claim, enforced with private nullifiers, protects against multi wallet farming.
- Fixed claim window, unclaimed funds auto return to the treasury or roll to a new campaign.
- Branded claim page and links, mobile friendly, clear privacy education banners.
- Aggregate dashboard, total eligible, total claimed, claim rate, waves, not individual addresses.
- Private receipts for claimants and a signed summary for the team.
- Optional allowlist gate for VIP campaigns, membership proven privately.

**Later**

- Multi asset and multi wave campaigns, booster rules, and vesting schedules.
- Referral attestations without revealing the referrer identity to the public.
- Gas sponsorship options and delegated claiming for users with limited funds.
- Dispute and appeal workflow, with selective disclosure per case.
- White label mode for agencies and brands, custom domains and themes.

**Not in scope now**

- Cross chain distribution, on chain reputation scores outside of approved data sources, secondary market integrations.

---

## 6) Privacy and disclosure policy

- **Private by default**: claims, identities and amounts are not public.
- **Selective disclosure**: per request, the team can reveal a specific claim to an authorized party, with dual approval and audit trail.
- **Aggregation first**: public site shows totals, claim rate and waves only, not a list of wallets.
- **Anti correlation**: optional padding, denominations and settlement windows reduce timing analysis and linkage.

---

## 7) Differentiators

- Fair distributions without doxxing users, and without blanket KYC for everyone.
- Single use claims that are auditable, without exposing individual addresses.
- Creator controlled disclosure presets, brand safety and compliance friendly.

---

## 8) Success metrics

- Claim rate by campaign, percent of eligible users who claimed.
- Fraud rate, attempted multi claims prevented per 1,000 claims.
- Time to settle a campaign, error rate below 1 percent.
- Fee revenue per campaign, repeat customers and partner referrals.
- Zero unauthorized disclosures, zero reconciliation mismatches.

---

## 9) Risks and mitigations

- **False eligibility or data errors**: use signed inputs and clear data provider contracts, provide dry runs and previews before going live.
- **Sybil evasion**: combine private nullifiers with optional private KYC or proof of personhood for high value campaigns.
- **User confusion about privacy**: explain what stays private and what can be revealed, with clear in product copy.
- **Low early adoption**: curate design partners, offer reduced fees and co marketing to seed the first waves.

---

## 10) MVP scope

- One campaign template, one asset, up to 50,000 eligible users per campaign in the pilot.
- One recommended wallet at launch, Obsidion or compatible.
- Team dashboard, branded claim page, auditor export, basic API for status checks.
- Configurable platform fee, default claim fee absorbed by the team or charged to claimants.

---

## 11) Pricing and commercial

- Platform fee per campaign, a flat setup fee plus a small percent of distributed value, or a pure SaaS plan for frequent users.
- White label and agency tier, monthly fee and reduced per campaign costs.
- Grants or discounts for public goods and non profits.

---

## 12) Launch roadmap

- **Pilot**: 3 projects, 5 campaigns total, gather feedback on claim UX and dashboards.
- **Open beta**: add multi wave campaigns, referrals, gas sponsorship and dispute handling.
- **GA**: white label, full API, partner distribution and case studies.

---

## 13) Open questions

- What default disclosure preset suits most teams, nothing public, winner and price for NFTs, or aggregate totals only.
- What data providers and proof sources are acceptable for eligibility, and in which jurisdictions.
- Should the platform handle optional private KYC for high value campaigns, or integrate partners.
- What refund policy should apply for unclaimed funds and failed or disputed claims.

### **Existing similar projects:**

https://enzyme.finance/

https://dhedge.org/

https://docs.mellow.finance/