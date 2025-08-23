# ZKMembership and Eligibility Gate

## 1) Vision and value proposition

**What it is**: a reusable proof of membership and eligibility layer for any Aztec app. Users prove they belong to a group or satisfy a policy, the app only learns pass or fail, never the user’s identity. Eligibility can be time bound, jurisdiction bound, reputation bound, or bundle multiple claims.

**What it solves**

- Private allowlists and ticketing without public rosters or wallet graph leaks.
- Real anti Sybil and anti bot gating that respects anonymity.
- One credential, many verifications, less friction and higher conversion.

**Expected outcome**

- Higher quality users, lower abuse, smoother onboarding with one click proofs.

---

## 2) Target users and needs

**Primary personas**

1. **Consumer apps and DAOs** want gates, allowlists, and perks without doxxing members.
2. **Marketplaces and mints** want bot resistant allowlists and jurisdiction or age checks.
3. **Compliance teams** want scoped proofs, audit trails, and revocation.
4. **Credential issuers** universities, employers, communities want a simple way to issue, rotate, and revoke group credentials.

**Jobs to be done**

- As a dApp, check eligibility privately with a single widget and an API.
- As a user, prove I qualify without exposing my wallet history.
- As an issuer, manage groups, expirations, and revocations with minimum ops.
- As compliance, answer a lawful request with a minimal proof package.

---

## 3) Core use cases

1. **Private allowlists and tickets**, set membership proofs for mints, beta access, events.
2. **Jurisdiction or age gates**, prove country or 18 plus without revealing date of birth.
3. **Reputation thresholds**, show rep above a level, do not reveal the exact score.
4. **Perk federation**, one credential unlocks discounts or features across partner apps.
5. **Sensitive features unlock**, claims like KYC passed, accredited investor, employee of X, without raw documents.

---

## 4) User experience

### Issuer flow

1. Create a group, upload members by list or rule, publish a Merkle root, define policy, expiry, and disclosure preset.
2. Distribute claim links or QR codes, rotate root on schedule, revoke as needed.
3. View aggregate usage, no per user logs by default.

### User flow

1. Link wallet or account, receive a private claim, store it locally or in a privacy preserving vault.
2. Click Verify in any partner app, the widget returns pass or fail and a short lived token.
3. Optional, request a one time selective disclosure pack for a specific counterparty.

### Partner app flow

1. Add the widget, configure accepted issuers and policies, set caching rules.
2. Receive pass or fail and a signed token, proceed with gated action, never store PII.

### Auditor flow

- Request a scoped pack, see issuer identity, policy hash, time window, and a proof that a valid claim satisfied the policy, identities remain hidden unless the user opts in.

---

## 5) Product features

**MVP**

- Group registry with Merkle roots, expirations, rotations, and revocation lists.
- One click proof widget and REST or JS API, pass or fail receipts with reason codes.
- Policy builder for simple gates, membership, age range, jurisdiction allow or deny, issuer allowlist.
- Freshness checks, nonce binding, replay protection, short lived verification tokens.
- Activity analytics, aggregate only, count of passes and fails, no identities.

**Later**

- Nested groups and AND or OR policies, for example member of X and not on deny list Y.
- Reputation thresholds and range proofs, for example rep greater than 100.
- Multi issuer federation and trust frameworks, for example EDU, employer, DAO issuer classes.
- zk email or zk document adapters, for example prove email domain or license attribute without reveal.
- Mobile SDK, WalletConnect plug in, server side verifier library.

**Not in scope now**

- Hosting user PII or raw KYC documents, manual document review.

---

## 6) Privacy and disclosure policy

- Private by default, proofs reveal only that a claim satisfying the policy exists.
- Selective disclosure only with explicit user consent, time bound, dual approval, full audit log.
- Anti correlation, randomize proof timing where helpful, do not expose issuer user identifiers to relying parties.
- Data minimization, store policy hashes and aggregate counters only.

---

## 7) Differentiators

- True privacy preserving eligibility, not a centralized “trust me” gate.
- Federation friendly, multiple issuers and policies with a single widget.
- Works across Aztec apps out of the box, portable and cacheable pass tokens.

---

## 8) Risks and mitigations

- **Garbage in at issuance**, require audited issuers, reputation for issuers, and configurable trust lists.
- **Replay or token theft**, nonce binding, expirations, origin checks, and device binding when available.
- **Linkability across apps**, per app tokens and optional anonymized relays, encourage one address per app.
- **Regulatory demands**, predefined disclosure templates, redaction by field, and expiry.

---

## 9) Success metrics

- Pass conversion rate, proof latency, proof failure reasons, issuer rotation frequency, abuse rates on gated features, bot pass rate.

---

## 10) MVP scope

- One issuer type and three policies, membership, country allowlist, 18 plus.
- 100 partner apps in pilot, 100k monthly verifications.
- One recommended wallet and a JS widget, public verifier for pass tokens.

---

## 11) Pricing and commercial

- Per verification fee, first N free per month.
- Issuer subscription for group management, rotations, and analytics.
- Enterprise plan, custom policies, SLAs, and dedicated support.

---

## 12) Open questions

- Default proof lifetime and cache rules, one minute, five minutes, longer.
- Governance of issuer allowlists, community lists, enterprise private lists, or both.
- Preferred disclosure artifacts for regulators by country.

---

## 13) Benchmarks and inspiration

**Web3**

- **Sismo** and ZK badges, selective disclosure from off chain identity to on chain actions.
- **Semaphore** and membership proofs, nullifiers to prevent double actions.
- **Gitcoin Passport** and anti Sybil credentials, combine stamps into a score, use range proofs on top.
- **Polygon ID** and **Verite**, verifiable credentials with ZK predicates.
- **World ID** and Proof of Humanity, inspiration for unique human claims, adapt with selective disclosure.

**Web2**

- **Auth0 or Okta** for issuer dashboards, policy builders, and rotation flows.
- **Persona or Onfido** for KYC flows to feed issuers, do not host their raw docs, only accept attestations.
- **Apple Sign In** philosophy, minimal data sharing, relay email as a pattern for privacy preserving federation.

---