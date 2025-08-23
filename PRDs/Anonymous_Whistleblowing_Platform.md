# Anonymous Whistleblowing Platform

## 1) Vision and value proposition

**What it is**: an Aztec based whistleblowing and compliance channel, reporters submit encrypted cases and evidence, reviewers receive, triage, and respond privately, immutable receipts prove timeline and handling, identity remains protected.

**What it solves**

- Removes fear of retaliation, encourages early reporting with strong anonymity.
- Creates tamper proof logs without exposing sensitive details.
- Simplifies regulator engagement with selective, case scoped disclosures.

**Expected customer outcome**

- Higher quality reports, faster resolution, reduced legal and reputational risk.

---

## 2) Target users and needs

**Primary personas**

1. **Employees or Community Members** want to report issues safely and get updates.
2. **Compliance or Ethics Teams** want secure intake and case management with audit trails.
3. **Executives or Board** want aggregate visibility without access to identities.
4. **Regulators or External Counsel** want scoped evidence with approvals.

**Jobs to be done**

- As a reporter, I want to submit a case and stay anonymous while receiving replies.
- As compliance, I want to manage cases, assign reviewers, and disclose only what is necessary.
- As a regulator, I want evidence that a report was made and handled, with minimal PII.

---

## 3) Core use cases

1. **Internal misconduct reports**, HR, harassment, policy violations.
2. **Fraud or financial irregularities**, attach ledgers or hashes of documents.
3. **Security vulnerabilities**, coordinated disclosure with private bounties.
4. **DAO governance complaints**, routed to an oversight committee.

---

## 4) User experience

### 4.1 Reporter flow

1. **Submit** fill form, attach files or hashes, receive private receipt and case ID.
2. **Dialogue** receive encrypted questions, respond without revealing identity.
3. **Status** view case status and outcomes privately.

### 4.2 Reviewer flow

1. **Triage** see new cases with risk tags, assign owners.
2. **Investigate** request more info, add internal notes, set actions.
3. **Resolve** close with outcomes, generate a redacted report if required.

### 4.3 Regulator flow

- Request a disclosure pack for a case, time bound access, approvals logged, export a verified bundle.

---

## 5) Product features

**MVP**

- Encrypted intake, attachments as encrypted blobs, hash receipts.
- Case management, roles, assignments, SLA timers, and notifications.
- Two way encrypted messaging, reporter remains pseudonymous.
- Selective disclosure packs with scoped artifacts and access expiry.
- Org dashboard, aggregates, no raw identities for executives.

**Later**

- Anonymous eligibility proofs, employee or member status without doxxing.
- Private bounty escrow for security cases.
- Policy templates and playbooks per jurisdiction.

**Not in scope now**

- Full HRIS integration, provide exports and webhooks instead.

---

## 6) Privacy and disclosure policy

- **Private by default**, case data and identities are encrypted end to end.
- **Selective disclosure**, case scoped, dual approval, full audit trail.
- **Least privilege**, role based views, executives see aggregates only.

---

## 7) Differentiators

- On chain integrity with off chain level privacy.
- Built for legal defensibility, receipts, timelines, approvals.
- Works for enterprises and DAOs, not just traditional companies.

---

## 8) Risks and mitigations

- **Malicious or false reports**, rate limits, eligibility proofs, triage scoring.
- **Deanonymization by behavior**, randomize timing, redact metadata, educate users.
- **Key loss**, org recovery flows and hardware wallet support.

---

## 9) MVP scope

- One org, up to 500 active cases, three reviewer roles, one regulator role.
- Email and wallet notifications, CSV and signed JSON exports.

---

## 10) Pricing and commercial

- Per org subscription based on active cases and seats.
- Add on for disclosure packs and long term retention.
- Enterprise, DPA, SLA, audit support.

---

## 11) Open questions

- Eligibility proof options for reporters by org type.
- Default retention and redaction policies per jurisdiction.
- Minimum executive level aggregates for governance reporting.

### **Existing similar projects:**

https://stealthnote.xyz/

https://www.convercent.com/Products/helpline-case-manager

https://www.navex.com/en-us/platform/employee-compliance/whistleblowing-solutions/ethicspoint-essentials/

https://www.integrityline.com/

https://www.speakup.com/

https://www.globaleaks.org/

https://www.washingtonpost.com/anonymous-news-tips