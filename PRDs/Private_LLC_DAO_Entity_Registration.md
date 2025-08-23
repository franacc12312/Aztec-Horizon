## 1) Vision and Value Proposition

**What it is**:

A platform that enables individuals, teams, and DAOs to register and manage legal entities (LLCs or equivalents) privately onchain using Aztec. It supports the full lifecycle of entity creation, member updates, governance setup, and legal document custody, with selective disclosure capabilities.

**What it solves**

- Reduces the friction and exposure involved in forming legal wrappers for DAOs or projects.
- Provides compliant and auditable structures without broadcasting entity information on public blockchains.
- Enables legal and operational coordination while preserving anonymity when needed.
- Prevents the need to choose between privacy and compliance.

**Expected outcome for the client**

- Seamless creation and management of legal entities from a DAO dashboard, with private records, roles, and limited disclosures when required.

---

## 2) Target Users and Needs

**Primary personas**

1. **DAO Core Contributor**: Wants to create a compliant wrapper with minimal friction and pseudonymity protection.
2. **Project Founder**: Seeks to legally register their venture without exposing sensitive identities or token holdings.
3. **Operations Lead**: Needs to manage entity roles, governance, and ownership updates with privacy and traceability.
4. **Legal Counsel**: Requires access to certain records for compliance, fundraising, or M&A, with audit logs and approval trails.
5. **Auditor or Regulator (optional)**: Expects access to a verifiable but scoped view of legal state, enabled via disclosure.

**Jobs to be Done**

- “As a DAO, I want to register an LLC without revealing every contributor’s identity publicly.”
- “As a founder, I want to prove I own a legal entity tied to my project without linking wallets to public records.”
- “As operations, I want to update members or documents securely and traceably.”
- “As legal, I want to respond to requests from regulators without over-disclosing internal data.”

---

## 3) Main Use Cases

1. **LLC Formation**: Create a legal wrapper from the platform, assign ownership shares privately, sign documents offchain or onchain with zk proofs.
2. **Entity Management**: Update members, change governance rules, manage cap tables, all through a private UI with commitment history.
3. **Document Storage and Disclosure**: Upload/share signed operating agreements or contracts privately, with selective disclosure.
4. **Delegation and Control**: Allow representatives or multisigs to act on behalf of the entity via attestations or zk credentials.
5. **Compliance Requests**: Respond to KYC/AML, investor onboarding, or legal inquiries with privacy-preserving disclosures.

---

## 4) User Experience

### 4.1 Formation Flow

1. **Create Entity**: Choose jurisdiction (e.g., WY, BVI), name, and legal form (LLC, DAO LLC, Cooperative).
2. **Assign Members**: Define wallet-controlled roles (e.g., founder, signer, contributor) with encrypted metadata.
3. **Document Signing**: Upload or generate operating agreement templates, signed with zk proofs of membership and timestamps.
4. **Private Vault Setup**: Securely store docs, cap table, governance config.

### 4.2 Management Flow

1. **Dashboard View**: See current members, governance status, voting rights, and encrypted documents.
2. **Update Flow**: Add/remove members, update docs, transfer ownership shares privately.
3. **Disclose Flow**: Initiate a selective disclosure session for regulators or partners, with expiration and approval logging.

---

## 5) Product Features

**MVP**

- Private entity creation and metadata registry (jurisdiction, name, form).
- Member assignment via wallet and private identity commitment.
- Document upload and hash notarization with private access controls.
- Selective disclosure session generator (link with scoped data).
- Cap table and role management with zk proof-backed updates.

**Later roadmap**

- Embedded formation API with registered agents or legal firms.
- zk-based credentials for legal agents or reps.
- Multichain integrations for token ownership or cap table sync.
- Exportable legal bundles for banking, KYC, or fundraising.
- Jurisdiction templates with localized compliance flows.

**Out of scope for now**

- Automatic fiat banking integrations.
- Full legal opinion generation or legal support (requires partnerships).

---

## 6) Privacy Rules and Policies

- **Default private entity metadata**, no public cap tables or ownership disclosures.
- **Proof-of-role** zk attestations for delegation or signing without wallet exposure.
- **Audit trail for disclosures**, showing who accessed what, when, and why.
- **Document encryption at rest**, with recipient-only decryption on disclosure.
- **Retention**: Entities can request deletion or offboarding based on jurisdictional rules.

---

## 7) Differentiators

- **Private-by-design legal formation**, with selective compliance when needed.
- **DAO-native governance integration**, not just wrapper formation.
- **Offchain + onchain sync**, allowing hybrid legal coordination.
- **Role-based zk credentials**, enabling anonymous operational delegation.

---

## 8) Risks and Mitigations

- **Jurisdictional mismatch**: Partner with legal nodes per region, offer disclaimers and human-in-the-loop when needed.
- **Over-complex UX**: Start simple with templates, prioritize clarity over full customization.
- **Abuse potential (bad actors)**: KYC-compatible disclosure hooks, denylisting options.

---

## 9) MVP Scope

- 3 supported jurisdictions: Wyoming (LLC), Panama, Marshall Islands (DAO LLC).
- Up to 10 members per entity, max 5 roles per org.
- Document storage via IPFS+encryption, and zk-notarized change history.
- Selective disclosure via 1-click link with scoping (jurisdiction, document, member list).

---

## 10) Commercial Model and Pricing

- **Basic**: Free entity creation and self-managed dashboard (limited docs/members).
- **Pro**: Paid plan with additional storage, disclosure sessions, and governance flows.
- **Legal Partner API**: Monthly fee + usage-based pricing for law firms or DAO ops providers.

---

## 11) Open Questions

- Which jurisdictions are legally compatible with zk entity registration?
- Should we enable notarized agreements directly in-app, or integrate existing providers?
- What’s the optimal UX for managing zk-based ownership shares and disclosures?

### **Existing similar projects:**

https://www.aragon.org/how-to/choose-a-legal-wrapper-for-your-dao

https://syndicate.mirror.xyz/4p6a0nKpBYMSxoAfN6KpjcUwJSD2t68Dq7zgoliB4pk

https://www.doola.com/

https://otoco.io/