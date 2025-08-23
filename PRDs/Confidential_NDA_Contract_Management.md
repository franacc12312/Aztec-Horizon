## 1) Vision and Value Proposition

**What it is**

A platform for drafting, signing, and managing NDAs with on chain proofs and private by default contents on Aztec. Parties sign the agreement, its existence and timestamp are verifiable, the terms and identities remain confidential unless selectively disclosed.

**What it solves**

- Keeps sensitive terms and counterparty identities private while providing tamper proof evidence of execution.
- Simplifies NDA workflows for pseudonymous teams, vendors, and DAOs.
- Reduces operational and legal risk from data leaks and document sprawl.

**Expected outcome for the client**

- Faster NDA turnaround, a single source of truth for status, private document custody, and selective disclosure for audits or disputes.

---

## 2) Target Users and Needs

**Primary personas**

1. **Founder or Deal Lead** needs fast NDA execution without exposing identity or pricing signals.
2. **Vendor or Candidate** wants a simple signature flow and private receipt, without doxxing to a public explorer.
3. **Legal Counsel** needs immutable evidence of who signed and when, with limited disclosure.
4. **Compliance or Auditor** needs scoped access to verify existence and parties, not full document dumps.

**Jobs to be Done**

- As a deal lead, I want a signed NDA before sharing materials, verified and timestamped.
- As a vendor, I want a secure, quick signing process with a private receipt.
- As legal, I want to disclose only what is necessary to an authorized party.

---

## 3) Main Use Cases

1. **Mutual NDA for exploratory call** quick draft from template, sign, share private data room link.
2. **One way NDA for recruiting** secure candidate materials, minimal identity leakage.
3. **Cross company NDA portfolio** manage many NDAs, filter by counterparty and term, private status badges.
4. **Dispute path** selectively disclose the agreement and signatures to an arbiter.

---

## 4) User Experience

### 4.1 Creator flow

1. **Draft** choose template, fill variables, attach exhibit if needed.
2. **Invite** add counterparty email or wallet, set expiry, select disclosure preset.
3. **Sign** sign privately, get a private receipt, contract moves to pending counterparty.
4. **Complete** counterparty signs, agreement is notarized with timestamp, both receive private copies.
5. **Manage** renew, terminate, or disclose with approval and audit trail.

### 4.2 Counterparty flow

1. **Open link** review terms, identity policy, download redacted preview if allowed.
2. **Sign** confirm identity privately, sign, receive private receipt and copy.
3. **Access** see status, renewal date, disclosure history if any.

### 4.3 Legal or auditor flow

- Request a **disclosure session**, receive a time bound link with scoped access, approval is logged, only the agreed fields are visible.

---

## 5) Product Features

**MVP**

- Template library, variables, versioning.
- Private signature and timestamp on Aztec, proof of execution, agreement hash notarization.
- Counterparty invite via email or wallet, deadline and reminders.
- Private storage of document blobs, encrypted at rest, controlled decryption.
- Selective disclosure sessions with scope, expiry, and dual approval.
- Dashboard with statuses, renewals, and export of audit logs.

**Later roadmap**

- Multi language templates, clause library with playbooks.
- Bulk NDA programs for vendor or candidate pipelines.
- Integration to CRM, ATS, and data rooms via webhooks and API.
- Arbitration connector for one click dispute disclosure.

**Out of scope for now**

- Automatic clause negotiation, full contract redlining editor.
- Native fiat billing for legal services.

---

## 6) Privacy Rules and Policies

- **Private by default** agreement text, party identities, signatures, and exhibits remain encrypted.
- **Selective disclosure** scoped fields only, time bound links, dual approval, full audit trail.
- **Data minimization** collect only necessary identifiers and contact points.
- **Revocation** creator can revoke old links and rotate access keys.

---

## 7) Differentiators

- Verifiable signatures and timestamps with strong privacy.
- DAO friendly, supports pseudonymous parties and zk attestations.
- One click selective disclosure that satisfies auditors without oversharing.

---

## 8) Risks and Mitigations

- **Misunderstood privacy scope** clear in product education and preview of what will be revealed.
- **Key loss** recovery with pre designated recovery contacts or custodial key options.
- **Template misuse** provide vetted defaults and warnings for risky edits.

---

## 9) MVP Scope

- 1 jurisdiction neutral template family, 1 storage backend, up to 1,000 active NDAs per org.
- Email and wallet invites, one disclosure role for legal.
- CSV export of metadata and signed JSON receipts.

---

## 10) Commercial Model and Pricing

- Per seat plus volume based NDA execution, free tier with monthly cap.
- Add on for disclosure sessions and extended retention.
- Enterprise plan, SSO, DPA, SLA.

---

## 11) Open Questions

- Which identity signals to support, email, DID, zk KYC badge.
- Minimum default fields in a standard disclosure, parties and date only, or include governing law.
- Retention policy defaults per industry.

---

### **Existing similar projects:**

https://www.dropbox.com/sign

https://juro.com/contract-templates/nda-non-disclosure-agreement

https://docs.openlaw.io/beginners-guide

https://ironcladapp.com/lp/non-disclosure-agreements-with-ironclad/