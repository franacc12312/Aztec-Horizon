## 1) Vision and value proposition

**What it is**: a privacy native lending platform on Aztec that issues loans based on zero knowledge proofs of creditworthiness, borrowers prove income, history or reputation privately, lenders earn yield with risk based pricing, compliance is handled through selective disclosure, never public data dumps.

**What it solves**

- Over collateralization and copyable strategies in public DeFi, borrowers can access credit without revealing salary, identity, or wallet graph.
- Lender front running and social risk, strategies and positions do not leak, only aggregates are visible.
- Compliance friction, regulators and partners get targeted proofs, not the entire ledger.

**Expected customer outcome**

- Borrowers get fair APRs based on private credentials, not on public wallet fame, lenders get predictable returns with clear risk controls, the protocol gains trust through verifiable but private operations.

---

## 2) Target users and needs

**Primary personas**

1. **Borrower, contractor or salaried**, wants a loan without posting large collateral, wants privacy for income and identity, wants transparent schedules and receipts.
2. **Pool manager or lender**, wants to price risk without revealing strategy, wants predictable liquidity, clear performance reports.
3. **Compliance officer**, wants selective evidence for specific cases, wants approvals and audit trail.
4. **Auditor or rating partner**, wants proofs that underwriting rules and caps were enforced, wants NAV and default accounting without user identities.

**Jobs to be done**

- As a borrower, I want to prove I meet eligibility rules, then borrow at a fair rate without doxxing my income or history.
- As a lender, I want to fund pools with defined risk, then monitor performance and fees through aggregate, verifiable reports.
- As compliance, I want to answer a lawful request by revealing the minimal information, with approvals and logs.

---

## 3) Core use cases

1. **Income based personal loan**, borrower proves salary above a threshold or stable payroll, no public proof of employer or payslips.
2. **Reputation backed loan**, borrower proves contribution to a protocol or past on chain repayment behavior, the exact accounts remain private.
3. **Student or training loan**, borrower proves enrollment or completion status privately, disbursements follow milestones.
4. **Merchant working capital**, revenue ranges are proven in ZK from a private data feed, inventory purchases are financed with rolling repayments.
5. **Corporate credit line for DAOs**, members prove governance status or treasury health privately, withdrawals follow configured limits.

---

## 4) User experience

### 4.1 Borrower flow

1. **Check eligibility**: connect wallet, choose loan product, review privacy policy and disclosure presets, run a private eligibility check, pass or fail is shown only to the user.
2. **Offer and terms**: receive a personalized APR range and limit, based on proofs provided, no public identity or data exposed.
3. **Accept and fund**: confirm the loan, receive private funds inside Aztec, repayment schedule and receipts are created for the borrower.
4. **Repay**: make private installments, see progress bars and payoff date, receive an end of loan statement for records.
5. **Optional disclosure**: generate a private certificate for an employer or partner, reveals only what the user agrees to.

### 4.2 Lender or pool manager flow

1. **Create pool**: define strategy, caps, target APR, underwriting rules from approved proof templates, disclosure preset.
2. **Fund and monitor**: deposit liquidity, track utilization, defaults and yield through aggregate dashboards, identities never shown.
3. **Reconcile**: receive periodic private statements, fee breakdowns, proofs that underwriting constraints and limits were enforced.

### 4.3 Auditor and compliance flow

- Request a report for a period or a case, receive proofs for rule compliance, totals, fees and default accounting, specific identities are revealed only if an approved request covers them.

---

## 5) Product features

**MVP**

- One loan product, fixed term, fixed APR band, one settlement currency at launch, wrapped stablecoin on Aztec.
- Private eligibility proofs, income above X, reputation badge, repayment history range, using approved proof templates.
- Private disbursement and repayment, borrower balances and schedules stay private, public sees aggregates only.
- Risk based pricing presets, low, medium, high, tied to which proofs are provided, no public identity ever required by default.
- Pool funding for lenders, utilization and performance via aggregates, periodic distribution of interest.
- Selective disclosure workflow, dual approval, time bound access for regulators or disputes.
- Statements and receipts, human readable for users, machine readable JSON for partners.

**Later**

- Variable rate and revolving credit lines, grace periods, early repayment discounts.
- Multi asset support, employer sponsored payroll deduction, co signer or guarantor proofs.
- Data partner connectors, payroll, education, commerce, with private attestations only.
- Secondary transfers of loan notes between approved parties, white label manager portals.
- Mobile notifications, delinquency reminders, hardship programs, private by design.

**Not in scope now**

- Cross chain settlement, unsecured leverage for trading, direct fiat rails managed by us.

---

## 6) Privacy and disclosure policy

- **Private by default**, borrower identity, income and history are not public, lender strategies and investor lists are not public.
- **Selective disclosure**, case by case, with explicit approvals and audit trail, for example a single borrower certificate or a regulator request tied to a ticket size.
- **Aggregation first**, the public sees outstanding principal, utilization, default rates, not identities or loan level data.
- **Anti correlation**, batching windows, rounded denominations, and delayed public updates reduce timing analysis and linkage.

---

## 7) Differentiators

- Real credit without doxxing, zero knowledge proofs replace data uploads and public links to wallets.
- Strategy protection for lenders, positions and rules are verifiable without revealing edge.
- Compliance ready, targeted evidence replaces spreadsheets of sensitive data.

---

## 8) Risks and mitigations

- **Score gaming or forged attestations**, accept proofs only from vetted issuers, use expiry and revocation, combine multiple proof types, random post issuance audits under selective disclosure.
- **Liquidity crunch**, use subscription and redemption windows for lenders, dynamic caps, throttled originations.
- **Regulatory expectations**, private KYC gates for large tickets or restricted jurisdictions, standard disclosure templates and jurisdiction aware presets.
- **Macro shocks**, tighten underwriting bands, increase reserves, publish aggregate stress indicators to lenders.
- **User misunderstanding of privacy**, in product education, what is private and what can be revealed, simple presets, clear receipts.

---

## 9) MVP scope

- One fixed term personal loan, 3 to 12 months, one wrapped stablecoin on Aztec.
- Private eligibility using one of two templates, income above threshold or reputation badge plus repayment history range.
- Pools funded by whitelisted lenders for the pilot, up to 200 active loans per pool.
- Borrower portal, lender dashboard, auditor request inbox, public page with aggregates.

---

## 10) Pricing and commercial

- Borrower pays an origination fee, example 1 to 2 percent, plus interest, platform takes a share of fees and interest spread.
- Lender pays a management fee from yield, tiered by AUM, discounts at scale.
- White label for partners, monthly SaaS, setup fee, custom disclosure presets.

---

## 11) Open questions

- Which proof templates to ship first, income threshold, employment status, education, on chain repayment history.
- What default APR bands fit early liquidity, how to balance access and risk.
- Which jurisdictions and ticket sizes should trigger private KYC gates.
- What disclosure presets lenders prefer for marketing, AUM only, AUM plus performance range.
- How often to publish aggregate credit metrics publicly, weekly or monthly.

### **Existing similar projects:**

https://maple.finance/

https://truefi.io/

https://www.samsungnext.com/blog/why-we-invested-in-spectral

https://www.forbes.com/sites/davidprosser/2023/04/25/unlocking-lending-with-credoras-privacy-preserving-credit-scoring/

https://www.teller.org/

https://github.com/masa-finance/masa-identity-protocol