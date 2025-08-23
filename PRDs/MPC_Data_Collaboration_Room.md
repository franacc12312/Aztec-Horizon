# MPC Data Collaboration Room

# PRD, zk MPC Clean Room, Verifiable Multi-Party Data Collaboration on Aztec

## 1) Vision and value proposition

**What it is**: a privacy preserving collaboration room where two or more parties compute joint metrics or train small models on their private inputs, then publish a zero knowledge proof that the output is correct. No party sees raw data from others, consumers verify results in one step.

**What it solves**

- Lets partners answer cross company questions without central brokers or data sharing.
- Lowers legal and competitive risk, reduces time to signature for data partnerships.
- Creates audit ready evidence, every output is tied to a proof and a policy.

**Expected outcome**

- Faster partnerships, safe insights, verifiable outputs that stand up to audits.

---

## 2) Target users and needs

**Primary personas**

1. **Enterprises and DAOs** need shared KPIs without revealing internals.
2. **Funds, brands, and data vendors** need clean room style overlap, lift, and attribution.
3. **Healthcare, research, and public sector teams** need reproducible statistics without PII handling.
4. **Auditors and regulators** need proof bundles that a computation followed the approved policy.

**Jobs to be done**

- As a partner, I want to compute overlap or lift safely, and walk away with a receipt I can show legal.
- As a data owner, I want strong policy control, revocation, and no raw data egress.
- As an auditor, I want a verifiable package that links inputs, policy, computation code, and output.

---

## 3) Core use cases

1. **Overlap and cohort sizing**, private set intersection and sum on the intersection, for example loyalty list overlap, no list exchange.
2. **Attribution and lift**, private measurement where only incremental conversions are learned, not user level logs. 
3. **Counterparty and risk checks**, exposure ranges and thresholds across counterparties without raw positions.
4. **Supply chain and compliance analytics**, rate, defect, and provenance aggregates by tier, no supplier books shared.
5. **Research statistics**, means, quantiles, confidence intervals, and reproducible bundles for IRBs, no PII egress.

---

## 4) User experience

### 4.1 Host flow

1. **Create a room** choose a template, set purpose, retention, k anonymity, and who can join.
2. **Invite participants** each party connects a source and runs a local pre check.
3. **Policy approval** legal sees a one page summary, inputs, outputs, allowed queries, and expiry.
4. **Run session** host clicks run, parties approve, proof and outputs are generated.
5. **Distribute** partners download results, the verifier link, and an audit receipt.

### 4.2 Participant flow

- Connect a data source or upload encrypted shard locally, review policy, approve, monitor progress, receive receipt, withdraw consent at any time.

### 4.3 Verifier and auditor flow

- Open a public verifier link, check the proof, the template hash, and the policy digest, request a time bound disclosure pack if required.

---

## 5) Product features

**MVP**

- **Templates** set intersection, private join and compute, sums, averages, ratios, and lift, with parameterized k anonymity and minimum counts. [MPC Deployments](https://mpc.cs.berkeley.edu/posts/Private-Join-and-Compute/?utm_source=chatgpt.com)
- **Session orchestration** invites, consent capture, policy snapshot, immutable logs, and short lived proof artifacts.
- **Proof bundles** machine readable JSON receipts plus a public verifier URL for third parties.
- **Policy engine** output caps, aggregation only, no row level exports, retention timers, revocation.
- **Connectors** CSV, S3, Postgres, and a simple SDK for custom loaders.
- **Governance** role based access, dual approvals for risky templates, and red flag checks.

**Later**

- **Model training on aggregates** simple GLMs and tree based models on features that pass k and DP checks.
- **Differential privacy add on** noise budgets and per column privacy parameters for public sharing.
- **PSI acceleration** optional PSI implementations and hardware backed options where available. [Apple](https://www.apple.com/child-safety/pdf/Apple_PSI_System_Security_Protocol_and_Analysis.pdf?utm_source=chatgpt.com)
- **Data residency and localization** region pinned rooms and deletion proofs.

**Not in scope now**

- Hosting raw PII on chain, long running ML training with raw features, general purpose data warehousing.

---

## 6) Privacy and disclosure policy

- **Private by design** inputs never leave participant control, rooms produce only aggregates and a zk proof.
- **Selective disclosure** case based, limited to policy, code hash, and aggregate outputs, optional regulator pack with expiry.
- **Anti linkage** batch windows, k thresholds, and suppression of small cells, plus optional DP noise for public use.
- **Right to revoke** any participant can revoke before execution, and may request deletion of artifacts after expiry.

---

## 7) Differentiators

- **Verifiable analytics, not trusted analytics**, every number ships with a proof.
- **Template first UX** lowers legal review time, gives predictable privacy guarantees.
- **Aztec native settlement** private payments for sessions and bounties, optional selective disclosure for invoices.

---

## 8) Risks and mitigations

- **Small cohort leakage** enforce k thresholds, suppress small cells, and DP noise where required.
- **Collusion or reconstruction** require N of M participants for sensitive templates, randomized splits, independent audits.
- **Data poisoning** template validations, monotonicity checks, and optional stake with slash.
- **Regulatory acceptance** provide standard proof bundles and mappings to GDPR, HIPAA, CCPA concepts.

---

## 9) MVP scope

- Three templates, PSI based overlap and sum on intersection, aggregate stats, and binary lift.
- Up to five parties per session, one country region, 1,000 sessions per month.
- One wrapped stablecoin on Aztec for billing and revenue share.

---

## 10) Pricing and commercial

- **Per session fee** by template and data size.
- **Enterprise subscription** seats, SLAs, and private regions.
- **Marketplace** revenue share for third party templates and certified connectors.

---

## 11) Open questions

- Which verticals to seed first, ads and retail, healthcare, finance.
- Default k and DP settings by template and jurisdiction.
- Third party certification for templates that claim specific compliance properties.

---

## 12) Benchmarks and inspiration

**Web2 clean rooms**

- **Google Ads Data Hub**, privacy centric warehouse for ad measurement, aggregate only, strict query controls. [Google for Developers](https://developers.google.com/ads-data-hub?utm_source=chatgpt.com)
- **Snowflake Data Clean Rooms**, native multi party collaboration with privacy preserving configurations. [docs.snowflake.com](https://docs.snowflake.com/en/user-guide/cleanrooms/introduction?utm_source=chatgpt.com)[snowflake.com](https://www.snowflake.com/en/fundamentals/what-is-a-data-clean-room/?utm_source=chatgpt.com)
- **AWS Clean Rooms**, “analyze and collaborate without sharing or copying underlying data”, overlap demos are standard. [Amazon Web Services, Inc.+1](https://aws.amazon.com/clean-rooms/?utm_source=chatgpt.com)
- **InfoSum**, “zero data sharing”, aggregate by design, limits on granularity and query complexity. [infosum.com+1](https://www.infosum.com/products/secure-data-clean-room?utm_source=chatgpt.com)
- **LiveRamp Safe Haven**, clean room for marketers, cross walled garden measurement. [LiveRamp](https://liveramp.com/our-platform/clean-rooms/?utm_source=chatgpt.com)[LiveRamp](https://liveramp.uk/safe-haven-data-partnerships/?utm_source=chatgpt.com)
- **Meta Private Lift**, MPC based incremental lift without exposing consumer level data, a strong precedent for our lift template. [MPC Deployments](https://mpc.cs.berkeley.edu/posts/Private-Lift-Measurement-for-Private-Advertising/?utm_source=chatgpt.com)[Facebook](https://www.facebook.com/business/marketing-partners/business-innovation-technology-podcast/Attribution-and-Private-Lift?utm_source=chatgpt.com)
- **Google Private Join and Compute**, PSI plus homomorphic encryption for “sum on intersection”, our overlap and aggregate template mirrors this. [Google Online Security Blog](https://security.googleblog.com/2019/06/helping-organizations-do-more-without-collecting-more-data.html?utm_source=chatgpt.com)[MPC Deployments](https://mpc.cs.berkeley.edu/posts/Private-Join-and-Compute/?utm_source=chatgpt.com)
- **Apple PSI and DP**, production grade PSI designs and public differential privacy approach for telemetry. [Apple](https://www.apple.com/child-safety/pdf/Apple_PSI_System_Security_Protocol_and_Analysis.pdf?utm_source=chatgpt.com)[WIRED](https://www.wired.com/2016/06/apples-differential-privacy-collecting-data?utm_source=chatgpt.com)

**Web3 privacy compute**

- **Ocean Protocol Compute to Data**, run approved algorithms where the data lives, no raw data egress, very aligned with our room model. [Ocean Protocol](https://oceanprotocol.com/learn/compute-to-data?utm_source=chatgpt.com)[docs.oceanprotocol.com](https://docs.oceanprotocol.com/developers/compute-to-data?utm_source=chatgpt.com)
- **Oasis Labs Parcel**, privacy first governance and isolated compute, examples of policy and access logs we can emulate. [docs.oasislabs.com](https://docs.oasislabs.com/parcel/latest/?utm_source=chatgpt.com)[oasis.net](https://oasis.net/blog/partners-and-new-use-cases-help-fuel-rapid-growth-of-the-oasis-parcel-ecosystem?utm_source=chatgpt.com)
- **Secret Network**, confidential smart contracts with TEEs, a reference for enclave based variants when ZK alone is not enough. [docs.scrt.network+1](https://docs.scrt.network/secret-network-documentation/introduction/secret-network-techstack/privacy-technology/private-computation-and-consensus-flow?utm_source=chatgpt.com)
- **Partisia Blockchain**, MPC smart contracts with private state alongside public state, a close analogue to our hybrid approach. [GitLab](https://partisiablockchain.gitlab.io/documentation/smart-contracts/zk-smart-contracts/zk-smart-contracts.html?utm_source=chatgpt.com)[Partisia Blockchain](https://partisiablockchain.com/?utm_source=chatgpt.com)
- **Nillion**, nil message compute, non interactive MPC for some non linear ops, interesting for future acceleration. [nillion](https://nillion.com/news/introducing-the-nillion-non-interactive-mpc-protocol-for-non-linear-computations/?utm_source=chatgpt.com)[DAIC Capital](https://daic.capital/blog/nillion-network-private-compute?utm_source=chatgpt.com)