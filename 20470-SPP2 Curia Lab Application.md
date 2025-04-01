# Post #1 by Curia
Posted at: 2025-03-31T13:02:38.093Z

**1. Applicant Information**

**Company Name:** Curia Lab

**Website:** [https://curialab.xyz](https://curialab.xyz/)  

**X/Twitter:** [Curia\_gov](https://x.com/Curia_gov)

**Primary Contact/Entity ENS Name:** curia-delegates.eth

**Primary Contact(s)**

* [Varit Ruangsiri](https://x.com/v3eth), Co-founder, v3naru.eth

**Company Overview**

* Curia Lab develops robust governance analytics solutions for DAOs, empowering decentralized communities with data-driven insights to enhance transparency, decision-making, and participation.
* Our tools support major protocols, including Optimism’s Token & Citizen House, ArbitrumDAO, and SafeDAO.

**Requested Amount:**

* $300,000 (basic scope, 1 yr)

**Size of team and commitment:**  

Curia Lab has a dedicated full-time team of 11 contributors, consisting of governance analysts, data engineers, full-stack developers, and product designers. If we are selected for the SSP program, supporting ENS DAO will become a strategic priority for us, and our team will allocate substantial resources and attention to ensure high-quality outcomes.

---

**2. Eligibility Confirmation**

**Company Age & Reputation:**  

Curia Lab was established in 2023 as part of an incubating project from SCB10x (SEA’s leading Blockchain, Fintech, AI focused venture capital). We officially spin-off and incorporated a company in Singapore on February 2024. Our proven track record includes building sophisticated governance analytics dashboards and governance related tools for prominent DAOs like [**Optimism**](https://optimism.curiahub.xyz/), [**Arbitrum**](https://arbitrum.curiahub.xyz/), and [**Safe**](https://safedao.curiahub.xyz/), receiving consistent positive feedback and adoption by the communities.

**Team Experience:**

* Our team has extensive experience in DAO governance analytics, blockchain data indexing, and delivering impactful governance analytics.
* We developed the Dynamic Delegate Attestation system for the Optimism Foundation, automating onchain attestations for the top 100 delegates in Optimism’s governance system ([GitHub link](https://github.com/CuriaLab/dynamic_attestation_mvp)).
* We’ve built the [OP Passport](https://docs.oppassport.xyz/), which provides onchain attestations of governance participants’ histories, supporting both public and privacy (ZK) endorsements/attestations.
* We actively serve as delegates for several prominent DAOs, including Optimism, Arbitrum, zkSync, Uniswap, Obol, and Gnosis, with a focus on promoting transparency and accountability. Additionally, our co-founder Varit has been elected to serve on Optimism’s Milestones & Metrics Council in each of the past three elections since its inception.

**ENS Token Endorsement Requirement:**  

Curia Lab has not yet secured endorsement but intends to seek public endorsement via Snapshot on April 1st.

**OFAC Sanctions Compliance:**  

We, Curia Lab, confirm that neither our organization nor any employees, contractors, or executive leadership is located in, or residents of, an OFAC-sanctioned country. We further confirm compliance with all applicable sanctions laws and will promptly notify ENS DAO if our status changes.

---

**3. Open Source Commitment**

All work funded by ENS DAO through this program will be openly available under the MIT license on Curia Lab’s public GitHub repository.

---

**4. Scope of Work & Budget**

**4.1 Basic Scope of Work:**

**Requested amount: $300K USD**

We believed ENS’s long-term success also depends on its resilient and transparent governance. Our scope aim to provide a comprehensive framework integrating research, methodologies, and continuous monitoring in order to achieves these key goals:

### **Key Goals:**

**Goal #1: Strengthen ENS governance data & insights accessibility**

**Goal #2: Improve community participation and accountability**

**Goal #3: Enable proactive identification of governance improvement opportunities and risks**

### Phase 1: Data Aggregation & Pipeline Development

> **Supports Goal #1** by aggregating previously fragmented governance data — onchain and offchain, ensuring stakeholders have easy access to comprehensive, up-to-date insights.

* **Objective:** Our indexing solution will integrate ENS governance data from multiple onchain and offchain platforms, combining Ethereum blockchain data, Snapshot governance interactions, Ethereum Follow Protocol profiles, Agora proposals and votes, [Multi-Delegate Manager (MDM)](https://ens.domains/blog/post/multi-delegate-manager) multi-delegation activities, and Discourse forum discussions to create a comprehensive view of ENS governance.
  + **Data Capture & Indexing Methodology**: We’ll implement both full historical backfilling and daily incremental updates across all platforms. Our approach captures Ethereum mainnet data (governance contracts, token transfers, voting power changes, delegation logs) alongside offchain data from Snapshot, EFP, Agora, Tally, [MDM](https://ens.domains/blog/post/multi-delegate-manager), and Discourse. This dual strategy ensures both historical context for trend analysis and current data for active governance monitoring, with built-in error handling to prevent data gaps.
  + **Platforms and Integration**: The solution leverages Google Cloud BigQuery and Flipside Crypto for onchain indexing, complemented by direct API integrations with Snapshot, EFP, Agora, and Discourse. These connections create a unified governance data lake offering comprehensive visibility into ENS governance processes across all relevant platforms.
  + **Technical Architecture**: Our infrastructure uses Google Cloud BigQuery as the primary data warehouse with Flipside Crypto for specialized blockchain analytics. Custom connectors will ingest data from all APIs, processed through SQL transformations and served via a Next.js frontend hosted on Vercel. Cloud-based distributed storage ensures scalability, with redundancy built into critical components for reliability.
* **Deliverable**: The final product will be a robust indexing system that seamlessly integrates onchain and offchain governance data, capturing activities across all platforms to reveal the nuanced dynamics of ENS governance. This unified view will provide the ENS community with actionable insights into governance participation, proposal effectiveness, and community sentiment to support more informed decision-making.

### Phase 2: ENS Governance Research & Analytics Framework

> **Supports Goal #1** — **Strengthen ENS governance data & insights accessibility**

> **Supports Goal #3** — **Enable proactive identification of governance improvement opportunities and risks**

* **Objective:** Develop an analytics framework to diagnose governance challenges within ENS, enabling proactive improvements and strategic insights.
  + **Step 1: Study ENS Governance:** Conduct a detailed review of ENS governance, analyzing token distribution, delegation dynamics, proposal mechanisms, stakeholder roles, protocol parameters, and smart contract structures. This contextual understanding ensures our analytics accurately address ENS’s unique governance environment.
  + **Step 2: Develop a Governance Evaluation Framework:**  
    
    Establish a comprehensive set of key governance metrics—covering **both onchain and offchain activities**—to provide a holistic view of ENS governance. This structured framework will deliver actionable insights, facilitate benchmarking against other DAOs, and support informed decision-making by delegates and stakeholders.  
    
    **An initial list of proposed metrics is available** [**here**](https://www.notion.so/Governance-Evaluation-Framework-1c62dc1c1f7980d5b825d1dfabcc1e79?pvs=21).
  + **Step 3: In-Depth Analysis Report:** Produce an extensive analytical report specifically tailored to ENS governance, incorporating industry-leading practices to systematically identify key trends, governance gaps, and strategic opportunities. This process includes:
    
    - In-depth quantitative and qualitative analyses of governance data.
    - Comparative evaluations of ENS governance relative to peer DAOs.
    - Community validation through surveys, interviews, and collaborative stakeholder feedback sessions…
* **Deliverable:** A detailed research report featuring clear findings, actionable recommendations, and a robust governance evaluation framework to guide continuous enhancements. Additionally, this phase also includes the initial draft of the periodic governance analytic reports.

### Phase 3: Dashboard Visualization & Monthly Governance Reports

> **Supports Goal #1** by presenting data in a user-friendly way, improving accessibility for all stakeholders

* **Objective:** Convert research findings into an interactive, intuitive dashboard providing near real-time governance analytics and insights, complemented by continuous reports.
  
  + **Step 1: Design & Prototyping** *Conduct stakeholder workshops to comprehensively define essential governance metrics and develop iterative wireframes and mockups for dashboard design.*
    - ***Stakeholder Engagement:***
      * *Host collaborative workshops with ENS stakeholders to precisely define governance metrics critical to effective decision-making and oversight.*
      * *Ensure alignment between s*takeholder expectations and dashboard functionalities.
    - **Wireframing & Mockups:**
      * Create iterative low-fidelity and high-fidelity prototypes, clearly illustrating dashboard structure, layout, and interaction flows.
      * **Overview Pages:** Develop concise summaries highlighting essential governance metrics for quick and efficient insights.
      * **Detailed Sections:** Create detailed dashboards offering comprehensive analyses of holders, delegates, voting power dynamics, proposals, participation patterns, forum interactions, and security indicators.
  + **Step 2: Dashboard Development:** Implement the governance dashboard through structured development phases, prioritizing responsiveness, accuracy, and near real-time performance.
    - Development Process:
      * Front-End Development: Build a responsive and modular dashboard using modern frameworks (e.g., Next.js). Integrate near real-time data via secure API connections to ensure up-to-date governance insights.
      * Back-End Integration: Establish a robust integration between the data pipeline and the visualization layer, ensuring secure, seamless, and efficient data flow.
      * Testing & Optimization: Conduct comprehensive testing phases—including unit, integration, and user acceptance testing—to ensure accuracy, performance, and a smooth user experience.
  + **Step 3: Monthly Governance Reports:** Generate comprehensive, monthly governance reports. These reports will help identify governance trends, detect anomalies or suspicious activities, and ensure the community can rapidly respond to emerging governance events.
  > **Supports Goal #1** — **Strengthen ENS governance data & insights accessibility**
  
  > **Supports Goal #3** — **Enable proactive identification of governance improvement opportunities and risks**
  
  + **Key Governance Metrics Focus:**
    - Highlight essential governance metrics including voter behavior, delegate activity and effectiveness, proposal outcomes, and changes in voting power distributions to provide stakeholders with an accurate governance overview.
  + **Actionable Recommendations:**
    - Offer specific, actionable recommendations based on identified governance trends, such as enhancing participation, adopting effective governance practices, or addressing potential governance vulnerabilities.
  + **Customized Reports Based on Community Input:**
    - Tailor report content to reflect the needs and interests of the ENS community, actively integrating feedback and suggestions to maintain report relevance and effectiveness.
  + **Visual Representation of Data:**
    - Utilize intuitive visual formats (charts, graphs, infographics) to make governance insights accessible and understandable to all community members, irrespective of their data literacy levels.
* **Deliverable:** Near Real-time interactive analytics dashboard and monthly detailed governance reports.

### Phase 4: API & Integration Toolkit

> **Supports Goal #1** — **Strengthen ENS governance data & insights accessibility**

* **Objective:** Extend our governance insights across the ENS ecosystem through a public API and integration toolkit.
* **Key Activities:**
  + Public API Access **—** Develop secure, standardized API endpoints for real-time data retrieval and provide comprehensive documentation.
  + Integration Toolkit **—** Create plug-and-play modules for embedding insights into existing platforms (e.g., [ENS Delegation page](https://delegate.ens.domains/), [Agora](https://agora.ensdao.org/), and [Tally](https://www.tally.xyz/gov/ens)).
  + Engage with the ENS community to refine and enhance toolkit features based on practical use cases.
* **Deliverable:** A publicly accessible API and toolkit that foster interoperability and extend governance analytics across the ENS ecosystem.

### **Looking Ahead: Namechain Readiness**

We recognize that significant changes to ENS governance may arrive with Namechain (~late 2025/2026). As part of our approach, we will stay closely involved with delegates and the broader community to ensure our analytics framework, dashboard, and integrations seamlessly adapt to new L2 or specialized governance structures. Curia Lab is prepared to serve as an ongoing partner, bridging the transition between current governance mechanisms and the evolving Namechain framework to maintain robust, transparent oversight.

**KPIs / Success Metrics:**

* ≥99% uptime for the governance analytics dashboard and underlying data pipeline
* ≥99% uptime for the public API
* Initial governance research report delivered by end of Q1
* Dashboard MVP with live data visualizations delivered by end of Q2
* Monthly governance reports delivered within 10 days after each month
* Successful integration of our analytics into at least 2 external platforms by end of Q4

---

**5. Past Achievements & Additional Information**

* We have incorporated EFP into all of our analytics platforms. See example [here](https://arbitrum.curiahub.xyz/delegate/delegate.l2beat.eth)
* Our previous work has focused on detailed monthly governance report contributes into change within the community, (eg. SafeDAO implementation of OBRA’s [Steering Committees and Council Structures](https://forum.safe.global/t/discussion-introducing-steering-committees-and-council-structures/5718).)
* We have actively collaborated with DAO communities to refine methodologies and ensure our tools meet evolving governance needs. (eg. our api & data contributed to these community-led research: [Measuring the Concentration of Power in the Collective](https://gov.optimism.io/t/measuring-the-concentration-of-power-in-the-collective/8956), [Voting Influence and Concentration Analysis (VICA) for the Optimism Collective](https://github.com/BilalBAI/op-vica))
* We were the first analytics provider for Optimism to integrate Agora’s [advanced partial delegation](https://github.com/voteagora/ERC20VotesPartialDelegationUpgradeable) data directly from their contracts (and remained the only one for several months). Additionally, we assisted the OP Labs Data team in populating partial delegation data from Agora’s contract into their Dune dashboards—underscoring our data proficiency and dedication to near real-time, accurate data for the Optimism Collective.
* We have been recognized for our contributions to OP governance and have been a recipient in multiple rounds of Optimism’s Retroactive Public Goods Funding (RPGF), underscoring our commitment to advancing open governance data & infrastructures.

---

**6. Video Introduction (≤ 5 minutes)**

Link here: To be uploaded in the next few hours.

---

**7. Conflict Of Interest Statement & Disclosures**

* None of our team members hold positions or receive compensation from ENS Labs or other current ENS DAO-funded projects.
* Curia Lab generates revenue from delegate activities and analytics services provided to other DAOs but has no direct competitive conflicts with ENS.
* Curia Lab has raised no external funding and is currently self-sustained through revenue from services provided.

---

We look forward to the opportunity to contribute to ENS DAO’s transparent and effective governance through our analytics expertise.

---

# Post #2 by daostrat.eth
Posted at: 2025-03-31T15:06:07.024Z

Hey [@Curia](/u/curia),

Thank you for submitting your application for the ENS Service Provider Program, Season 2. We are pleased to confirm that your application meets the eligibility criteria as outlined in the program design.

A few notes:

* MetaGov will include you in the group endorsement snapshot on April 1;
* Please post back into the forum when your video summary is updated!

Good luck running for SPP2!

---

*Metagov Stewards*

---

# Post #3 by Curia
Posted at: 2025-03-31T22:40:53.735Z

Here’s our Video Summary: [SPP2 Curia Lab Application](https://drive.google.com/file/d/1yd7eIQJAuNJ3T4avAL-ki_vuCibTfrSz/view?usp=sharing)

---

As a follow-up, here are a few examples of the monthly governance reports we’ve published for other communities:

• [SafeDAO Governance Analytics Report Thread](https://forum.safe.global/t/safedao-governance-analytics-report-thread/5283/11)

• [Arbitrum Governance Analytics Report](https://forum.arbitrum.foundation/t/arbitrum-governance-analytics-january-report/28390)

The scope we’re proposing for ENS goes further than what we’ve done before, but we hope these examples give a sense of our approach and commitment to delivering value. We’re looking forward to the opportunity to contribute meaningfully to ENS—supporting transparency, surfacing insights, and helping push forward initiatives that can strengthen the DAO.

---

# Post #4 by daostrat.eth
Posted at: 2025-03-31T22:55:10.910Z

Thank you [@Curia](/u/curia) ![:saluting_face:](https://discuss.ens.domains/images/emoji/twitter/saluting_face.png?v=12 ":saluting_face:")

---

