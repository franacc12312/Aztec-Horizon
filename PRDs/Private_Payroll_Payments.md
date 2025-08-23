## 1) Vision and Value Proposition

**What it is**: A B2B platform that enables companies to pay salaries and fees in crypto privately on Aztec. Amounts and the identities of payer and recipient are not publicly exposed. The company retains full control to meet audit requirements with “selective disclosure.”

**What it solves**

- Prevents exposure of salaries, bonuses, and vendor details on public explorers.
- Reduces reputational or security risks for employees and executives.
- Allows audits and compliance without revealing entire books.
- Maintains a familiar payroll experience, with clear receipts and reports.

**Expected outcome for the client**

- Run payroll as easily as in a Web2 tool, but with on-chain privacy, cryptographic traceability, and a reduced surface for information risk.

---

## 2) Target Users and Needs

**Primary personas**

1. **HR / Payroll Manager**: Wants to load payroll, validate it, and execute without friction. Needs process status, error handling, and receipts for employees.
2. **Finance / Treasury**: Needs to fund the account, reconcile, and export aggregated reports. Seeks cost and timing predictability.
3. **Compliance Officer**: Requires a simple flow to handle legal or audit requests with selective disclosure, with approval trails.
4. **External Auditor**: Expects verifiable payment evidence and aggregated reports that do not reveal unnecessary PII.
5. **Employee / Contractor**: Wants to be paid on time, see a private receipt, and use or withdraw funds when desired.

**Jobs to be Done**

- "As HR, I want to run a payroll cycle without exposing sensitive information and with clear confirmation that everyone got paid."
- "As Finance, I want to reconcile payments and export reliable aggregated data."
- "As Compliance, I want to respond to audits revealing only what’s necessary and leaving evidence of approval."
- "As an Employee, I want to receive, understand my receipt, and have access to my funds without third parties seeing my salary."

---

## 3) Main Use Cases

1. **Monthly / biweekly payroll**: CSV or UI upload, review, confirmation, batch execution, private receipts.
2. **Contractor payments**: Ad hoc payments with private memo and individual proof.
3. **Bonuses and retroactive payments**: Additional payments in the same period without breaking the privacy of amount patterns.
4. **Annual audit**: Generation of verified aggregated reports and, if needed, selective disclosure of specific payments with documented authorization.

---

## 4) User Experience

### 4.1 Company Flow

1. **Onboarding**: Create organization, invite HR, Finance, and Compliance. Choose default stablecoin and pay period.
2. **Funding**: Transfer funds to the company’s private vault in the app. Display available balance and cost projection.
3. **Employee setup**: Upload via CSV or individually. The app guides minimal data capture and wallet linking.
4. **Prepare cycle**: Select period, import amounts, view validations, and simulate costs and timing.
5. **Confirm and execute**: HR confirms, the app shows real-time progress, automatic retries, and results per person.
6. **Post-execution**: Access to private receipts, aggregated exports, and reconciliation dashboard for Finance.
7. **Compliance**: Guided audit flow with a record of who disclosed what, when, and to whom.

### 4.2 Employee Flow

1. **Receiving**: Wallet/Email notification, private receipt with breakdown of concepts.
2. **Using funds**: Private transfer within the network or withdrawal to a public chain if desired.
3. **History**: View previous payments, only visible to them, with totals per period.

---

## 5) Product Features

**MVP**

- Company, role, and permission management (Owner, HR, Finance, Compliance).
- Employee creation and editing, bulk upload via CSV.
- Batch payroll execution with pre-validations and progress bar.
- Private receipts for employees, downloadable in readable format.
- Aggregated reports per period without identities or individual amounts.
- **Selective disclosure** flow with Compliance approval and audit trail.
- Accounting exports, CSV and JSON signed with hash and batch metadata.
- Notifications for key events, automatic retries for recoverable failures.

**Later roadmap**

- Multi-stablecoin support, multiple frequencies, deduction and benefit templates.
- Integrations with common HRIS and ERPs, webhooks, and public API.
- Aggregated analytics and budgeting panel without exposing sensitive data.
- Compliance checklist per jurisdiction and automated reminders.

**Out of scope for now**

- Automatic tax calculation per country, handled through configurable deductions.
- Full accounting management, provided via exports and connectors.

---

## 6) Privacy Rules and Policies

- **Privacy by default** in all payments and receipts, no public exposure of identities or amounts on explorers.
- **Data minimization**: capture only what’s strictly necessary to run payroll.
- **Selective disclosure**: access controls, dual approval, and audit logs. Disclose the minimum required for a limited time.
- **Aggregated reports**: period metrics without PII or individual amounts.
- **Retention**: clear retention and deletion policies upon request.

---

## 7) Differentiators

- **End-to-end confidentiality**, no public exposure of salaries or payment patterns.
- **Built-in compliance control**, avoids exporting full books.
- **Familiar HR experience**, with Web2 simplicity and verifiable blockchain security.

---

## 8) Risks and Mitigations

- **De-anonymization via patterns**: use denominations and execution windows, optional payment padding.
- **Operational errors**: preview, strong validations, retries, and idempotency per cycle.
- **Changing regulatory requirements**: disclosure templates per jurisdiction and ongoing legal advisory.

---

## 9) MVP Scope

- One wrapped stablecoin, one default pay period, up to 100 employees per pilot company.
- Recommended wallet for employees, with notifications and private receipts.
- Aggregated exports and reports ready for accounting and audit.

---

## 10) Initial Commercial Model and Pricing

- **Starter**: up to 50 employees, fixed monthly price plus per-payment fee.
- **Growth**: up to 500 employees, volume-based pricing with discounts.
- **Enterprise**: SSO, SLA, and support, custom pricing.

---

## 11) Open Questions

- Which jurisdictions to prioritize for disclosure templates?
- Which wallets to support in addition to the recommended one for employees?
- What level of detail do clients want in default aggregated reports?

### **Existing similar projects:**

https://gusto.com/

https://www.deel.com/

https://www.request.finance/

https://docs.superfluid.org/