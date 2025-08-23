## 1) Vision and value proposition

**What it is**: a privacy native retirement plan on Aztec where employees and contributors make recurring deposits, employers match, balances grow in approved strategies, and all sensitive data stays private by default. Auditors and regulators can receive selective proofs on demand, no full ledger exposure.

**What it solves**

- Protects personal savings, salaries, employer policies, and allocations from public chain analytics.
- Reduces operational risk and data leakage in payroll linked contributions and vesting.
- Delivers verifiable compliance and solvency without sharing unnecessary PII or position level detail.

**Expected customer outcome**

- Run a compliant, portable retirement plan with cryptographic receipts, private balances, predictable operations, and clear selective disclosures when required.

---

## 2) Target users and needs

**Primary personas**

1. **Employer HR and Payroll Manager** wants to onboard employees, configure matching rules, execute contributions, and see status, without leaking salaries or identities.
2. **Treasury or Plan Sponsor** wants funding predictability, policy controls, and aggregated reporting, with private underlying positions.
3. **Employee or Contributor** wants easy enrollment, private balance view, risk choice, benefit statements, and portability between employers.
4. **Fund Manager or Strategy Provider** wants to accept plan inflows and publish performance proofs without revealing full books.
5. **Compliance Officer and External Auditor** wants scoped evidence for contributions, vesting, and solvency, with approvals and audit trail.

**Jobs to be done**

- As HR, I want to run recurring contributions and employer match with private receipts and automatic retries.
- As a sponsor, I want to prove the plan meets funding and policy constraints without exposing individual balances.
- As an employee, I want to see my private balance and vesting, change risk bands, and transfer my plan when I change jobs.
- As compliance, I want to answer audits with minimal, time bound disclosures that show rules were enforced.

---

## 3) Core use cases

1. **Recurring contributions and matching** linked to payroll cycles, private receipts per participant, aggregated plan report.
2. **Vesting and eligibility** private schedules for employer match and incentives, unlocks after cliffs or tenure, minimal public signals.
3. **Portfolio selection** employee chooses a lifecycle or risk band, strategy manager publishes performance proofs and fee receipts, allocations stay private.
4. **Portability and rollovers** transfer a participant account to a new employer plan or an individual plan, identity and history stay private, entitlements preserved.
5. **Withdrawals and retirement payouts** authorized flows, hardship exceptions with approvals, disclosures limited to case and period.
6. **Compliance and solvency checks** proofs of contribution rates, fee caps, and funding status, no raw position data disclosed.

---

## 4) User experience

### 4.1 Employer and plan sponsor flow

1. **Create plan** choose jurisdiction presets, contribution limits, match rules, vesting templates, risk bands enabled.
2. **Onboard employees** import via CSV or HRIS, send private enrollment links, set default band and match.
3. **Fund and execute** deposit plan funds to private vault, run contribution cycle, view progress and exceptions.
4. **Review and export** aggregated reports by period, policy compliance signals, download signed summaries.
5. **Compliance** open selective disclosure sessions for audits, scope by employee, period, and fields, approvals logged.

### 4.2 Employee and contributor flow

1. **Enroll** accept terms, link wallet, pick risk band, optional beneficiaries, receive a private welcome receipt.
2. **Contribute** see contributions and match accrue privately, notifications for deposits, vesting, and rebalancing.
3. **Manage** change allocation within allowed windows, request statements, initiate rollover or withdrawal when eligible.
4. **Proofs** generate one time proofs for mortgage, visa, or benefits, for example balance within a range, without revealing exact amounts.

### 4.3 Fund manager and auditor flow

- **Manager** registers approved strategy, receives net inflows from the plan’s private vault, publishes performance and fee proofs, no investor list exposure.
- **Auditor** requests a proof pack for a period, gets contributions, match, fees, and solvency signals, identities and positions remain private unless explicitly disclosed.

---

## 5) Product features

**MVP**

- Plan templates, contribution limits, employer match rules, and vesting schedules.
- Private participant accounts and receipts, balances and entitlements as private state.
- Batch contribution engine, retries, idempotency, progress dashboard.
- Risk bands with whitelisted strategies, performance and fee proofs, allocation updates in windows.
- Selective disclosure sessions, dual approval, time bound access, full audit log.
- Aggregated reports by period, totals and policy pass or fail with reason codes.
- Exports, CSV and signed JSON summaries for finance and audit.
- Notifications and reminders, enrollment, funding, contribution success or failure.

**Later**

- Lifecycle default funds that auto shift risk by age or tenure, private rules and public proofs.
- Rollovers across employers and to individual plans, automated portability flows.
- Multi asset support, multiple stablecoins and tokenized treasuries, adapters for custodial partners.
- Tax wrappers and jurisdiction presets, benefit statements localized.
- Robo rebalancing and personalized nudges, privacy preserving analytics.
- Integration connectors, HRIS and payroll, webhooks and API.

**Not in scope now**

- Direct custody of fiat, regulated brokerage functions, tax filing, or personalized investment advice.

---

## 6) Privacy and disclosure policy

- **Private by default** contributions, balances, vesting, allocations, and participant identities remain encrypted on Aztec.
- **Selective disclosure** case based, smallest necessary fields, explicit approvals, time limits, complete audit trail.
- **Aggregation first** public or partner facing materials show totals, ranges, and pass or fail signals, never participant rosters.
- **Anti correlation** batching windows, denomination strategies, optional delayed stats to reduce linkage by timing.

---

## 7) Differentiators

- End to end confidentiality for retirement savings with verifiable compliance and solvency proofs.
- Portability and rollovers without exposing personal histories or employer policies.
- Simple HR and employee UX, on chain integrity, no public leakage of sensitive financial data.

---

## 8) Risks and mitigations

- **Regulatory uncertainty** address with jurisdiction presets, disclosure templates, and legal review, start with pilot markets.
- **Smart contract and strategy risk** third party audits, guarded launches, whitelisted strategies, circuit breakers and pause controls.
- **De anonymization by patterns** batching, randomized execution windows, rounded contribution tiers, optional payment padding.
- **Key loss** recovery flows, role based permissions, hardware wallets, organization recovery for plan keys.
- **Liquidity and market risk** risk bands with conservative defaults, disclosures of methodology, and rebalancing rules.

---

## 9) MVP scope

- One wrapped stablecoin on Aztec, one default contribution frequency, monthly.
- Three plan templates, simple percent match, three vesting templates.
- Two risk bands, conservative and balanced, with fee and performance proofs.
- Up to 25 employers and 2,000 participants in pilot, contribution cap per cycle.
- One recommended wallet and web app for HR and employees.

---

## 10) Pricing and commercial model

- **SaaS plan** per employer seat, tiered by number of participants.
- **Platform fee** per contribution batch, volume discounts.
- **AUM based fee** optional, for managed strategies, with transparent caps.
- **Enterprise** SSO, SLAs, custom disclosures, and integrations.

---

## 11) Open questions

- Which jurisdictions to target first, default disclosure artifacts regulators will accept, and retention policies.
- Preferred strategy menu and fee caps for pilots, custodial partner requirements if any.
- Default vesting and eligibility rules by market, hardship withdrawal policies.
- Portability flows between employers, what metadata needs to travel and what can remain private.
- Minimum public metadata for participant trust, for example hash receipts, or none by default.

### **Existing similar projects:**

https://www.guideline.com/

https://humaninterest.com/solutions/401k-for-small-business/

https://www.betterment.com/work

https://www.forusall.com/

https://www.empower.com/press-center/empower-retirement-realigns-recordkeeping-business-to-enhance-retirement-services-for-institutional-clients