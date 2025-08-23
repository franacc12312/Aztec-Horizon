## 1) Vision and value proposition

**What it is**: a privacy native donations platform on Aztec where individuals and organizations can give to causes without revealing donor identity or amount to the public, while recipients can publish trustworthy aggregate totals and accept selective audits when needed.

**What it solves**

- Prevents public wallet doxxing and unwanted profiling of donors and recipients.
- Reduces targeting, harassment, and political or commercial pressure tied to public donation trails.
- Enables transparent outcomes through aggregate reporting and selective disclosure, without exposing every donor.

**Expected customer outcome**

- Higher willingness to give, especially from high profile donors and in sensitive contexts, clean public reporting, lower operational risk from data leaks, simple tax compliant receipts for donors without sacrificing privacy.

---

## 2) Target users and needs

**Primary personas**

1. **Donor, individual or corporate**, wants to support a cause privately, wants a clear receipt and optional recognition without linking their main wallet.
2. **Recipient, NGO or creator**: wants to accept funds safely, show credible public totals, run campaigns, and meet compliance requests without publishing donor lists.
3. **Campaign organizer or fundraiser**: wants branded pages, progress bars, and collaboration tools, without leaking contributor identities.
4. **Compliance officer or legal counsel**: needs selective disclosure, case by case, with approvals and audit trail.
5. **Auditor or grant maker**: needs proofs that totals and flows match, and that restricted funds were honored, without blanket access to donor data.

**Jobs to be done**

- As a donor, I want to give privately, get a receipt for my records, and decide if I reveal anything, to anyone.
- As a recipient, I want to show total raised, meet audit or grant conditions, and protect my community from unwanted exposure.
- As compliance, I want to answer a lawful request by revealing only what is required, with explicit authorization and logs.

---

## 3) Core use cases

1. **Private one time donation**: donor gives once, recipient sees funds, public site shows only aggregate progress.
2. **Private recurring support**: monthly contribution with private receipts and optional end of year summary for the donor.
3. **Matching campaigns**: a sponsor commits to match up to a cap, sponsor identity and cap can be private or partially disclosed.
4. **Emergency fund**: very fast campaign setup for urgent causes, with strict privacy defaults and minimal public footprint.
5. **Corporate giving program**: company funds multiple causes, publishes aggregate CSR reports, keeps individual employee donations private.
6. **Grant tranches with milestones**: donor funds are released privately as milestones are met, public page shows milestone status, not donor details.

---

## 4) User experience

### 4.1 Donor flow

1. **Choose a campaign**: view cause page, impact story, disclosure policy, accepted assets, progress bar that shows aggregates only.
2. **Give privately**: connect wallet, choose amount and frequency, optional message to recipient stored privately, confirm and receive a private receipt.
3. **After donation**: decide whether to generate a tax ready certificate, decide whether to reveal an alias on the public thank you wall, default is not revealed.

### 4.2 Recipient flow

1. **Create campaign**: set goal, deadlines, disclosure preset, branding, accepted assets.
2. **Accept funds**: see private inflows in dashboard, public page shows totals and progress without donor lists.
3. **Withdraw and report**: move funds within Aztec or withdraw to public chains if needed, publish aggregate reports and updates, respond to selective audit requests.

### 4.3 Organizer flow

- Manage multiple campaigns, schedule announcements, enable matching sponsors, export aggregate reports for stakeholders, coordinate selective disclosure with compliance.

### 4.4 Auditor flow

- Request specific evidence, for example total raised in a period or proof that a single large donation exists, receive proofs and redacted statements, only identities that compliance approves are disclosed.

---

## 5) Product features

**MVP**

- Campaign pages with privacy by default, aggregate progress, goal, deadline, story, media.
- Private donations for one asset type at launch, a wrapped stablecoin on Aztec, with private receipts for donors and settlement receipts for recipients.
- Recurring donations, monthly and quarterly, with private scheduling and receipts.
- Matching sponsor mode, sponsor may opt in to reveal name, cap, or stay anonymous while still proving the match on chain.
- Selective disclosure workflow with dual approval, audit trail, and time bound access tokens for recipients and auditors.
- Aggregate reporting, total raised, donor count, average ticket, never a public donor list.
- Basic tax certificate generator for donors, private by default, exported on request.
- Campaign discovery and search without exposing donor activity.

**Later**

- Multi asset support, private NFT rewards, gift cards, and private referral attribution.
- Team roles for recipients, multi language pages, white label microsites for large NGOs and brands.
- Milestone based escrow and release, private grant management, payout schedules.
- Gas sponsorship and delegated donations for users with limited funds.
- Integration with payment links and QR codes for offline events, with private settlement on return.

**Not in scope now**

- Cross chain settlement beyond standard portals, lending or staking of donated funds on third party venues, crowd governance of campaign funds.

---

## 6) Privacy and disclosure policy

- **Private by default**: donor identity, amount, and message are not shown publicly. Recipient can see donor alias only if donor opts in.
- **Selective disclosure**: compliance can approve a case specific reveal, for a single donation or a defined period, with signatures, time limits, and encrypted delivery.
- **Aggregation first**: public pages show totals, progress bars, and campaign metadata only.
- **Anti correlation**: the platform offers batching windows, optional rounded denominations, and delayed public updates to reduce timing analysis and linkability.

---

## 7) Differentiators

- Donation privacy with credible public reporting, donors and recipients choose what to reveal and when.
- Safe space for sensitive causes, removes public on chain trails that lead to harassment or profiling.
- Audit readiness without data dumps, selective proofs replace public donor spreadsheets.

---

## 8) Risks and mitigations

- **Regulatory expectations**: provide optional private KYC for large tickets or restricted jurisdictions, maintain selective disclosure templates and legal review.
- **Abuse or illicit funding**: set per campaign rules and limits, enable case by case KYC gates, maintain an allow or deny list workflow with proofs, never publish donor databases.
- **Deanonimization by timing and amounts**: use batching, rounded denominations, delayed public updates, mix withdrawals.
- **Trust at launch**: seed with reputable NGOs and creators, publish independent audits of the disclosure workflow and aggregate proof methods.

---

## 9) MVP scope

- One wrapped stablecoin on Aztec, one recommended wallet at launch, Obsidion or compatible.
- Up to 10,000 donors per campaign in pilot, single currency goal and progress.
- Recipient dashboard, donor portal with receipt history, public campaign directory with search and tags.
- Configurable platform fee, default fee applied on incoming donations or absorbed by the recipient.

---

## 10) Pricing and commercial

- Platform fee on processed donations, for example 1 to 2 percent, with volume discounts for large NGOs.
- Monthly SaaS for white label campaigns, custom domains and brand controls.
- Sponsor placements on the public catalog, featured campaigns sold by slot.
- Grants and discounted pricing for public goods and emergency relief.

---

## 11) Open questions

- What default disclosure preset should new campaigns use, aggregate totals only, or totals plus donor count.
- What ticket sizes and jurisdictions should trigger a private KYC gate by default.
- Do recipients prefer public thank you walls with opt in donor aliases, or no wall at all.
- Should the platform support optional public proof of reserve for campaign balances, while keeping individual donations private.

### **Existing similar projects:**

https://support.gofundme.com/hc/en-us/articles/203687114-Donating-as-Anonymous-on-the-fundraiser-page

https://help.justgiving.com/hc/en-us/articles/200670401-How-can-I-donate-anonymously-or-hide-the-donation-amount