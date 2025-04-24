# Post #1 by Yush
Posted at: 2025-03-30T16:30:55.068Z

# ENS SPP2: Decentralized Zero Knowledge Verification of Social Profiles with ZK Email

## 1. Applicant Information

* Team Name: ZK Email
* Website/Company Blog: <https://zk.email>
* Entity ENS: zk-email.eth (to register)
* Primary Contact(s):
  + Yush, 0xyush.eth
  + Rute, rutefig.eth
  + Paradox, bisht13.eth
* Company Overview: We are a public goods organization that works to privately verify email data on-chain in a maximally decentralized way, bridging web2 and web3 identities. We provide more details below in the Vision section!
* Requested Amount:
  + Extended budget of $800K / year; or
  + Basic budget of $400k / year
* Team / Commitment: Currently 8 FT resources. We are committing to making the work outlined in this proposal a top priority for the duration of the agreement, and we have edited our own internal roadmaps to ensure that ENS is a priority.

## 2. Eligibility Confirmation

* Company Age & Reputation: We confirm our organization is over 1 year old as evidenced by our Github history on [github.com/zkemail](http://github.com/zkemail).
* Prior Experience: Our team has extensive experience in blockchain technology, specifically in zero-knowledge proofs and identity attestation systems, as demonstrated by our mainnet deployments and prominence in the ZK space.
* ENS Endorsement: We expect to get the required 50k ENS endorsement through [Snapshot](https://snapshot.box/#/s:nominations.ens.eth/proposal/0xa364c79944671e51185da6c4170e632f4ead933e03629fd258b87d88298bd761)!
* OFAC Compliance: We, ZK EMAIL, confirm that neither our organization nor any of our employees, contractors, or executive leadership is located in, or a resident of, an OFAC-sanctioned country. We further confirm that none of our business resources are derived from or routed through any country or entity that is subject to sanctions imposed by the United States (OFAC) or equivalent regulatory bodies. We pledge to remain compliant with all applicable sanctions laws and will promptly notify the ENS DAO if our status changes.

## 3. Open Source Commitment

All of our code is MIT licensed and open source, and all work completed under the scope below will meet the same criteria. You can find our full codebase and ongoing work at [github.com/zkemail](https://github.com/zkemail).

## 4. Vision

ENS currently only has one two way record – the primary identity. We believe ZK Email can extend this model by enabling two-way records for every Web2 identity—email accounts, social media profiles, credentials, and more—directly on ENS.

By verifying tamper-proof digital signatures embedded in emails, ZK Email allows users to prove statements from Web2 services on-chain. This includes confirming social media handles, event participation, KYC results, and other credentials—without revealing private data. With ZK Email, a user’s on-chain identity can reflect more than just blockchain transactions; it can also include verifiable real-world actions.

Our integration creates a cryptographically sound bridge between Web2 identity (emails, social platforms, verification systems) and ENS, the core of Web3 identity. This unlocks new use cases across the ecosystem—enabling large apps to run sybil-resistant airdrops, and smaller apps to access rich, privacy-preserving identity context that was previously unavailable.

In a post-AI world, where trust in digital content is eroding, cryptographic signatures—whether from private keys or authenticated emails—are one of the few remaining proofs that cannot be faked. We believe bringing Web2 digital signatures into ENS via ZK Email can establish a new foundation for trust in personal identity and naming across Web3.

## Why is ZK Email the Right Team to Build This

ZK Email is a team of 7–8 researchers and engineers focused on building cryptographic infrastructure that bridges Web2 data with Web3 functionality. Our team brings experience from MIT, Microsoft, NVIDIA, ZKSync, 0xPARC, and the Ethereum Foundation’s Privacy & Scaling Explorations (PSE) group. We specialize in applied cryptography, EIP development, infrastructure engineering, and protocol design.

Our mission is to extend the privacy-preserving capabilities of crypto to broader audiences—not just existing Web3 users—through cryptographically sound, production-ready tools. Until early 2025, we were funded by PSE, which concluded its support as part of a strategic shift toward earlier-stage research (e.g., iO and MPC tooling). PSE has cited ZK Email as one of its most successful initiatives to date.

Over the past two years, ZK Email has become a recognized contributor in the ZK ecosystem, known for our dual focus on open-source research and shipping usable products. Our work has been integrated into a range of other ZK-based projects, including OpenPassport (now Self), Anon Aadhar, and ZKP2P.

We know that we are a new player to the ENS DAO – we only just realized the incredible overlap between our social name proofs and ENS’s mission a few weeks ago. We are committed to delivering a ton of long-term value for ENS: [one goal of the ENS service provider streams](https://snapshot.box/#/s:ens.eth/proposal/0x5748982aed143f51333befbc6cc490116648b85a2b0212fdfaf3ab848932c7ae) was to “[explore] untapped platforms or entirely new applications for ENS”, and we intend to enable exactly that by making social media usernames possible to resolve on-chain with ENS.

## Why is ZK Email the right technology for this

ZK Email enables users to prove specific attributes from emails—such as “I own an email at this domain,” “I made a Venmo transaction of this amount to this person,” or “I received a Twitter email confirming my username is @\_\_\_”—without revealing the rest of the email content.

It leverages DKIM (DomainKeys Identified Mail), a signature attached to every sent email that proves the contents are authentic. By verifying the DKIM signature inside a zero-knowledge proof (ZKP), users can selectively disclose verified information (e.g., their Twitter username) while keeping sensitive details like their email address or real name private.

To support this, we built a zk-regex compiler parsing email content with zero knowledge. The DKIM public key used for verification is stored in the sender’s DNS records, and we mirror these records on-chain in a verifiable way that any third party can audit.

This approach also supports private, on-chain verification of social logins (e.g., proving a Google sign-in). For a deeper technical dive—including why ZK Email is spoof-proof and how it achieves trustless, decentralized identity verification—see our [detailed blog post](https://zk.email/blog/zkemail).

## 4.5. Proposed Scope of Work

### Basic Scope: Social Username Resolution in ENS

1. ENS Resolver Integration: Develop ZK email verification for ENS names that allows users to prove ownership of email accounts + (optionally) avoid revealing the entire address, perhaps opting to reveal only the domain if desired
2. Social Account Verification: Implement ZK proofs to verify ownership of social media accounts (Twitter, GitHub, etc) linked to ENS names
3. Resolver Contract Development: Create resolver contracts that map ENS names to zk verified identity records
4. SDK Development: Build developer-friendly SDKs that enable easy integration of these verification methods, along with on-chain verification, and a simple UI to do so (and native integration with ENS or an alternate frontend if they are interested).

We hope that an MVP of 1, 2, and 3 can be developed after 3 months – this will cover time to develop the resolvers, integrate it into the UI, and make client-side proving fast enough for users. We suspect resolver integration will take ~1 month, testing will take ~1 month, and fast client side proving will take the full 3 months and can be done in parallel. Once we’ve solicited community feedback, we expect the SDK + testing to take another month, and final audits to take 2 months. We then believe 6 months will be needed for debugging edge cases, making proofs faster, supporting more devices, (and building the expanded scope if that’s approved). In total, the full scope is one year.

Proposed Amount: $400K

### Expanded Scope

1. Directly being able to pay social media accounts on ENS: You can pay accounts that *havent signed up yet* and let them claim that money once they claim. We think this can drive significant adoption of ENS to new users who want to use ENS for things like RetroPGF or even just tipping/payments on those platforms.
2. KYC Verifications on Resolvers: Allow resolvers to link to KYCs that users have done on other platforms and register verification of uniqueness.
3. Gas Optimization: If gas is a bottleneck (which it will likely be on L1), recursive proofs can decrease proof overhead in both execution and calldata, by combining many proofs into one. We can do this via adding recursive aggregation with i.e. Nebra, and using World’s optimized on-chain verifiers.
4. Faster User Experience: Optimize proof generation for faster client-side verification times with production-ready Noir implementations, 5-10x speeding up proof calculations on a user’s device from 5 minutes to 1 minute. Client side proofs would mean information never has to leave a user’s device.
5. DNSSEC Verification: If we finish all of the above, we can also build a ZK verifier for DNSSEC calculations that reduces gas cost on mainnet from 1-2M with ENS’s verifier, to ~250K with a single proof.
6. Making DAO Voting with Safes Easier: We know that [one of Agora’s goals](https://discuss.ens.domains/t/spp2-agora-application/20443) as posited by delegates was to make it easier for Safe Wallets to vote on proposals. Our [ability to let email addresses approve Safe transactions](https://zk.email/blog/2fa) can let anyone approve any proposal with a single email reply.
7. Increasing Decentralization: We want to work on an AVS to double check the DNS keys that let us verify email public keys, allow anyone to contribute to trusted setups for all the circuits if needed, IPFS backups of our frontend + ENS resolvers for that, backups of all of our code/zkeys onto IPFS and similar sources, and contract upgrades in a more decentralized fashion. We want to ensure ENS’s system is fully secure even if ZK Email teammates are compromised.
8. Audits: If this starts securing economic value, we would want to complete an audit of the relevant code.

We expect the AVS to take a month to build and test, gas optimization to take a month to build and test, and DNSSEC verification to take 2 months to build and test even with a ZKVM on the server side (including tooling around fetching upgrades and nonstandard CAs). An audit will take 2 months or so. If this extended scope is approved, the full scope of work including the basic scope will take 1 year. While we have proposed 8 things here, we would discuss with the DAO which ones are the top priorities and focus on those, likely ending up shipping only 6.

Proposed Amount: $800K

## 5. Past Achievements and Relevant Track Record

ZK Email has demonstrated a strong track record in the ZK and identity space with consistent delivery against our roadmap:

* 2023: Successfully released V1 ZK email SDKs and launched an MVP email wallet at Zuzalu, followed by V1 ZK email wallet deployment on mainnet for Devconnect Istanbul.
* 2024: Deployed [account recovery to mainnet with Safe](https://zk.email/blog/recovery) and [Clave](https://blog2.getclave.io/clave-unveils-the-new-zk-email-recovery-beta/), [built](http://zk.email/blog/archive) the largest DKIM key archive on Earth, [released 2FA](http://zk.email/blog/2fa) for Gnosis Safe email signers, and completed multiple successful [audits](http://zk.email/blog/audits).
* Q1 2025: Implemented a [registry](https://registry.zk.email) that lets you define new kinds of proofs (i.e. X username, Netflix subscription) in 5 minutes with scalable architecture, and deploy the registry into production with Jupiter, supporting over 5000 proofs in 2 weeks with a Kubernetes GPU autoscaled prover system.

Beyond basic email verification, we’ve built an extensive ecosystem of proofs at [registry.zk.email](http://registry.zk.email) with over 100 different types of proofs, including:

* KYC Verification: Enabling users to KYC once anywhere (e.g., on Airbnb) and reuse those credentials on-chain
* Domain Ownership: Verifying domain ownership/transfers through Namecheap emails (used by zkp2p to build a marketplace already)
* Professional Affiliations: Proving employment at specific companies by verifying email domains without revealing actual addresses
* Event Attendance: Confirming attendance at events like Luma through email verification

We are confident that we can take on this major scope expansion for ENS, and execute well.

## Strategic Alignment with ENS

This proposal aligns well with ENS’s mission of creating a more accessible and usable web3 identity system:

1. Expanded Utility: ZK email verification adds decentralized, verified web2 credentials with identity verification to ENS names + resolvers, without compromising privacy
2. Increased Adoption by Non-Crypto Users: Email is universally understood and the UX is 2-3 simple clicks, making this an ideal feature for non-crypto native users. You can test this flow yourself on [registry.zk.email](http://registry.zk.email)!
3. Enhanced Security: The permissionless verification system reduces the risk of web2 identity fraud within the ENS ecosystem, and has no notaries or proxies as points of centralization like a ZKTLS solution would.
4. Decentralized Infrastructure: The proof generation and verification can be done by anyone, including client-side, with no reliance on ZK Email.

## Measurable KPIs

### Basic Scope KPIs

1. Successfully deploy ZK email verification resolver on Namechain by launch
2. Onboard at least 5,000 ENS users to verify credentials via ZK email within the first 6 months
3. Reduce proof generation time to under 1 minute on average
4. Achieve 95%+ success rate for verification attempts (our current failure rate is ~1% and we will target that, but we want to keep a buffer for issues with client side proving, RAM, protonmail, load, or odd mail providers).

### Extended Scope KPIs

1. Reduce gas costs for verification by 80%+, through proof aggregation
2. Onboard at least 1 partner or protocol to use the verification system

## Budget Request

Based on our expected team size of nine members, the amount needed to fund this team and this work on the extended scope amounts to a request of $800,000/year, which falls within the eligible range ($300K - $1.3M). If only the basic scope is covered, we would request $400,000/year.

| Category | % Allo | Description |
| --- | --- | --- |
| Salary / Headcount | 75% | Frontend, design, infrastructure, zk engineers (x2), Solidity engineers (x2), DevRel. We need a wide range of roles as the proposal will require everything from zk research to end-user product development. |
| Cloud Costs | 10% | GCP (Kubernetes, storage, databases), Modal (on-demand GPU), [Render.com](http://Render.com) (hosting). |
| Service Providers | 10% | Slack, Google OAuth audits, Google Workspace, Xero (expenses), Claude API, Cursor Pro (dev tooling), misc. |
| Growth / Travel | 5% | Conference presence at ZK Summit, ETHCC, Protocol Berg, Chaos Computer Conference, and DEFCON to engage with both protocol and security communities. |

## 6. Video Introduction (≤ 5 minutes)

## 7. Conflict Of Interest Statement

Our team has no current conflicts of interest. ZK Email has small amounts of revenue from deployments but has not raised any external venture capital. Should any potential conflict arise in the future—such as new roles or overlapping commitments—we will promptly disclose it and implement clear separation of responsibilities to avoid any influence or bias. We are committed to transparency and will work with the DAO to resolve any concerns.

---

# Post #2 by daostrat.eth
Posted at: 2025-03-30T17:05:50.181Z

Hey [@Yush](/u/yush),

Thank you for submitting your application for the ENS Service Provider Program, Season 2. After review, we are pleased to confirm that your application meets the eligibility criteria as outlined in the program design.

*Metagov will monitor the snapshot you posted above.*

Good luck in SPP2!!

---

*Metagov Stewards*

---

# Post #3 by nick.eth
Posted at: 2025-03-31T09:58:21.735Z

I’ve spoken with the ZK Email team, and I’m very impressed with what they’ve built and are intending to build. Trustless, two-way verified credentials embedded in ENS are exactly the sort of things that will enhance ENS’s usefulness as a decentralized web3 profile, and constitute a significant improvement in ENS’s core capabilities - exactly the sort of thing that the service provider program exists to fund.

Although the team lacks a history interacting with the ENS DAO, they have a solid track record delivering on their core tech, and have already demonstrated they can deliver. I have no doubt they will do an outstanding job on this, if funded, and they have my endorsement.

---

# Post #4 by alextnetto.eth
Posted at: 2025-03-31T17:44:16.125Z

Hey [@Yush](/u/yush), thanks for applying!

Quick fix needed, the program only accepts budgets in [multiples of $100k](https://snapshot.box/#/s:ens.eth/proposal/0x0cca1cf36731203e235b0e2de9041be3a16d9cdeadff6e15e1f1215c611e12ef) (e.g., $300k, $400k, $500k). So your Basic budget must be a multiple of 100k, and currently, it’s $450k.

---

# Post #5 by Yush
Posted at: 2025-03-31T19:57:37.040Z

Thanks for the note. We’ve updated the basic scope to 400K and made the below change:

For the extended scope, we’ve added the ability to pay *any* social media account through ENS, even if they haven’t created their ENS record yet. We think this can drive a lot of new apps like retroPGF or even native platform tipping (like bots tipping money on Github or Twitter, but with money claimable through zk verified records on ENS). We think this can drive new ENS activity on new platforms with new interaction modalities, and hopefully can give the DAO more confidence in our extended ask being valuable to ENS as well!

---

# Post #6 by James
Posted at: 2025-04-01T05:19:48.438Z

ZKemail team are building some of the most practicle and interesting technology in the Ethereum ecosystem, bringing web2 credentials onchain with ZK magic. Having them build alongside the ENS ecosystem is a huge win.

Social Username Resolution as a well as a **number** of the extended scope outcomes are incredibly interesting to FireEyes!

---

# Post #7 by jefflau.eth
Posted at: 2025-04-04T16:56:22.499Z

I’ve believed in programmable cryptography being the next step for ENS to be the center of identity since 2021. Back then, it was largely a pipe dream and teams preceding ZK-email were building circuits to prove simple things like keccak256. It’s amazing to see the technology progress to the point where it can actually be used in applications such as ENS. If this can all be proved on a mobile device and client-side, which from zk-email’s proposal is highly likely I’d love to see this powering ENS resolvers for fully permissionless verified records.

I am happy to endorse ZK email for SPP2

---

