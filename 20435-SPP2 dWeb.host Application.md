# Post #1 by chomtana
Posted at: 2025-03-28T23:52:11.357Z

## 1. Applicant Information

1. **Company / Team Name:** dWeb.host
2. **Website/Other**: <https://dweb.host>
3. **Primary Contact/entity ENS Name.eth:** dwebhost.eth
4. **Primary Contact(s)**
   * Chomtana Chanjaraswichai
   * chomtana.eth
   * [Telegram: Contact @chomtana](https://t.me/chomtana)
5. **Company Overview:** dWeb.host is a collaboration between Opti.Domains and Upnode to research, build, and deploy critical dWeb infrastructure on ENS. We identify gaps in ENS dWeb infrastructure and address them.
6. **Requested Amount**:
   * $300k - Basic Scope
   * $400k - Extended Scope
7. **Size of team and commitment**
   * 5 full time engineers (frontend/backend/smart contract/devops)
   * Engineers will appropriately allocated to each task

---

## 2. Eligibility Confirmation

*(Please confirm each point below.)*

1. **Company Age & Reputation**
   * Opti.domains has been working on ENS L2 on Optimism for more than 1 year.
   * Upnode has been a mainnet validator for Celestia for more than 1 year and has received foundation delegation.
   * Our company has been registered in the Isle of Man for more than 1 year.
   * More information on “Past Achievements” section
2. **Team Experience:**

**Chomtana Chanjaraswichai** - Team Lead

* [Opti.domains: ENS L2 on OP](https://ens.opti.domains)
* [Optimism TechNerd](https://retrolist.app/project/0x127bdc6d776fb958f986cd2059b43e917a2d74e912c0b360316f77a05b30087b)
* [RetroList](https://retrolist.app/) - Optimism Retro Funding Discovery UI
* [Maintaining simple-optimism-node](https://github.com/smartcontracts/simple-optimism-node)
* [Top 100 Optimism Delegate](https://vote.optimism.io/delegates/delegate.chomtana.eth)
* Won many hackathons
* And more…

**Johny Phan** - Full Stack Developer - Dedicated to dWeb.host project

* Develop prototype of [dWeb.host IPFS Pinning for ENS domains](https://alpha.dweb.host/stats)
* Develop prototype of [dWeb.host Vercel for ENS](https://alpha.dweb.host)
* Develop UI for [Opti.domains ENS L2 on OP](https://ens.opti.domains)

1 more full stack developer, 1 more frontend developer and 1 more backend developer

4. **ENS Token Endorsement Requirement:** No public endorsement as of yet. Please consider voting for us in the upcoming vote!
5. **OFAC Sanctions Compliance**
   * Our company is registered in the Isle of Man, a Crown Dependency of the United Kingdom.
   * All employees currently reside in the Isle of Man, the United Kingdom, Thailand, and Vietnam.
   * We, dWeb.host, confirm that neither our organization nor any of our employees, contractors, or executive leadership is located in, or a resident of, an OFAC-sanctioned country. We further confirm that none of our business resources are derived from or routed through any country or entity that is subject to sanctions imposed by the United States (OFAC) or equivalent regulatory bodies. We pledge to remain compliant with all applicable sanctions laws and will promptly notify the ENS DAO if our status changes.

---

## 3. Open Source Commitment

Yes, dWeb.host is fully open-source, and its source code is accessible at [dwebhost · GitHub](https://github.com/dwebhost)

The source code for our dWeb.host prototype (Both the IPFS Pinning service and the Vercel for ENS prototype) is open-source and available at [GitHub - dwebhost/dweb-alpha](https://github.com/dwebhost/dweb-alpha).

## 4. Scope of Work & Budget

At dWeb.host, our team is addressing key infrastructure and application gaps in the ENS dWeb ecosystem.

To tackle these challenges, we propose the following solutions:

1. Develop a **decentralized IPFS and IPNS pinning service for all ENS domains** with at least 3 external node operators.
2. **dWeb Deployer and Builder Network**: Develop an infrastructure and SDK that enables developers to easily develop and deploy a profile dWeb that anyone can claim and personalize, and a community subdomain dWeb that serves all members of a community.
3. **dWeb Gallery**: Enable end users to easily configure and claim a subdomain representing a personalized website derived from the base domain.
4. (Extended Scope) **CNAME Gatewa**y: Enable end users to connect their DNS names to ENS websites through CNAME and TXT records in a Vercel-like experience.

Here are the key issues we are addressing:

1. Most ENS websites are hosted on IPFS but many of them are inaccessible.
2. Unique dWeb use cases exclusive to ENS? Claimable profile dWeb for all, Subdomain community dWeb? These solutions remain challenging to develop today.
3. (Extended Scope) When there are such unique websites but users prefer to use their Web 2 domain, there is currently no way to easily link a Web 2 domain to an ENS website.

And by having external node operators run the infrasturucture, we can improve the overall reliability of the ENS dWeb infrastructure. They would not only support essential services but also pave the way for future innovations—such as a serverless function system, which, while outside the scope of our current proposal, exemplifies the potential benefits of a decentralized node operator network.

### Working Prototype

To demonstrate our expertises and commitment, we have developed two prototypes:

1. An IPFS pinning service for all ENS domains.
2. A Vercel-like deployer for building and deploying decentralized websites from the source code of any open-source repository.

The IPFS pinning service prototype indexes all content hash change events and attempts to pin each corresponding IPFS website to our local IPFS node. As a result, we discovered that many ENS websites on IPFS are no longer retrievable.

Currently, we have indexed over 40,000 websites on 20,000 unique ENS domains and have successfully pinned over 8,000 websites, which occupy approximately 40 GB of disk space. This number continues to grow as more sites are pinned.

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/eb92f6c0c10dbf4fe0b609ae90baa21b8e0e72e8_2_690x305.png)image2028×898 43.7 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/eb92f6c0c10dbf4fe0b609ae90baa21b8e0e72e8.png "image")

Live pinning statistics are available at: [dWeb - Deploy decentralized websites](https://alpha.dweb.host/stats)

Another prototype is a Vercel-like deployer that enables anyone to deploy any open-source repository on GitHub directly to their ENS domain name.

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/2/297da23acd2a758e7f5e3be2cd54aa9ce018978d_2_690x307.png)image1905×849 47.7 KB](https://discuss.ens.domains/uploads/db9688/original/2X/2/297da23acd2a758e7f5e3be2cd54aa9ce018978d.png "image")  

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/85c04bd75a954c8a6df799a99562d704e84c515e_2_520x499.png)image908×873 38.9 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/85c04bd75a954c8a6df799a99562d704e84c515e.png "image")  

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/7/748b0187868e016441d2d836855d317e75fd402e_2_407x500.png)image924×1133 43.3 KB](https://discuss.ens.domains/uploads/db9688/original/2X/7/748b0187868e016441d2d836855d317e75fd402e.png "image")

This Vercel-like deployment UI is live at: <https://alpha.dweb.host>

The source code for both prototypes is available at: [GitHub - dwebhost/dweb-alpha](https://github.com/dwebhost/dweb-alpha)

### Critical Infrastructure: Decentralized IPFS and IPNS Pinning for all ENS domains

This same idea was discussed years ago on this forum.

![](https://discuss.ens.domains/user_avatar/discuss.ens.domains/gregskril/48/3877_2.png)
[IPFS Nodes for Pinning .eth Websites](https://discuss.ens.domains/t/ipfs-nodes-for-pinning-eth-websites/12662) [Ecosystem Discussion](/c/ens-ecosystem/ecosystem-discussion/33)
> Summary
> It seems that most .eth websites are pinned to IPFS via commercial pinning services. These services are fantastic for uploading to IPFS, but we should not rely on them as the primary host of .eth websites. Otherwise, we’re back at step 1 (centralized website hosts). To further decentralize the stack, the ENS DAO should have its own IPFS nodes that are dedicated to pinning .eth website content.
> Background
> During the last [.eth Websites Subgroup meeting](https://discuss.ens.domains/t/eth-websites-subgroup-meeting-may-10-2022-17-00-cet/12555/2), we heard from several community m…

Many websites hosted on IPFS have been lost in eternity. Moreover, IPNS websites are even more prone to loss because they are mapped to a key on an IPFS node that is easily lost. Notably, even <https://nick.eth.limo>, which is hosted on IPNS, is inaccessible at the time of writing.

We solve this by providing a free IPFS pinning service for all ENS domains, regardless of the primary pinning service (e.g., Pinata, Firebase) they use.

| **Features** | **Cost** |
| --- | --- |
| IPFS Pinning for all .eth domains | 20,000$ |
| IPNS Caching network for .eth domains | 20,000$ |
| IPFS Direct peering with eth.limo | - |
| Explorer and Wayback Machine | 10,000$ |
| 2 Instances of pinning node hosted by us | 40,000$ |
| 3 External pilot node operators | 60,000$ |
| **Total** | **150,000$** |

Initially, we propose that free IPFS pinning support be rate-limited to 1 GB per 2LD .eth domain to prevent abuse. We expect to increase this limit once the network is stable to accommodate new use cases.

This is the most critical infrastructure within ENS, and we will allocate all of our engineers to its development and launch in Q2 2025.

### Decentralized Source Code Builder Network

Imagine you are building a no-code website maker. Traditionally, you would need to develop a deployment pipeline to build websites on demand. However, because no-code website makers are designed for developers with both frontend and UX/UI skills, creating these pipelines can be a cumbersome process. With the Decentralized Source Code Builder Network, developers can build websites directly from the frontend, eliminating the need for a dedicated builder server.

| **Features** | **Cost** |
| --- | --- |
| Source code builder node | 20,000$ |
| Control plane for task distribution | 20,000$ |
| Share node operators with IPFS pinning | - |
| **Total** | **40,000$** |

The pilot set of node operators is shared with the Decentralized IPFS and IPNS Pinning services, so it doesn’t incur additional cost. The control plane will enforce an appropriate rate limit.

### API and SDK for building a dWeb for every name

To build a no-code website maker, we typically require two components that do not currently exist:

1. An SDK and API capable of building a website template from source code and returning a pinned IPFS CID. This serves as the interface for the decentralized Source Code Builder Network.
2. An SDK that dynamically resolves records based on the origin domain name (e.g., accessing `chomtana.sourcer.eth.limo` should resolve records from `chomtana.sourcer.eth`, which merges records from `chomtana.eth` with specific records defined in `chomtana.sourcer.eth`).

If we are using Vercel, we had to handle a complicated authentication process that needed a user key just to trigger a new deployment, which meant we even had to rebuild Vercel to build a portfolio maker site.

| **Features** | **Cost** |
| --- | --- |
| Source Code Builder API and SDK | 20,000$ |
| Origin ENS name resolver SDK | 10,000$ |
| **Total** | **30,000$** |

#### Source Code Builder API and SDK

An SDK that let developer deploy any website from source code with a simple syntax like this

```
deploy({
  repo: "https://github.com/Chomtana/snake-game",
  branch: "main",
  buildSettings: {
    installCommand: "yarn install",
    buildCommand: "yarn build",
    rootDirectory: "",
    outputDirectory: "dist",
  },
  environmentVariables: {
    VITE_SOME_KEY: "Hello World!",
  },
  authentication: ... (Optional) ...,
})

```

Authentication is optional; however, if the user authenticates with a wallet that holds an ENS domain, it will be given higher priority during high-demand periods.

Our goal is for this API to work in the browser, enabling developers to build website builders without requiring any server or DevOps expertise.

#### Origin ENS name resolver SDK

To build a website like `https://web3.bio/vitalik.eth` and have it accessible from URLs like `https://vitalik.web3bio.eth.limo` or even linked to a custom DNS domain such as `https://vitabio.me` we need an SDK that dynamically converts the origin (e.g., [https://vitalik.web3bio.eth.limo](https://vitalik.web3bio.eth.limo/) or [https://vitabio.me](https://vitabio.me/)) into the corresponding ENS domain name (vitalik.eth).

In the case of Web3.bio, the domain name is specified in the path (/vitalik.eth), so there’s no issue. However, when the domain is specified as a subdomain (vitalik.web3bio.eth.limo) or as a custom domain ([vitabio.me](http://vitabio.me)), resolving the ENS name becomes less straightforward.

The origin ENS name resolver SDK addresses this challenge as follows:

```
originEnsName("vitabio.me") -> "vitalik.web3bio.eth"
cname("vitalik.web3bio.eth") -> "vitalik.eth"

```

Additionally, the ENS domain **vitalik.web3bio.eth** is equipped with a special resolver that merges the records from **vitalik.eth** with specific records set directly in **vitalik.web3bio.eth**.

We might also require an ENSIP to set up a CNAME record for an ENS name, as well as a TXT record for a DNS domain that points to an ENS name.

### dWeb Gallery and Deployer

The dWeb Gallery and Deployer simplify the development and user experience for use cases unique to ENS, such as:

1. Claimable profile dWebs for all ENS users
2. Subdomain-based community dWebs

With dWeb.host, developers can deploy their app just once—similar to Vercel—but then allow .eth holders to claim subdomains and customize their records. For instance, once `sourcer.eth` website is deployed, a user holding `chomtana.eth` can claim the `chomtana.sourcer.eth` website, with records automatically inherited from `chomtana.eth` for a personalized experience.

By default, dWeb Gallery uses the user’s .eth 2LD domain as a subdomain, increasing the utility of the eth domain and boosting revenue for the DAO. Additionally, this approach prevents minting legally sensitive or speculative names such as `coinbase.sourcer.eth`.

| **Features** | **Cost** |
| --- | --- |
| UX/UI Design | 10,000$ |
| dWeb Gallery Development | 20,000$ |
| dWeb Deployer Development | 40,000$ |
| Smart Contract Development | 10,000$ |
| **Total** | **80,000$** |

Finally, we will collaborate with subdomain communities to deploy dWeb solutions that serve all their members. Subdomains should not merely be just names for airdrop hunting; instead, each should feature an innovative dWeb that encourages real use cases.

### Extended Scope

For extended scope, we plan to expand the external node operator set from three to five node operators to enhance reliability, develop a CNAME gateway based on the eth.limo codebase and a load balanced gateway across node operators.

We have discussed with the eth.limo developer to ensure that we have not recreated anything already done by eth.limo, and to obtain guidelines for developing a CNAME gateway based on their codebase.

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/9154025d8671970172536573700a28145439ebd8_2_550x500.jpeg)image1782×1618 149 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/9154025d8671970172536573700a28145439ebd8.jpeg "image")  

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/ef9b6201ca74c2465f0533378b1b30f584868297_2_690x354.png)image1796×924 246 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/ef9b6201ca74c2465f0533378b1b30f584868297.png "image")

To develop the CNAME gateway, we first need to propose an ENSIP standard that links traditional DNS names to ENS domains using a TEXT record, and create a Domain API endpoint that resolves DNS names to ENS names.

Additionally, to enhance the utility of node operators, they could work together to form a reliable, load-balanced gateway for .eth domains.

| **Features** | **Cost** |
| --- | --- |
| 2 More node operators | 40,000$ |
| CNAME Gateway Development | 40,000$ |
| Load-balanced Gateway Endpoint | 20,000$ |
| **Total** | **100,000$** |

### 4.1 Basic Scope of Work

* **Requested amount:** $300k
* **Description**: Develop and manage infrastructure solutions, including decentralized IPFS and IPNS pinning for all .eth domains and a decentralized source code builder network along with its API and SDK for developer to build dWeb applications, alongside a dWeb gallery and deployment UI application. More information is in the above section.
* **KPIs / Success Metrics**
  + Developed a decentralized IPFS and IPNS pinning infrastructure for all .eth domains by Q2 2025.
  + Developed a decentralized source code builder network by Q3 2025.
  + Proposed and developed developer tooling and an SDK by Q3 2025.
  + Developed dWeb gallery and deployer by Q3 2025.
  + Launched 2 internal nodes and collaborate with 3 external node operators by Q3 2025.
  + Maintained 99.99% uptime for the decentralized IPFS and IPNS pinning service and source code builder network (considered operational if at least one node operator remains online).
  + Number of domains deployed with dWeb deployer.
  + Number of subdomains claimed in dWeb gallery.
* **Budget:** $300k/year

### 4.2 Extended Scope of Work

* **Requested amount:** $400k
* **Description:** Expand the external node operator set from three to five node operators to enhance reliability, develop a CNAME gateway based on the eth.limo codebase and a load balanced gateway across node operators.
* **KPIs / Success Metrics**
  + Launched 2 internal nodes and collaborate with 5 external node operators by Q3 2025.
  + Developed a CNAME gateway based on the eth.limo codebase by Q3 2025.
  + Create an ENSIP for pointing a traditionally managed DNS name to an ENS name by Q4 2025.
* **Budget:** $400k/year

---

## 5. Past Achievements & Additional Information

dWeb.host is a collaboration between Opti.Domains and Upnode to research, build, and deploy critical dWeb infrastructure on ENS. Here are our past achievements:

### Opti.Domains

* [Completed a grant for the Opti.Domains project focused on scaling ENS to Optimism](https://app.charmverse.io/op-grants/opti-domains-ens-l2-development-9893299892995353)
* [Received a Gitcoin Grant in the past year for the project “Opti.Domains | Scale ENS to OP”](https://explorer.gitcoin.co/#/projects/0xe084029d76ed3ac56650706b083845b0ffe786e9abb770f14c0a145381c32b2a)
* [Was the first to build a fault gateway for Optimism following its migration from L2OutputOracle to the Dispute Game mechanism](https://discuss.ens.domains/t/op-fault-proof-upgrade-break-op-verifier-and-op-gateway-implementation-in-the-evm-gateway/18973)
* [Developed a Superchain CCIP gateway with a unique “deploy-once, run-anywhere” feature](https://github.com/Opti-domains/superchain-gateway), enabling each individual domain to specify the chain and resolver from which it should be resolved without the need to deploy a dedicated verifier contract and gateway
* [Received an ENS small grant for adding custom UniversalResolver support to Wagmi](https://ensgrants.xyz/rounds/29/proposals/708) (Previously, Wagmi did not support setting a custom UniversalResolver contract)

[![image](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/95425539d7a54527bc65308b7bc8a50c90767ce9_2_690x490.jpeg)image1280×910 73.2 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/95425539d7a54527bc65308b7bc8a50c90767ce9.jpeg "image")

Opti.Domains ENS L2 is live at <https://ens.opti.domains>

Opti.Domains developer documentation is available at [GitHub - Opti-domains/opti-registry: An extendable smart contract for developer to develop creative domain name use cases on superchain](https://github.com/Opti-domains/opti-registry) and [GitHub - Opti-domains/superchain-gateway: ENS Gateway for Superchain](https://github.com/Opti-domains/superchain-gateway)

### Upnode

* [Upnode has been a mainnet validator for Celestia for more than 1 year and has received foundation delegation](https://www.mintscan.io/celestia/validators/celestiavaloper133t4gpv4vhpqgfn9gr8l4u423zrglg8rkqeupr)
* We have hosted many validators and indexers on behalf of private investors, whose identities cannot be disclosed due to confidentiality agreements.
* Upnode has successfully completed multiple Optimism grants focused on the development of developer tooling.
  + [signer-proxy](https://github.com/upnodedev/signer-proxy): An RPC signer proxy server used for signing transactions via YubiHSM2 hardware or AWS KMS signers. Used by a few OP Stack chains.
  + [UpRoll](https://uproll-web.vercel.app): OP Stack deployment tool [[Demo Video]](https://drive.google.com/file/d/1mnkTkV45UFrmchCSaCq4CYa9cz2Sdg-e/view)
  + [opstack-compose](https://github.com/upnodedev/opstack-compose): OP Stack docker compose deployment script (Superseded by UpRoll)
* Our objective is to leverage our expertise and connection in validator node operations to build and maintain a decentralized dWeb infrastructure for ENS.

---

## 6. Video Introduction (The BEST WAY to learn about our project!)

[![](https://discuss.ens.domains/uploads/db9688/original/2X/9/94de1b56905a5c9e0bedd79e77a39a480cbf0a07.jpeg "dWeb Pitch Video")](https://www.youtube.com/watch?v=TuwGLqHhJps)

---

## 7. Conflict Of Interest Statment

* Several of our projects have received grants from Optimism. One project directly related to ENS, [Opti.domains](https://ens.opti.domains), scaling ENS to OP, is funded by an OP grant. However, this proposal is not intended as double funding; rather, it aims to build a new project for dWeb infrastructure on ENS, which falls outside the scope of the OP grant.
* [Upnode](https://upnode.org) generates revenue through its validator business.

---

# Post #2 by daostrat.eth
Posted at: 2025-03-29T14:39:08.535Z

[@chomtana](/u/chomtana) gm!

Thank you for submitting your application for the ENS Service Provider Program, Season 2. **Excited to see that the application meets the four eligibility criteria outlined in the program design.**

Notes:

* Metagov will also include dWeb.host in the group endorsement vote on April 1.
* Make sure to update with the summary video link for the application prior to the timeline closing. ![:film_projector:](https://discuss.ens.domains/images/emoji/twitter/film_projector.png?v=12 ":film_projector:")

Good luck in SPP2!

---

*Metagov Stewards*

---

# Post #3 by chomtana
Posted at: 2025-03-31T00:40:22.131Z

Hi [@daostrat.eth](/u/daostrat.eth) , we have posted our introduction video. Can you check if we have now meet all eligibility criteria.

---

# Post #4 by daostrat.eth
Posted at: 2025-03-31T01:14:26.623Z

Good to go [@chomtana](/u/chomtana) !

---

