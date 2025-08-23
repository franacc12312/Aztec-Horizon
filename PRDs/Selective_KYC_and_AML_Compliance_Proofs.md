## 1) Vision and Value Proposition

**What it is**

A privacy preserving compliance layer for Aztec. Users prove they meet specific KYC or AML policies, for example verified identity, jurisdiction allowlist, sanctions screen, age threshold, transaction size band, without revealing personal data or linking wallets. Dapps consume yes or no proofs and optional scoped attributes, with selective disclosure for regulators.

**What it solves**

- Removes the false tradeoff between privacy and compliance, users keep PII off chain while protocols enforce rules.
- Reduces onboarding friction for institutions and regulated users who need policy gates.
- Minimizes data liability for protocols, no centralized store of KYC data, only proofs and revocation signals.

**Expected outcome for the client**

- Higher conversion on onboarding, regulator friendly operations with targeted evidence, simple SDK integration for private dapps on Aztec.

---

## 2) Target Users and Needs

**Primary personas**

1. **Protocol Operator** wants to enforce policy gates without storing PII or doxxing users.
2. **Compliance Officer** needs audit ready evidence that rules were applied, and scoped disclosures on request.
3. **End User** wants to access products privately, prove eligibility once, reuse credentials across apps.
4. **KYC Issuer or Partner** needs a safe way to issue and revoke credentials, with usage reporting that does not expose users.
5. **Auditor or Regulator** expects targeted disclosures, not full user databases.

**Jobs to be Done**

- As a protocol, I want to check that a user has a valid KYC credential before letting them interact.
- As compliance, I want to provide a regulator a minimal proof that a given transaction met policy.
- As a user, I want to pass checks privately and reuse my credential in multiple apps.

---

## 3) Main Use Cases

1. **Private dapp onboarding** prove possession of a valid KYC credential from an approved issuer.
2. **Jurisdiction gating** prove country is in an allowlist, or not in a blocklist, without revealing which one.
3. **Sanctions and PEP screening** prove negative screen as of a date, with revocation if status changes.
4. **Age verification** prove age over a threshold without revealing birthdate.
5. **High value transaction control** prove transaction amount is below a reporting band, or that enhanced checks were performed.

---

## 4) User Experience

### 4.1 Integrator flow, protocol

1. **Configure policy** choose rules, accepted issuers, validity windows, revocation behavior.
2. **Install SDK** add a single check to protected entry points, receive pass or fail with a short policy receipt.
3. **Monitor** view aggregate pass rates and revocation events, no user level PII.

### 4.2 User flow

1. **Obtain credential** complete KYC off chain with an issuer, receive a private credential bound to an Aztec identity.
2. **Prove** when using a dapp, generate a zero knowledge proof that satisfies the policy, wallet signs a private transaction.
3. **Reuse** keep using the credential across apps until expiry or revocation.

### 4.3 Compliance or auditor flow

- **Selective disclosure** request a scoped proof or a one time view of a credential attribute, dual approval, time bound link, full audit log.

---

## 5) Product Features

**MVP**

- Policy engine with common checks, KYC present, jurisdiction allowlist or blocklist, sanctions negative screen, age over threshold, amount band proofs.
- Issuer integrations, one or two providers at launch, credential issuance, expiry, and revocation feeds.
- Client side proof generation in wallet, serverless, no PII leaves the user or issuer.
- Smart contract verifier for Aztec, accept or reject based on proof and issuer registry.
- Selective disclosure sessions for regulators, scoped attributes only, dual approval and audit trail.
- Admin console, policy configuration, issuer registry, aggregate metrics.

**Later roadmap**

- Travel rule connectors and VASP attestations with minimal data exchange.
- Source of funds and enhanced due diligence attestations via partners.
- Multi chain verifier adapters and bridge checks.
- Mobile SDK and custodial flow for enterprise wallets.

**Out of scope for now**

- Performing KYC in house, the MVP relies on external issuers.
- Storing raw documents or PII in our systems.

---

## 6) Privacy Rules and Policies

- **Private by default** no PII on chain, only proofs and revocation signals.
- **Selective disclosure** scoped attributes on request, time bound, dual approval, logged.
- **Revocation first** real time revocation supported, proofs must include freshness.
- **No linkability** credentials are bound to an Aztec identity, apps receive pass or fail without cross app identifiers.

---

## 7) Differentiators

- Compliance grade controls without centralizing PII.
- Developer friendly, single check integration, reusable user credentials.
- Regulator friendly, targeted evidence on demand.

---

## 8) Risks and Mitigations

- **Regulatory acceptance** engage counsel and early regulator sandboxes, ship clear whitepapers and sample disclosures.
- **Issuer compromise** multiple issuers per policy, rapid revocation and grace policies.
- **User UX confusion** guided wallet flows, plain language copy, pre flight checks.
- **Proof replay** include nonce and expiry in proofs, enforce anti replay in contracts.

---

## 9) MVP Scope

- Two supported issuers, three policy types, up to 100k proofs per month across integrators.
- One verifier contract template, one admin console, one disclosure role.

---

## 10) Commercial Model and Pricing

- SaaS per integrator, tiered by monthly verified users, plus per proof fee above tier.
- Enterprise plan with SLAs, custom issuer integrations, and audit support.
- Referral revenue share with issuers.

---

## 11) Open Questions

- Which jurisdictions and issuers to prioritize at launch.
- Default freshness windows for sanctions proofs.
- Minimal attribute set in regulator disclosures.
- How to handle credential portability across identities if a user rotates keys.

### **Existing similar projects:**

https://zkpassport.id/

https://sismo.mirror.xyz/MimvqFv45hohMwDBD9rGqY4XGZIHRR8On7nx6q9YFRc

https://polygon.technology/blog/introducing-polygon-id-zero-knowledge-own-your-identity-for-web3

https://quadrata.com/

https://www.gemini.com/es-LA/cryptopedia/civic-identity-cvc-crypto-civic-crypto-cvc-token

https://decentralized-id.com/

https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4563364