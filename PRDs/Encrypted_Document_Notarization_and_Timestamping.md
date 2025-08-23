# Encrypted Document Notarization and Timestamping

## 1) Vision and Value Proposition

**What it is**

A privacy first notarization service on Aztec, users register document hashes and receive immutable timestamps and optional third party attestations. Contents and identities remain confidential, selective disclosure is available when needed.

**What it solves**

- Proves existence and integrity of documents at a point in time without exposing contents.
- Reduces fraud and backdating risk, improves evidentiary posture.
- Simplifies multi party attestations and custody of sensitive material.

**Expected outcome for the client**

- Fast, low cost notarization, court friendly receipts, and controlled disclosures for partners or regulators.

---

## 2) Target Users and Needs

**Primary personas**

1. **Founder or IP Owner** wants to prove prior art or authorship without publishing drafts.
2. **Legal Counsel** needs tamper proof timestamps and optional notary co signature.
3. **Compliance Officer** needs auditable logs of policy documents and sign offs.
4. **Research or Media Teams** want sealed evidence packages for later reveal.

**Jobs to be Done**

- As an IP owner, I want to prove I had this file on a date.
- As legal, I want to attach a notary attestation without leaking contents.
- As compliance, I want to verify a policy version was in force at a time.

---

## 3) Main Use Cases

1. **Authorship and prior art** code, designs, manuscripts.
2. **Contract versioning** sealed drafts and executed versions.
3. **Evidence preservation** photos, logs, chain of custody notes.
4. **Policy control** signed policy releases with private attestations.

---

## 4) User Experience

### 4.1 Creator flow

1. **Add document** drag and drop, client computes hash locally, no upload by default.
2. **Seal** write private commitment on Aztec, optional add a co signer.
3. **Receipt** get a human readable certificate and a signed JSON receipt.
4. **Manage** group seals into collections, add labels, set retention.

### 4.2 Attestor flow

- Receive request, verify context, co sign privately, appear on receipt as authorized attestor without seeing the document unless allowed.

### 4.3 Verifier flow

- Receive a **disclosure link** with the original file and receipt, verify hash equality and timestamp, or verify only metadata if content stays sealed.

---

## 5) Product Features

**MVP**

- Local hashing, private commitment and timestamp on Aztec.
- Optional co signer flow, encrypted note addressed to both parties.
- Receipt generator, PDF and JSON, QR code for verification.
- Selective disclosure links with scope, expiry, and audit logs.
- Collections, labels, and search over user metadata, not file contents.

**Later roadmap**

- Time based releases and dead man switches, reveal if no heartbeat.
- Multi file packages with ordered chain of custody.
- Trusted time oracle redundancy, multiple attestations.
- API and webhooks for CI pipelines, DMS integrations.

**Out of scope for now**

- Raw file storage, we do not host content by default, optional encrypted storage add on later.
- Content fingerprinting or plagiarism detection.

---

## 6) Privacy Rules and Policies

- **Private by default** only hashes and encrypted notes on chain, no file contents.
- **Selective disclosure** reveal original files only to authorized verifiers, time bound and logged.
- **No backdoors** verification relies on public hash algorithms and open receipts.

---

## 7) Differentiators

- Court friendly receipts with privacy, not public hash graffiti.
- Co signer and attestation flows that do not leak contents.
- Easy verification for non crypto users, QR and web verifier.

---

## 8) Risks and Mitigations

- **Weak client hashing practices** ship desktop and browser apps with audited hashing, warn on low entropy inputs.
- **Lost files** encourage redundant off chain storage, optional encrypted vault add on.
- **Verifier confusion** simple verifier UI and step by step validation guide.

---

## 9) MVP Scope

- Up to 50,000 notarizations per org in pilot, 1 co signer role, 1 time source.
- Receipts in English, basic branding, CSV and JSON exports.
- Public verifier page that checks receipts without wallet.

---

## 10) Commercial Model and Pricing

- Per seal fee with volume tiers, example 0.50 to 2.00 USD equivalent.
- Team plan for shared org space, disclosure sessions, and co signer roles.
- Enterprise, custom retention policies, DPA, SLA.

---

## 11) Open Questions

- Which notary or attestation partners to support first.
- Jurisdiction specific language for receipts, evidentiary standards.
- Default retention and key rotation policies.

### **Existing similar projects:**

https://opentimestamps.org/

https://docs.proofofexistence.com/

https://originstamp.com/solutions/timestamp/en

https://www.docusign.com/products/notary