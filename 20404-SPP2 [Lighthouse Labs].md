# Post #1 by Arnold
Posted at: 2025-03-24T17:31:18.535Z

## 1. Applicant Information

1. Team Name: Lighthouse Labs
2. Website/Company Blog: <https://lighthouse.cx/> / [Lighthouse Labs](https://mirror.xyz/lighthousegov.eth)
3. Entity ENS Name.eth: lighthousegov.eth
4. Primary Contact(s):  
   
   Arnold Almeida (1a35e1.eth)  
   
   James MacWhyte (jkm.eth)
5. Company Overview: We are focused on designing original products to improve the accessibility of on-chain governance in decentralised environments. We currently offer three services:
6. Lighthouse Governance: a native mobile governance client, offered free for end users as a public good. To date we have had over 2500 unique addresses connected to our client and delivered over 50k proposal notifications to end users.
7. Lighthouse Dispatch: an enterprise messaging tool for on-chain orgs to better engage their participants.
8. Signals: an open-source protocol currently under development, designed to surface community sentiment as a supplement to governance operations.

More details about our other achievements can be found below.

6. Requested Amount: Requesting $300k for a one year stream
7. Team / Commitment: Currently 2.5 FT resources, ready to expand to 3 if this proposal is successful. This project will be our top priority for the duration, and we do not have any conflicts on our internal roadmap.

---

## 2. Eligibility Confirmation

1. Company Age & Reputation

* We have been operating since early 2023 as a bootstrapped company.

3. Team Experience

* We were the first to market with a native mobile app that supports multiple governance systems, giving attention to complex features such as multisig voting and on-chain comments. We’ve indexed all the major DAOs across the EVM landscape and gained a large amount of insight into the struggles they face, which now informs the direction of our work.
* Arnold, Founder/CTO
  
  1. 15 years industry experience
  2. Led teams up to 10 heads
  3. Scaled orgs with headcount up to 150 at C level
  4. Taken 10+ products to market from ideation
  5. One exit, two public listings
* James, CPO
  
  1. 12 years crypto startup experience
  2. Early-stage Coinbase and Kraken
  3. C-level at BRD, involved in 4 rounds of funding leading to one exit
* Xaun, Head of Engineering
  
  1. 10 years digital experience
  2. Led cross functional teams up to 8 heads
  3. Digital Agency, Founder Experience

3. ENS Token Endorsement Requirement

* We have been informed that we do meet this requirement.

4. OFAC Sanctions Compliance

* We, [Lighthouse Labs], confirm that neither our organization nor any of our employees, contractors, or executive leadership is located in, or a resident of, an OFAC-sanctioned country. We further confirm that none of our business resources are derived from or routed through any country or entity that is subject to sanctions imposed by the United States (OFAC) or equivalent regulatory bodies. We pledge to remain compliant with all applicable sanctions laws and will promptly notify the ENS DAO if our status changes.
* For avoidance of doubt, all employees currently reside in:
  1. United Kingdom
  2. Australia

5. Multi Year Stream Eligibility

* None

---

## 3. Open Source Commitment

Our core product, Lighthouse, is a free, native mobile app which is not currently open-source. However, we commit to building the work in this proposal as public, open-source resources which we will then integrate into our core product.

The Signals protocol is already open source, and will continue to be.

## 4. Scope of Work & Budget

## 4.1 Basic Scope of Work

Total requested amount: $300k

### Overview

For this proposal, we would like to focus on work that will deeply integrate ENS’s on-chain functionality into the Lighthouse app and make on-chain governance data easily and publicly accessible.

## Project 1: Integrating ENS into Lighthouse and offering public tools

Budget: $150k

Overview: We already require DAOs represented in Lighthouse to have an ENS configured, and we display end users’ ENS data throughout the app. We would like to expand on this support, by adding additional ENS functionality. We will make the below deliverables publicly available, and will also use them to add this additional functionality to the Lighthouse experience.

Deliverable 1: We will create an open-source reference implementation of the following key ENS features for native mobile clients:

* Register an ENS name
* Renew an ENS name
* Update ENS text records and other metadata
* Delegate voting power to ENS user
* Lookup and display an ENS user’s metadata

With this, others will be able to easily integrate ENS functionality into their own react native apps.

Deliverable 2: We will release an open-source indexer, designed to do the following:

* Surface all of the important on-chain data related to the ENS ecosystem
* Trigger notifications of upcoming expirations and other important events that users may want to be made aware of
* Provide an index of all ENS delegates
* Surface on-chain proposal metadata

This software can be run locally to build an index of the above data items, allowing for quick lookups of requested data, either in an enterprise setting or for personal use.

Deployment: In addition to providing more open-source resources that others can use in their own projects, we will integrate the above into our Lighthouse ecosystem, enabling the following features:

* In-app ENS onboarding flow for new users
* In-app notifications of upcoming expiration and important ENS-related situations for all app users who have an ENS registered
* In-app customization of a user’s ENS profile, including control over how they appear in the Lighthouse app
* In-app surfacing of ENS delegates, and easy delegation of voting power

These features will make Lighthouse a much more powerful tool for ENS governance participation, but will also bring more activity and users to ENS and further solidify ENS’s reputation of being an on-chain representation of one’s identity.

Measure of success:

* Number of forks/stars of open-source repos
* Number of new ENS names registered through Lighthouse
* Number of ENS-related notifications delivered through Lighthouse
* Number of votes facilitated on Lighthouse for both Governor and Snapshot systems

## Signals Protocol development

Budget: $150k

Overview: In the lead up to the SPP2 vote, we witnessed weeks of debate about how to best distribute a $4.5M budget via a voting system that was not specifically designed to support the type of decision-making we are trying to undertake. The final solution required a lot of work and coordination between multiple service providers, and it was a great example of governance in action! However, we are now even more confident that the industry as a whole can use more nuanced tools for managing these types of decisions, and we believe the Signals Protocol could be one of those tools.

Why Signals: We developed Signals specifically to surface sentiment within an on-chain community. Forum posts don’t always necessarily reflect the poster’s true intentions, and decisions made by voting alone can be heavily swayed by large token holders. Signals aims to solve these problems by allowing community members to temporarily lock up their governance tokens in support of initiatives, and the opportunity cost of these lockups will filter out weakly-held opinions. By giving greater weight to lockups that are committed to for a longer time, even small token holders can have their voice represented.

We believe Signals could improve decision-making participation amongst DAO participants, and reduce the need for paid delegates and committees.

Here’s how it works:

1. A Signals “board” is created and configured for a particular DAO, specifying eligibility requirements, which tokens will be used, and other aspects.
2. DAO members submit initiatives that they think are important for the community to get behind. These can be anything from vague concepts to detailed proposals. The DAO is free to decide what format is most useful to them.
3. Other participants can lock up their governance tokens in support of the initiatives they agree with. Locking up tokens for a longer time is counted as a larger amount of support, allowing even small token holders to have an equal voice.
4. Once an initiative has reached a preconfigured threshold of support, the DAO can officially “accept” the initiative which signals an acknowledgement that the community has reached alignment.
5. When an initiative is accepted, all tokens are unlocked and returned to their owners. Unpopular initiatives will eventually expire and unlock as well, however the opportunity cost means users will only want to support initiatives they believe will have a strong chance of being accepted in a timely manner.

Current state: Signals is currently in the PoC stage, having been built during a hackathon in which we won first place. We have a working prototype which includes the following features:

* Basic factory contract: Users can deploy their own contracts.
* Signals core functionality: users can submit initiatives and lock up tokens to provide support. Eligibility and other restrictions can be configured. Additional incentives can be contributed towards initiatives.
* Web GUI: Full visibility of all initiatives and how much support and incentives they have received, including visualizations of how additional support may impact an initiative.

Live demo: <https://signals.capstone.lighthouse.cx/>

Deliverable: We will continue the next stage of protocol development, taking Signals from a hackathon proof-of-concept to a production-ready product. This includes:

* Completion of the Signals smart contracts, including incentives accounting and management, weight calculation customization, and exposing all essential methods
* Completion of the Signals factory contract, optimized for efficient deployments
* Completion of and improvements to the reference Signal web app, which will allow full access to deploying new boards and interacting with existing ones
* Gas optimization
* The finalization of a protocol spec and relevant documentation
* Preparation for a full code audit and pilot program

Our goal will be to run up to 3 testnet pilot programs in collaboration with the DAO, and work closely with participants to improve the mechanism design with ENS DAO’s needs in mind.

We intentionally chose to not include a mainnet deployment in our proposal, because of the amount of work required to get a new protocol ready to touch user assets. We have plans in place for a full code audit, after which we will be ready to run a mainnet pilot.

Although there will be no obligation for ENS to adopt this protocol, we plan to suggest it as an option for SPP3 and will work towards making it fit for that purpose.

Measure of success:

* Number of ENS holders who participate in the Signals pilot program
* Metrics from the pilot program final report

## 5. Past Achievements & Additional Information

**Signals**

* Arbitrum x RnDAO Collabtech hackathon - 1st place winner
* Uniswap Hooks Incubator - winner of Arbitrum track and Uniswap Foundation track

**Grants and recognition**

* Safe DAO grant for Safe x Snapshot integration
* Optimism retrofunding recipient
* Gitcoin recipient - recognized public good

**ENS contributions**

*Supported ENS Snapshot + Governor*

Voting on ENS with the Lighthouse Governance Client supports both Snapshot and on-chain Governor. Users of Safe can also enjoy voting using their Safe on the ENS Snapshot space.

*SPP2 Vote*

In the lead up to the SPP2 vote, we have contributed to the shaping of the SPP2 program. We designed a custom interface in Lighthouse specifically for this vote, and pushed for making the voting data machine-readible and accessible. We open sourced the library we wrote for this project, and have designed it specifically so ENS and others can use it on other similar proposals in the future.

* Github [GitHub - 0xLighthouse/snapshot-copeland-results](https://github.com/0xLighthouse/snapshot-copeland-results)

---

## 6. Video Introduction (≤ 5 minutes)

* [ens-spp-remastered.mp4 - Google Drive](https://drive.google.com/file/d/16hiJfBZFquWWJBy91J-PNUjeqYDQC784/view)

## 7. Conflict Of Interest Statement

None

---

# Post #2 by daostrat.eth
Posted at: 2025-03-24T22:42:56.012Z

Hi [@Arnold](/u/arnold)!

Thank you for submitting your application for the ENS Service Provider Program, Season 2. **After review, we are pleased to confirm that your application meets the eligibility criteria as outlined in the program design.** MetaGov will also include Lighthouse Labs in the *endorsement snapshot* on April 1. ![:saluting_face:](https://discuss.ens.domains/images/emoji/twitter/saluting_face.png?v=12 ":saluting_face:")

We want to point out a quick note regarding program compliance if selected for SPP2.

The program design, per the most recent passed [snapshot](https://snapshot.box/#/s:ens.eth/proposal/0x0cca1cf36731203e235b0e2de9041be3a16d9cdeadff6e15e1f1215c611e12ef), states that all work funded directly by the SPP must be open sourced (MIT). We encourage all applicants to align scope with this criteria.

> All work done directly funded by this program must be Open Source and Freely Licensed (MIT). Service Providers are free to also have proprietary codebases but the works establised in their proposals and quarterly reports must also be available on github or other public repositories.

We look forward to seeing you in the running for SPP2!

---

*Metagov Stewards*

---

# Post #3 by Arnold
Posted at: 2025-03-31T20:29:55.348Z

Hi all, based on feedback and a closer look at the open source requirements, we have updated our proposal and included additional details.

We are unable to edit the main post, so here are the revised sections 3&4 (the rest is the same). The entire updated proposal [can be seen here](https://docs.google.com/document/d/1Crr7NW3q-xpfhUp2JP6p2TI3zqEz_JoMDtiqNdZubZQ/edit?usp=sharing).

## 3. Open Source Commitment

Our core product, Lighthouse, is a free native mobile app which is not currently open-source. However, we commit to building the work in this proposal as public, open-source resources, and will then (using other funding) integrate that work into our core product.

The Signals protocol is open source, and that will not change for continued Signals development.

## 4. Scope of Work & Budget

## 4.1 Basic Scope of Work

Requested amount: $400k

### Overview

Lighthouse’s core product is a native mobile app that optimises governance participation and communication, and in the course of developing this product we have gotten deeply involved in the area of on-chain governance data and infrastructure. For this proposal, we would like to focus on work that will

1. Deeply integrate ENS functionality into the Lighthouse app
2. Make on-chain governance data easily and publicly accessible
3. Advance ENS’s governance objectives for the ENS DAO

## Integrating ENS into Lighthouse and offering public tools

Budget: $150k

Overview: We already require DAOs represented in Lighthouse to have an ENS configured, and we support end users’ ENS data throughout the app. We would like to expand on this support, by adding additional ENS functionality throughout our app. We will make the below deliverables publicly available, and will also use them to add this additional functionality to our app.

Deliverable 1: We will create an open-source, reference implementation of the following key ENS features for native mobile clients:

* Register an ENS
* Renew an ENS
* Update ENS text records and other metadata
* Delegate voting power to ENS user

Deliverable 2: We will release an open-source indexer, designed to do the following:

* Surface all of the important on-chain data related to the ENS ecosystem
* Trigger notifications of upcoming expirations and other important events that users may want to be made aware of
* Provide an index of all ENS delegates
* Surface on-chain proposal metadata

Impact: In addition to providing more open-source resources that others can use in their own projects, we will integrate the above into our Lighthouse ecosystem, enabling the following features:

* ENS onboarding flow for new users
* In-app notifications of upcoming expiration and important ENS-related situations
* In-app customization of a user’s ENS profile, in relation to how they appear in the Lighthouse app
* In-app surfacing of ENS delegates, and easy delegation of voting power

These features will make Lighthouse a much more powerful tool for ENS governance participation, but will also bring more activity and users to ENS and further solidify ENS’s reputation of being an on-chain representation of one’s identity.

Measure of success:

* Number of forks/stars of open-source repos
* Number of new ENS names registered through Lighthouse
* ENS-related notifications delivered through Lighthouse

## Increase transparency and improve ENS DAO operations

Budget: $150k

Overview: We currently offer a service called Lighthouse Dispatch which enables DAOs to broadcast official communications to their members. With Dispatch, users who are authorized to publish messages on behalf of the DAO can broadcast their official communications through the Lighthouse platform, getting the attention of DAO members through push notifications. All communications are authenticated and verifiable, and members can discuss proposals and announcements directly in-app.

Our next stage of innovation is to make this feature more transparent and add functionality which ENS DAO can leverage to improve DAO coordination and communication.

Deliverable 1: We will open-source our Dispatch client, making available (for reference or audit) how authentication is performed and communications are initiated.

Deliverable 2: We will add to the Dispatch client the following features:

* The ability to specify a DAO org chart (through Hats protocol or equivalent), allowing the DAO to specify who is authorized to broadcast official communications
* We will work together with ENS DAO to identify and implement the ideal solution for providing on-chain authorization of access-control lists
* Additional communications channels (member-to-member, DAO-to-member, delegate-to-delegate, etc) gated by verifiable authentication

Impact: The above improvements will give DAO communications additional credibility by adding an on-chain component to authentication and verification. It is important to note ENS DAO will not be forced to transition to a new system, and these new features will work in tandem with existing DAO infrastructure.

Measure of success:

* Number of roles publicly assigned on-chain
* Number of DAO communications and proposals initiated through Lighthouse

## Continuing Signals development

Budget: $100k

Overview: Signals is a new, experimental protocol which enables on-chain communities to surface what their members consider most important. It uses a token lockup mechanism which allows members to more concretely commit to their opinions, and enables even smaller token holders to have an equal voice.

Deliverable: We will commit 25% of this proposal’s budget towards continuing Signals development with engagement from the ENS community:

* Refinement and deployment of the Signals smart contracts and web UI
* The launch of a pilot program on testnet for ENS holders
* We will compile a final report on the findings of the pilot program and an assessment of the protocol’s appropriateness for the ENS DAO
* An analysis of pilot program metrics:
  + Number of initiatives proposed
  + Number of initiatives reaching the activation threshold
  + Impacts from activated proposals
  + User feedback

Impact: As this is the most experimental portion of this proposal, impact may be hard to predict. However, ENS will be taking a pivotal role in developing a new and novel governance protocol, which can only be a net benefit to the crypto ecosystem.

Measure of success:

* Number of ENS holders who participate in the Signals pilot program

---

# Post #5 by Arnold
Posted at: 2025-04-26T14:48:59.121Z

**[REVISON NOTES]**

After experiencing the SPP2 process, both as a governance client provider and as an applicant, we have decided to reduce our proposal’s budget to focus add valuing in two key areas:

* Refine ENS protocol availability and governance accessibility in our mobile clients
* Focus on development of the new Signals protocol

We believe both of these endeavours will be net positive contributions to the ENS community.

---

# Post #6 by daostrat.eth
Posted at: 2025-04-26T14:57:25.705Z

Thanks for the updated proposal and continued contribution [@Arnold](/u/arnold).

I also endorse this application. Look forward to seeing you in the SPP2 vote.

---

