## 1) Vision and value proposition

**What it is**: a privacy native asset management platform on Aztec where fund managers run strategies without exposing trades or positions to the public, while investors enjoy private balances and selective, audit ready disclosures.

**What it solves**

- Protects investment strategy from copy trading and MEV surveillance.
- Shields investor identities and allocations from competitors and data brokers.
- Enables compliance workflows with selective disclosure, not full data dumps.

**Expected customer outcome**

- Operate a professional fund with crypto native settlement and privacy by default, offer investors bank grade discretion, provide regulators and auditors the evidence they need with minimal disclosure.

---

## 2) Target users and needs

**Primary personas**

1. **Fund Manager**: wants to execute trades and rebalancing without leaking alpha, needs robust reporting and fee collection.
2. **Operations and Compliance**: needs controlled disclosure, investor registry management, audit trails, and incident free settlements.
3. **Investors, retail or professional**: want private subscriptions and redemptions, clear statements, fast settlement windows.
4. **Auditors and regulators**: want proofs that rules were followed, NAV and fee calculations are correct, and that redemptions match subscriptions.
5. **Partners, custodians and oracles**: need clean interfaces and logs, not investor level data.

**Jobs to be done**

- As a manager, I need to move size without revealing portfolio composition, so I preserve alpha and pricing power.
- As an investor, I need to subscribe and redeem privately, and receive a clear statement of holdings and fees.
- As compliance, I need to answer inquiries with selective evidence, not by exporting the whole ledger.
- As an auditor, I need to validate NAV and fees with verifiable proofs, and record approvals for any disclosure.
    
    ---
    

## 3) Core use cases

1. **Actively managed fund**: periodic subscriptions and redemptions, private rebalancing, performance and management fee collection.
2. **Fund of funds**: the top level fund deploys into other strategies privately, only aggregate exposures are optionally disclosed.
3. **Locked vault strategy**: fixed lockup with a clear schedule of redemptions, reduced leakage and execution risk for long horizon bets.
4. **Stealth reallocation event**: manager rotates sectors or assets without public signaling, then publishes an aggregate report.
5. **Selective due diligence**: manager shares private performance proofs and holdings ranges with a prospective institutional LP.

---

## 4) User experience

### 4.1 Manager flow

1. **Create fund**: define name, share class, base currency, fees, lockup rules, disclosure preset.
2. **Onboard investors**: invite or approve wallets, optional private allowlist or KYC gate.
3. **Accept capital**: open a subscription window, show soft cap and timing, collect private deposits.
4. **Run strategy**: execute trades and treasury actions privately, monitor aggregate metrics, not investor level balances.
5. **NAV and fees**: set NAV periods, review fee preview, approve collection, publish a redacted statement to investors.
6. **Redemptions**: open a redemption window, process requests, settle privately, provide statements.

### 4.2 Investor flow

1. **Join**: connect wallet, pass allowlist or KYC if required, review terms and disclosure policy.
2. **Subscribe**: choose amount, confirm, receive a private receipt and fund share position.
3. **Hold**: view statements, performance charts with privacy safe aggregation, receive notices about windows.
4. **Redeem**: request redemption during a window, receive private payout and a statement of fees.

### 4.3 Auditor flow

- Request an aggregate report, receive proofs for NAV computation, subscriptions and redemptions by window, fee accruals, and policy compliance, without investor identities, unless a selective disclosure is approved.

---

## 5) Product features

**MVP**

- Private subscriptions and redemptions, one base currency, one share class.
- Periodic NAV calculation with privacy safe statements, investors see their balances, the public sees only aggregate AUM if enabled.
- Private strategy operations, rebalancing and treasury actions are not publicly visible.
- Performance and management fees with clear investor level breakdown in private statements.
- Subscription and redemption windows with caps, waitlists, and status updates.
- Allowlist or private KYC gating, membership proven without exposing identities.
- Selective disclosure workflow with dual approval and audit trail.
- Export of investor statements in human readable PDF and machine readable JSON.

**Later**

- Multiple share classes and currencies, benchmark reporting, and high watermark support.
- Streaming fees, hurdle rates, carried interest and crystallization schedules.
- Secondary transfer of fund shares under manager approval, private OTC board.
- White label manager portal, API for reporting, mobile notifications.

**Not in scope now**

- Cross chain settlement, on chain leverage, external custody integrations beyond basic portals.

---

## 6) Privacy and disclosure policy

- **Private by default**: investor balances, flows, and portfolio actions are not public.
- **Selective disclosure**: compliance can approve case by case disclosures, for example a single investor statement or a regulator request.
- **Aggregation first**: public pages show only aggregate fund metrics, AUM, subscriber count, performance ranges if enabled.
- **Anti correlation**: optional padding, standard denominations, and settlement windows reduce timing analysis and linkage.

---

## 7) Differentiators

- Strategy protection, trades and allocations are not reverse engineered by bots or rivals.
- Investor privacy with auditable operations, a combination that traditional blockchains cannot offer.
- Compliance ready, selective evidence replaces full database exports.

---

## 8) Risks and mitigations

- **Valuation accuracy**: publish clear NAV rules, use trusted price sources, provide proofs and third party attestation options.
- **Liquidity risk**: use lockups, gates and notice periods, publish a calendar and honor it.
- **Regulatory expectations**: offer KYC, AML and travel rule friendly disclosures without breaking privacy for everyone.
- **Low trust at launch**: seed with reputable managers, audits, and transparent fee policies.

---

## 9) MVP scope

- One fund template, one share class, one base stablecoin on Aztec.
- Weekly subscription and redemption windows, up to 200 investors per fund in the pilot.
- Manager dashboard, investor portal, auditor request inbox.
- Configurable platform fee and default performance and management fee presets.

---

## 10) Pricing and commercial

- Platform fee on AUM or on fee revenue, for example 10 percent of protocol collected fees.
- Fund setup fee and monthly SaaS for managers, white label optional.
- Discount tiers for larger AUM and multi fund groups.

---

## 11) Open questions

- Preferred NAV frequency, daily, weekly, or monthly.
- Which assets and venues the strategy is allowed to access, and what disclosure level is acceptable.
- Whether KYC is mandatory for some jurisdictions and ticket sizes.
- What default disclosure preset best fits, aggregate AUM only, or AUM plus ranges of performance.