# Post #1 by lightwalker.eth
Posted at: 2025-04-01T05:10:10.449Z

[![NameHash Labs - Critical ENS Infrastructure](https://discuss.ens.domains/uploads/db9688/optimized/2X/b/b20c45235e91e3379230462ae1f3f205cd050ac3_2_690x415.jpeg)NameHash Labs - Critical ENS Infrastructure1440×868 85.2 KB](https://discuss.ens.domains/uploads/db9688/original/2X/b/b20c45235e91e3379230462ae1f3f205cd050ac3.jpeg "NameHash Labs - Critical ENS Infrastructure")

# 0. Introduction

## 0.1. Proposal Summary

[![](https://discuss.ens.domains/uploads/db9688/original/2X/b/b5b74bcf5fff6e962914b0a1628244f37a6f9d6b.jpeg "NameHash Labs - ENS Service Provider - Season 2 - Proposal")](https://www.youtube.com/watch?v=g88tCK5TECU)

[NameHash Labs](https://namehashlabs.org) is an existing ENS Service Provider with a team of 14. We are seeking a $1.1M budget from the ENS DAO to deliver key infrastructure for the ENS ecosystem.

This includes 8 substantial ENS infrastructure engineering projects, to include ENSNode, ENSAdmin, NameGraph, and NameAI to address urgent ENS infrastructure needs:

**1. Close critical ENS infrastructure gaps:**

Indexed ENS data is vital for the upcoming launch of ENSv2 and Namechain. Existing ENS indexed data providers (the ENS Subgraph) are fundamentally unsuitable for ENSv2 and a replacement is critically required for many of ENS’s most important apps, including the official ENS Manager App among many others.

**2. Strengthen the decentralization and “unstoppability” of ENS:**

Our infrastructure under development removes a strict dependency on many centralized offchain gateway servers whose downtime would otherwise shut down impacted multichain ENS names that are key to the future of ENSv2 and Namechain, such as subnames of base.eth, linea.eth, or tokenized DNS names such as .box names or 3DNS names.

**3. Deliver game-changing ENS protocol innovations:**

We are engineering radically accelerated resolution of most ENS queries. ENSNode’s architecture unlocks near-instant bulk resolution of live ENS records, including name resolution configurations that span across multiple chains. This can be contrasted with the status quo strategy that requires time-consuming routing through the multi-step CCIP-read handshake process and offchain gateway servers that are potentially centralized or potentially implement request tracking. For most ENS names, enjoy ~20 times faster ENS resolutions of *live* (not stale) ENS records with more privacy and no centralized dependencies.

**4. Support a restabilization of declining ENS DAO revenues:**

We are executing a number of infrastructure-level strategies to help boost and restabilize ENS DAO revenues to ensure the indefinite continuation of ENS protocol development.

With your approval of our $1.3M total “Extended Scope” budget (please vote us to be your #1 ranked proposal ![:pray:](https://discuss.ens.domains/images/emoji/twitter/pray.png?v=12 ":pray:")), ENS will additionally gain solutions for other urgent needs, including:

**5. Guarantee the creation of an ENS Referral Program to promote the launch of ENSv2 and Namechain with a minimum budget of $50k.**

The guarantee is simple, if our “Extended Scope” budget is approved and if the ENS DAO still has not launched a different ENS Referral Program prior to the launch of ENSv2, then upon the launch of ENSv2, we will deploy our own permissionless ENSv2 Referral Program contracts. We will fund these contracts ourselves with $50k to provide revenue sharing rewards for registrar apps that refer a minimum number of their users to make .eth registrations and renewals.

We will also invest in the creation and distribution of marketing materials, community outreach, and related “microsites” for the ENS Referral Program.

**6. Boost ENS revenue stabilization and the long-term health of the ENS DAO through a new (and much needed!) infrastructure project - ENS TokenScope:**

We will deliver infrastructure for ENS registrar apps to easily identify that a name might be taken, but could still be purchased for a fair price and to help facilitate that aftermarket transaction. This action further supports ENS DAO revenues as secondary market transactions ultimately encourages more .eth registrations and renewals.

Relatedly, we will also deliver ENS infrastructure to trace the relationship from an ENS name (including tokenized DNS names) to the specific NFT that tokenizes the ownership of the name.

ENS TokenScope closes a key vector of adoption risks for ENS vs. Namechain’s highly VC funded competitors, and supports the attraction of new DNS TLDs from the upcoming ICANN auctions to tokenize their names on Namechain.

Our team of 14 includes highly accomplished senior engineers and is delivering big for ENS.

Now we need your help.

We are 100% bootstrapped and have never raised any money from investors. The ENS Service Provider Program is crucial for us to continue supporting our team and maintaining our commitment to ENS.

We really appreciate your consideration for funding and thank you so much for your support.

## 0.2. ENS Key Infrastructure Needs

[![ENS - 3 Key Areas of Need](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/ea093c08a8e23448a7f2d0ddeed06e46a1a92760_2_690x388.jpeg)ENS - 3 Key Areas of Need3840×2160 565 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/ea093c08a8e23448a7f2d0ddeed06e46a1a92760.jpeg "ENS - 3 Key Areas of Need")

Our team is building key solutions for ENS’s 3 key areas of need:

1. Critical infrastructure gaps for ENSv2;
2. DAO financial stability; and
3. Developer enablement for more big ENS integrations.

### 0.2.1. Critical Infrastructure Gaps for ENSv2

First, and most importantly, ENSv2 has a critical unsolved infrastructure gap: indexed data.

The [ENS Subgraph](https://thegraph.com/explorer/subgraphs/5XqPmWe6gjyrJtFn9cLy237i4cWw2j9HcUJEXsP5qGtH?view=Query&chain=arbitrum-one) has been critical infrastructure for ENSv1, serving as the source of indexed ENS data. However, the Subgraph is fundamentally unsuitable for ENSv2.

[![ENS Subgraph - Fundamentally Unsuitable for ENSv2](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/e958b3d4b95edc68de563b5bcab42c1625c53bd3_2_690x388.jpeg)ENS Subgraph - Fundamentally Unsuitable for ENSv23840×2160 558 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/e958b3d4b95edc68de563b5bcab42c1625c53bd3.jpeg "ENS Subgraph - Fundamentally Unsuitable for ENSv2")

How critical is the need for indexed ENS data? There’s over 700 million / requests for it a year, and growing! And this is only for mainnet!

[![Requests for Indexed ENS Data](https://discuss.ens.domains/uploads/db9688/optimized/2X/5/534225ad6d6f92a45c3bcb3afae814d0e7e6135f_2_690x388.jpeg)Requests for Indexed ENS Data3840×2160 635 KB](https://discuss.ens.domains/uploads/db9688/original/2X/5/534225ad6d6f92a45c3bcb3afae814d0e7e6135f.jpeg "Requests for Indexed ENS Data")

Critical ENS Apps currently rely on this service, including:

The [official ENS Manager app](https://app.ens.domains/).

[![Official ENS Manager app](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/ad0109fd674c58818d56dc41dd5494c50b675ea8_2_690x388.jpeg)Official ENS Manager app3840×2160 411 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/ad0109fd674c58818d56dc41dd5494c50b675ea8.jpeg "Official ENS Manager app")

Core ENS Developer Tooling like [ENSjs](https://github.com/ensdomains/ensjs).

[![ENSjs](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/98634c9b53105fa7312c9f0946ccf22b4c85ee75_2_690x388.jpeg)ENSjs3840×2160 501 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/98634c9b53105fa7312c9f0946ccf22b4c85ee75.jpeg "ENSjs")

Wallets like [Rainbow](https://rainbow.me/).

[![Rainbow](https://discuss.ens.domains/uploads/db9688/optimized/2X/1/1b0f8944ef319202ae2bc871d6b87ae1e57a3496_2_690x388.jpeg)Rainbow3840×2160 544 KB](https://discuss.ens.domains/uploads/db9688/original/2X/1/1b0f8944ef319202ae2bc871d6b87ae1e57a3496.jpeg "Rainbow")

Marketplaces like [Vision](https://vision.io/).

[![Vision](https://discuss.ens.domains/uploads/db9688/optimized/2X/d/d45a141aba3fd7fa530ee95a19c1f65e11d056ee_2_690x388.jpeg)Vision3840×2160 580 KB](https://discuss.ens.domains/uploads/db9688/original/2X/d/d45a141aba3fd7fa530ee95a19c1f65e11d056ee.jpeg "Vision")

Chain explorers like [Blockscout](https://www.blockscout.com/).

[![Blockscout](https://discuss.ens.domains/uploads/db9688/optimized/2X/3/3d72e6715a80543e02db92cae994ce0d7075cdab_2_690x388.jpeg)Blockscout3840×2160 523 KB](https://discuss.ens.domains/uploads/db9688/original/2X/3/3d72e6715a80543e02db92cae994ce0d7075cdab.jpeg "Blockscout")

Social apps like the [Ethereum Follow Protocol](https://efp.app/).

[![EFP](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/a4fff91b5cd84e33100df1e1da9d7f3073e82215_2_690x388.jpeg)EFP3840×2160 583 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/a4fff91b5cd84e33100df1e1da9d7f3073e82215.jpeg "EFP")

… and many other key platforms that form the ENS ecosystem, including:

[![Many other platforms in ENS](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/95bc4a6e4e7ddecc6e25c6aab94df67dbe4580b3_2_690x388.jpeg)Many other platforms in ENS3840×2160 350 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/95bc4a6e4e7ddecc6e25c6aab94df67dbe4580b3.jpeg "Many other platforms in ENS")

As you can see, indexed data is key to the ENS protocol.

However, even for ENSv1, a strong argument can be made that the Subgraph is already unsuitable. Data for 90% of ENS names is already missing in the Subgraph!

[![Lost ENS Names](https://discuss.ens.domains/uploads/db9688/optimized/2X/7/7b86f2c4d6186abbea64936f7534658a4d34e5f0_2_690x388.jpeg)Lost ENS Names3840×2160 532 KB](https://discuss.ens.domains/uploads/db9688/original/2X/7/7b86f2c4d6186abbea64936f7534658a4d34e5f0.jpeg "Lost ENS Names")

The Subgraph has many big problems. Chief among those: the Subgraph is single-chain only.

Let’s make some practical examples. Because the Subgraph is single-chain only, this means for over 90% of ENS names it’s not currently possible to answer fundamental questions like:

What are all the names owned by this address?

[![Lost Name Example](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/4907a873425c012d8f52d1b3a2cad52e427977c5_2_690x388.jpeg)Lost Name Example3840×2160 487 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/4907a873425c012d8f52d1b3a2cad52e427977c5.jpeg "Lost Name Example")

Or, what are all the social records / chain addresses set on this name?

[![Lost Profile Records Example](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/927c46d421da9963837787546db6f591caeff09f_2_690x388.jpeg)Lost Profile Records Example3840×2160 480 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/927c46d421da9963837787546db6f591caeff09f.jpeg "Lost Profile Records Example")

This data *is* currently available only for mainnet, which is why you may not have noticed the problem yet.

But ENS is multichain, and ENS is offchain, too! 90% of ENS names are already issued off of mainnet, this includes base.eth subnames on Base, linea.eth subnames on Linea, and offchain subnames including uni.eth, cb.id, and many more.

And crucially, what happens with ENSv2? For ENSv1 the Subgraph at least is working for direct subnames of .eth on mainnet.

[![ENSv2 Launch Impact](https://discuss.ens.domains/uploads/db9688/optimized/2X/6/62dec85280203f5e4de20971aeacd389d670f131_2_690x388.jpeg)ENSv2 Launch Impact3840×2160 329 KB](https://discuss.ens.domains/uploads/db9688/original/2X/6/62dec85280203f5e4de20971aeacd389d670f131.jpeg "ENSv2 Launch Impact")

However, when ENSv2 launches, direct subnames of .eth are transitioning off of mainnet to Namechain.

[![ENSv2 Launch Impact](https://discuss.ens.domains/uploads/db9688/optimized/2X/5/541d7755219a267b243357cf644fc084f3705ac5_2_690x388.jpeg)ENSv2 Launch Impact3840×2160 405 KB](https://discuss.ens.domains/uploads/db9688/original/2X/5/541d7755219a267b243357cf644fc084f3705ac5.jpeg "ENSv2 Launch Impact")

![:fire:](https://discuss.ens.domains/images/emoji/twitter/fire.png?v=12 ":fire:") The limitations of the Subgraph are critical.

Key limitations include being single-chain only. ENS is already 90% multichain, the key exception has been .eth on mainnet. However with ENSv2, even .eth is becoming multichain!

![:star:](https://discuss.ens.domains/images/emoji/twitter/star.png?v=12 ":star:") We need to ensure ENSv2 launches with a strong data indexing solution!

### 0.2.2. DAO Financial Stability

ENS is blessed to have a meaningful financial runway saved in reserves. However, we should take note:

![:fire:](https://discuss.ens.domains/images/emoji/twitter/fire.png?v=12 ":fire:") ENS Revenues are trending downward.

The ENS DAO [daily revenues graph from Steakhouse](https://dune.com/steakhouse/ens-steakhouse) show a concerning trend that would be unwise to dismiss.

[![Declining revenues](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/47473c5b799c1eeec26d98af3befb1426790ff94_2_690x302.png)Declining revenues1262×554 39.4 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/47473c5b799c1eeec26d98af3befb1426790ff94.png "Declining revenues")

DAO Revenues originate from .eth registrations and renewals.The [historical active .eth graph from Makoto](https://dune.com/makoto/historical-active-eth) shows this critical metric for ENS dropping over time.

[![Declining registrations](https://discuss.ens.domains/uploads/db9688/optimized/2X/b/b661bad65e3119b15595665de92ad9abf5e78b8a_2_690x234.png)Declining registrations1030×350 20 KB](https://discuss.ens.domains/uploads/db9688/original/2X/b/b661bad65e3119b15595665de92ad9abf5e78b8a.png "Declining registrations")

Growing subnames in general is good for ENS, but only direct subnames of .eth produce revenue for the ENS DAO.

![:star:](https://discuss.ens.domains/images/emoji/twitter/star.png?v=12 ":star:") We need .eth registrations and renewals to be healthy and growing (or at least stable)!

### 0.2.3. Developer Enablement for ENS Integrations

ENS provides powerful capabilities, but some developers experience challenges with integrations.

![:fire:](https://discuss.ens.domains/images/emoji/twitter/fire.png?v=12 ":fire:") A number of ENS integrations fail to support all ENS names, use cases, or best practices.

A number of operations in the ENS protocol require special care to implement correctly. A lot of documentation may already exist, but that doesn’t mean developers are correctly reading the docs in full. For important use cases it can be a lot of work to correctly understand, implement, and test. This ultimately is resulting in fewer ENS integrations, or flawed ENS integrations that lead to bad ENS user experiences.

![:star:](https://discuss.ens.domains/images/emoji/twitter/star.png?v=12 ":star:") We need to enable developers to more easily build optimal ENS integrations.

## 0.3. Strategy Overview

The following table outlines the relationship between ENS’s 3 key needs, our solutions, and funding of the basic vs extended proposal scope:

[![Strategy Overview](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/408efe0e282c91ca57cf351b3a6773b205bbc267_2_690x401.png)Strategy Overview1806×1052 95.5 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/408efe0e282c91ca57cf351b3a6773b205bbc267.png "Strategy Overview")

## 0.4. Our ENS Infrastructure Solutions

To service ENS’s 3 key needs, our team is building 8 key ENS infrastructure projects:

[![8 Key ENS Infrastructure Solutions](https://discuss.ens.domains/uploads/db9688/optimized/2X/3/39c48c273c75c9d6ba6ade55690388197efa7e3e_2_690x388.jpeg)8 Key ENS Infrastructure Solutions3840×2160 780 KB](https://discuss.ens.domains/uploads/db9688/original/2X/3/39c48c273c75c9d6ba6ade55690388197efa7e3e.jpeg "8 Key ENS Infrastructure Solutions")

These eight ENS infrastructure projects work together to address the critical needs of ENSv2, enhance DAO financial stability through increased registrations and renewals, and support developers to build more big ENS integrations.

### 0.4.1. ENSNode

[![ENSNode](https://discuss.ens.domains/uploads/db9688/optimized/2X/5/5a0568675d98ac8ac60409fc2ede877c0f02d599_2_690x323.png)ENSNode1216×570 174 KB](https://discuss.ens.domains/uploads/db9688/original/2X/5/5a0568675d98ac8ac60409fc2ede877c0f02d599.png "ENSNode")

* Product Webpage
  + [ENSNode](https://ensnode.io/)
* Infrastructure Summary
  + ENSNode is the new multichain ENS indexer for ENS and ENSv2.
  + ENSNode builds on [Ponder](https://ponder.sh/). Ponder’s powerful open source framework enables many of the key ENS indexing innovations in ENSNode.
* Strategic Goals
  + Fill critical ENS infrastructure gaps for ENSv2.
  + ENS developer enablement.
* Selected Key Benefits
  + **Close critical ENS infrastructure gaps:**
    - Indexed ENS data is vital for the upcoming launch of ENSv2 and Namechain. Existing ENS indexed data providers (the ENS Subgraph) are fundamentally unsuitable for ENSv2 and a replacement is critically required for many of ENS’s most important apps, including the official ENS Manager App among many others.
  + **Strengthen the decentralization and “unstoppability” of ENS:**
    - Our infrastructure under development removes a strict dependency on many centralized offchain gateway servers whose downtime would otherwise shut down impacted multichain ENS names that are key to the future of ENSv2 and Namechain, such as subnames of base.eth, linea.eth, or tokenized DNS names such as .box names or 3DNS names.
  + **Deliver game-changing ENS protocol innovations:**
    - We are engineering radically accelerated resolution of most ENS queries. ENSNode’s architecture unlocks near-instant bulk resolution of live ENS records, including name resolution configurations that span across multiple chains. This can be contrasted with the status quo strategy that requires time-consuming routing through the multi-step CCIP-read handshake process and offchain gateway servers that are potentially centralized or potentially implement request tracking. For most ENS names enjoy ~20 times faster ENS resolutions of *live* (not stale) ENS records with more privacy and no centralized dependencies.

[![ENSNode Roadmap Summary](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/84b89725ec8615bb164ee4ce6d81408debf6c9d9_2_690x388.jpeg)ENSNode Roadmap Summary3840×2160 608 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/84b89725ec8615bb164ee4ce6d81408debf6c9d9.jpeg "ENSNode Roadmap Summary")

* Key Metrics / User Traction / Successful Deployments and Integrations
  + Indexes 100% of base.eth subnames on Base.
  + Indexes 100% of linea.eth subnames on Linea.
  + ENSNode is verified to pass 100% backwards compatibility with the ENS Subgraph to streamline adoption.
  + 10x faster than the ENS Subgraph.
  + 35x more efficient than the ENS Subgraph.
  + Passes 100% of ens-test-env tests.
  + ENS Labs is currently reviewing switching the ens-test-env from using the ENS Subgraph to using ENSNode.
* Additional Links
  + [GitHub](https://github.com/namehash/ensnode)
  + [Docs](https://ensnode.io/ensnode/)
  + [ENS Subgraph Transition Tools](https://github.com/namehash/ens-subgraph-transition-tools)
  + [ens-test-env fork passing all tests after replacing ENS Subgraph with ENSNode](https://github.com/namehash/ens-test-env)
  + [ensjs fork passing all tests after replacing ENS Subgraph with ENSNode](https://github.com/namehash/ensjs)
  + [ens-deployments](https://github.com/namehash/ensnode/tree/main/packages/ens-deployments)
  + [ponder-subgraph-api](https://github.com/namehash/ensnode/tree/main/packages/ponder-subgraph-api)
  + [Hosted Instances](https://ensnode.io/ensnode/usage/hosted-ensnode-instances/)

### 0.4.2. ENSRainbow

[![ENSRainbow](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/acda2196f33d128e96c386ac940db4e154e72c93_2_690x268.png)ENSRainbow1216×474 63.8 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/acda2196f33d128e96c386ac940db4e154e72c93.png "ENSRainbow")

* Product Webpage
  
  + [ENSRainbow](https://ensrainbow.io/)
* Infrastructure Summary
  
  + Heal millions of unknown ENS names with this ENSNode sidecar service.
* Strategic Goals
  
  + Fill critical ENS infrastructure gaps for ENSv2.
  + ENS developer enablement.
* Selected Key Benefits
  
  + Reduce ENS’s UX / DX complexity:
    - The ENS community has better things to do than learn about technical complexities like unknown names or encoded labelhashes.
* Key Metrics / User Traction / Successful Deployments and Integrations

[![Name Healing Coverage](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/8688cedc0e7a0e85689c5536ec8b2a4cc787c9ff_2_690x493.jpeg)Name Healing Coverage1280×916 96.2 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/8688cedc0e7a0e85689c5536ec8b2a4cc787c9ff.jpeg "Name Healing Coverage")

[![Healable Labels](https://discuss.ens.domains/uploads/db9688/optimized/2X/f/f3b8a2d5d0edc9dd91011778f0e358b9ecfb67e5_2_690x172.png)Healable Labels1510×378 24.3 KB](https://discuss.ens.domains/uploads/db9688/original/2X/f/f3b8a2d5d0edc9dd91011778f0e358b9ecfb67e5.png "Healable Labels")

* Additional Links
  + [GitHub](https://github.com/namehash/ensnode/tree/main/apps/ensrainbow)
  + [Docs](https://ensnode.io/ensrainbow/)
  + [ens-rainbow-sdk](https://github.com/namehash/ensnode/tree/main/packages/ensrainbow-sdk)

### 0.4.3. ENSAdmin

[![ENSAdmin](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/8f525193e73007c6ece8f05e3d8a85fb02ba6526_2_690x268.png)ENSAdmin1216×474 61.9 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/8f525193e73007c6ece8f05e3d8a85fb02ba6526.png "ENSAdmin")

* Product Webpage
  
  + [ENSAdmin](https://admin.ensnode.io/)
* Infrastructure Summary
  
  + Explore the ENS Protocol like never before.
* Strategic Goals
  
  + ENS developer enablement.
* Selected Key Benefits
  
  + Interactively learn and debug how ENS Registries, Registrars, Resolvers, Gateways, and Clients interact.  
    
    [![ENS Protocol Inspector](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/8fc527f1193b137cfd263ce0f96d301a7dda42e4_2_510x500.png)ENS Protocol Inspector2556×2504 478 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/8fc527f1193b137cfd263ce0f96d301a7dda42e4.png "ENS Protocol Inspector")
  + Monitor multichain indexing status of a connected ENSNode instance[![ENSNode Monitoring](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/ed64742d86c42d0d752a0e3a9947a692aab58595_2_551x500.png)ENSNode Monitoring2556×2318 391 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/ed64742d86c42d0d752a0e3a9947a692aab58595.png "ENSNode Monitoring")
  + Connect to any ENSNode instance  
    
    [![ENSNode Connections](https://discuss.ens.domains/uploads/db9688/optimized/2X/d/d91b33e5a079f8f9dbdf08eeee8116df24bf1abe_2_690x308.png)ENSNode Connections1138×508 57.9 KB](https://discuss.ens.domains/uploads/db9688/original/2X/d/d91b33e5a079f8f9dbdf08eeee8116df24bf1abe.png "ENSNode Connections")
  + Interactively preview ENSNode APIs  
    
    [![ENSNode APIs](https://discuss.ens.domains/uploads/db9688/optimized/2X/f/f796a923f77d40d7fd28392e3fce24cfb42df76a_2_690x432.png)ENSNode APIs2552×1600 470 KB](https://discuss.ens.domains/uploads/db9688/original/2X/f/f796a923f77d40d7fd28392e3fce24cfb42df76a.png "ENSNode APIs")
* Additional Links
  
  + [GitHub](https://github.com/namehash/ensnode/tree/main/apps/ensadmin)
  + [Docs](https://ensnode.io/ensadmin/)

### 0.4.4. ENSv2 Referral Programs

[![ENSv2 Referral Programs](https://discuss.ens.domains/uploads/db9688/optimized/2X/b/b0617c8a08a4eacfe0105e3cb242ef6b877a848a_2_690x268.png)ENSv2 Referral Programs1216×474 100 KB](https://discuss.ens.domains/uploads/db9688/original/2X/b/b0617c8a08a4eacfe0105e3cb242ef6b877a848a.png "ENSv2 Referral Programs")

* Product Webpage
  + [ENSv2 Referral Programs](https://namehashlabs.org/ens-v2-referral-programs)
* Infrastructure Summary
  + Smart contracts for implementing an ENS Referral Program on ENSv2.
* Strategic Goals
  + DAO financial stability.
  + ENS developer enablement.
* Selected Key Benefits
  + Incentivize platforms with large existing audiences to integrate and promote .eth registrations and renewals.
  + Permissionless. Not only to participate as a referrer, but also to create and fund.
  + Enables any number of ENSv2 Referral Programs to be created. Each can define their own rules for what qualifies for a reward, how rewards are scored, how they are withdrawn, etc…
  + Mitigates previously voiced concerns of theoretical referral program uncertainties through support for optional finite-lifespan referral program strategies that constrain any “blast radius” of unintended side effects. Let’s try, learn, and iterate with improvements!
  + Compatible with the ENSv2 contracts ENS Labs has open sourced.
* Additional Links
  + [GitHub](https://github.com/namehash/ens-v2-referral-programs)

### 0.4.5. NameGraph

[![NameGraph](https://discuss.ens.domains/uploads/db9688/optimized/2X/c/cdaee467fea0c74a9e8c53251aa5e221795fe02c_2_690x268.png)NameGraph1216×474 173 KB](https://discuss.ens.domains/uploads/db9688/original/2X/c/cdaee467fea0c74a9e8c53251aa5e221795fe02c.png "NameGraph")

* Product Webpage
  + [NameGraph](https://www.namegraph.dev/)
* Infrastructure Summary
  + NameGraph helps name collectors find collectable names they love.
  + Name discovery algorithms build on NameAI and NameGuard.
* Strategic Goals
  + DAO financial stability.
  + ENS developer enablement.
* Selected Key Benefits
  + The most powerful discovery engine for collectable names ever created: Processes inputs through multiple interpretations and tokenizations
  + World’s largest knowledge graph of names: 400,000+ curated collections with 21+ million unique names
  + Social, cultural, addictive, and fun! The initial release of NameGraph doesn’t include support to add or customize your own collections yet. But capabilities for this are in the roadmap, including some special strategies to ensure collections are high quality and don’t become polluted with abuse or low quality content. So over time the collections will fill out and become even stronger!
  + Fast and easy integration.
  + Note: The following screenshots are from the NameGraph “developer demo” app. This app is intended to inspire developers with features they can build into their own apps using NameGraph. The “developer demo” app is not intended for direct consumer use (although it’s pretty fun)!
  + Powerful search across more than 400,000 name collections  
    
    [![Collection Search](https://discuss.ens.domains/uploads/db9688/optimized/2X/3/352a159ef5bc7577b191e9e8a0d8558c14dc15cf_2_564x500.png)Collection Search1316×1165 139 KB](https://discuss.ens.domains/uploads/db9688/original/2X/3/352a159ef5bc7577b191e9e8a0d8558c14dc15cf.png "Collection Search")
  + View details of a collection in the NameGraph  
    
    [![Collection Details](https://discuss.ens.domains/uploads/db9688/optimized/2X/b/b30badbe0f58a5a92bb10c6eecfb70b0ec344e74_2_559x500.png)Collection Details1308×1169 171 KB](https://discuss.ens.domains/uploads/db9688/original/2X/b/b30badbe0f58a5a92bb10c6eecfb70b0ec344e74.png "Collection Details")
  + View details of a name in the NameGraph  
    
    [![Name Details](https://discuss.ens.domains/uploads/db9688/optimized/2X/3/373bb9e9b51eb9a26c3ce6ae0ff73e47aab461e5_2_564x500.jpeg)Name Details1316×1165 159 KB](https://discuss.ens.domains/uploads/db9688/original/2X/3/373bb9e9b51eb9a26c3ce6ae0ff73e47aab461e5.jpeg "Name Details")
  + Recursively navigate curiously related ideas in the NameGraph  
    
    [![Recursive Exploration](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/a9f01b758444bf7568e948d75c37ffde2392729b_2_557x500.png)Recursive Exploration1296×1163 165 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/a9f01b758444bf7568e948d75c37ffde2392729b.png "Recursive Exploration")
  + Supports any parent name  
    
    [![Support Any Parent](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/a6246eab37a67205b9c7175c20308f5bdec88bc1_2_415x499.png)Support Any Parent578×696 24.3 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/a6246eab37a67205b9c7175c20308f5bdec88bc1.png "Support Any Parent")
  + Explore endless fun!  
    
    [![Fun Example 1](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/4cffc91c592676c1e89cc91d09409f8680e019a1_2_544x500.jpeg)Fun Example 11269×1166 210 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/4cffc91c592676c1e89cc91d09409f8680e019a1.jpeg "Fun Example 1")  
    
    [![Fun Example 2](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/98aaae496cf2fb54ecf74ebfbb922738e9bd7013_2_544x500.png)Fun Example 21271×1167 174 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/98aaae496cf2fb54ecf74ebfbb922738e9bd7013.png "Fun Example 2")  
    
    [![Fun Example 3](https://discuss.ens.domains/uploads/db9688/optimized/2X/7/7ba7434a1d82da9fd4a9b875bf97839efba6d154_2_553x500.png)Fun Example 31288×1163 172 KB](https://discuss.ens.domains/uploads/db9688/original/2X/7/7ba7434a1d82da9fd4a9b875bf97839efba6d154.png "Fun Example 3")  
    
    [![Fun Example 4](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/4f460725ee438f12b83772651f26725ee63252d5_2_553x499.png)Fun Example 41285×1160 120 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/4f460725ee438f12b83772651f26725ee63252d5.png "Fun Example 4")
* Key Metrics / User Traction / Successful Deployments and Integrations
  + Public launch on 20 March 2025
  + [Vision already launched an initial integration.](https://x.com/ensvision/status/1902711055802933619) Additional integrations under development.
  + Annualized user request volume: 3,000,000 requests / year (only 10 days since launch!)
* Additional Links
  + [NameGraph collection building data pipeline](https://github.com/namehash/namegraph-collections)
    - [Engineering background info on the pipeline](https://github.com/namehash/namegraph-collections/blob/master/docs/readme-internal.md)
  + [NameGraph backend service](https://github.com/namehash/namegraph)
    - We host an instance of NameGraph that’s freely available for you or anyone in the community to make use of at api.namegraph.dev.
  + [API Docs](https://api.namegraph.dev/docs)
  + [NameGraph TypeScript SDK](https://github.com/namehash/namekit/tree/main/packages/namegraph-sdk)
  + [NameGraph Developer Demo App](https://github.com/namehash/namekit/tree/main/apps/namegraph.dev)

### 0.4.6. NameAI

[![NameAI](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/4360eeb1c214fb2f891832136c22f6d59ae23635_2_690x268.png)NameAI1216×474 320 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/4360eeb1c214fb2f891832136c22f6d59ae23635.png "NameAI")

* Product Webpage
  + [NameAI](https://www.nameai.io/)
* Infrastructure Summary
  + Building on NameGuard, NameAI enables sophisticated multi-dimensional scoring for ENS names, helping ENS marketplace apps automatically sort the most attractive names to the top. Through advanced tokenization and analysis techniques, NameAI evaluates all possible ENS names across various attributes to effectively approximate their overall attractiveness, making it easier for name collectors to find and collect more names they love.
* Strategic Goals
  + DAO Financial Stability
  + Developer Enablement
* Selected Key Benefits
  + Multi-dimensional Name Scoring: Customize name scoring strategies that are optimized for your community.
  + Advanced Tokenization: Probabilistic parsing of name components into recognized words. Filter names by word-count.
  + Fast and easy integration: even small teams can now offer sophisticated name discovery features, fostering innovation throughout the ecosystem.
* Key Metrics / User Traction / Successful Deployments and Integrations
  + Public launch on February 20, 2025
  + [Vision already launched an initial integration](https://docs.vision.io/profile-features/vision-score-beta) (branded as VisionScore). Additional integrations under development.
  + Over 40,000,000 requests since launch!
* Additional Links
  + [Server](https://github.com/namehash/namekit/tree/main/apps/api.nameai.io)
  + [TypeScript SDK](https://github.com/namehash/namekit/tree/main/packages/nameai-sdk)
  + [API Docs](https://api.nameai.io/docs)
  + [Dev Demo App](https://github.com/namehash/namekit/tree/main/apps/nameai.io)

### 0.4.7. NameGuard

[![NameGuard](https://discuss.ens.domains/uploads/db9688/optimized/2X/2/234be9313229ca594abd230e9ed98fa8cb1c2966_2_690x268.png)NameGuard1216×474 102 KB](https://discuss.ens.domains/uploads/db9688/original/2X/2/234be9313229ca594abd230e9ed98fa8cb1c2966.png "NameGuard")

* Product Webpage
  + [NameGuard](https://www.nameguard.io/)
* Infrastructure Summary
  + NameGuard provides comprehensive security analysis for ENS names, identifying and preventing malicious use through advanced detection systems. It creates a safer environment for ENS users by detecting potential security risks, impersonation attempts, and usability issues in ENS names, addressing the “sharp edges” that could lead to unexpected or harmful consequences. Currently being rearchitected to leverage ENSNode services, NameGuard will deliver improved analysis capabilities while transitioning core logic to TypeScript for broader application integration.
* Strategic Goals
  + Developer Enablement
* Selected Key Benefits
  + Multi-level Protection: Comprehensive security checks across various dimensions
  + Impersonation Detection: Identifies names attempting to mimic legitimate ENS names
  + Confusable Character Analysis: Detects visually similar characters that could be used to deceive
  + Internationalization Checks: Assesses accessibility across language barriers
  + Unified Rating System: Clear Pass/Warn/Fail classifications for security issues
  + Key Metrics / User Traction / Successful Deployments and Integrations
  + Foundation for NameAI, which has already received 40,000,000 requests since launch
* Additional Links
  + [nameguard-js](https://github.com/namehash/namekit/tree/main/packages/nameguard-js)
  + [nameguard-python](https://github.com/namehash/namekit/tree/main/packages/nameguard-python)
  + [nameguard-react](https://github.com/namehash/namekit/tree/main/packages/nameguard-react)
  + [nameguard-sdk](https://github.com/namehash/namekit/tree/main/packages/nameguard-sdk)
  + [API docs](https://api.nameguard.io/docs)
  + [Dev demo app](https://github.com/namehash/namekit/tree/main/apps/nameguard.io)

### 0.4.8. NameKit

[![NameKit](https://discuss.ens.domains/uploads/db9688/optimized/2X/d/d1a655b50113a4ee5451866c07ddbe44dbb1e0a7_2_690x268.png)NameKit1216×474 161 KB](https://discuss.ens.domains/uploads/db9688/original/2X/d/d1a655b50113a4ee5451866c07ddbe44dbb1e0a7.png "NameKit")

* Product Webpage
  + [NameKit](https://www.namekit.io/)
* Infrastructure Summary
  + NameKit is a developer toolkit that aims to make ENS onboarding fun and easy.
  + Major ENSv2 rearchitecture in progress. NameKit will build for ENSv2 using ENSNode.
  + The vision is to provide developers with tools to easily integrate rich ENS user journeys into wallets, apps, and games. Currently focused on core ENS functionality, NameKit offers a suite of packages including React components, TypeScript utilities, and contract templates that simplify ENS integration.
* Strategic Goals
  + DAO Financial Stability
  + Developer Enablement
* Additional Links
  + [Github](https://github.com/namehash/namekit)
  + [namekit-react](https://github.com/namehash/namekit/blob/main/packages/namekit-react)
  + [Namekit-contracts](https://github.com/namehash/namekit-contracts)
  + [Alpha](https://alpha.namekit.io/)

# 1. Applicant Information

## 1.1. Company Name

NameHash Labs

## 1.2. Websites

Our company

* [NameHash Labs](https://namehashlabs.org/)

Our 8 key ENS infrastructure products

1. [ENSNode](https://ensnode.io/)
2. [ENSRainbow](https://ensrainbow.io/)
3. [ENSAdmin](https://admin.ensnode.io/)
4. [ENSv2 Referral Programs](https://namehashlabs.org/ens-v2-referral-programs)
5. [NameGraph](https://www.namegraph.dev/)
6. [NameAI](https://www.nameai.io/)
7. [NameGuard](https://www.nameguard.io/)
8. [NameKit](https://www.namekit.io/)

## 1.3. Company ENS Name

[namehashlabs.eth](https://app.ens.domains/namehashlabs.eth)

## 1.4. Primary Contacts

[lightwalker.eth](https://app.ens.domains/lightwalker.eth) and [caldonia.eth](https://app.ens.domains/caldonia.eth).

## 1.5. Company Overview

[![Helping ENS Grow](https://discuss.ens.domains/uploads/db9688/optimized/2X/7/7d1d9a768c1dea2e9e458fc8b138b3c43087342a_2_690x440.jpeg)Helping ENS Grow1323×845 77.1 KB](https://discuss.ens.domains/uploads/db9688/original/2X/7/7d1d9a768c1dea2e9e458fc8b138b3c43087342a.jpeg "Helping ENS Grow")

Founded in 2022, NameHash Labs is dedicated to developing open source infrastructure to support the global adoption of ENS.

We are honored to be an existing ENS Service Provider. Thank you for your trust and for the opportunity.

[![Our Supporters](https://discuss.ens.domains/uploads/db9688/optimized/2X/5/51d27d3d8df585b60ae540d671f3cbe737dfd38b_2_690x388.jpeg)Our Supporters3840×2160 510 KB](https://discuss.ens.domains/uploads/db9688/original/2X/5/51d27d3d8df585b60ae540d671f3cbe737dfd38b.jpeg "Our Supporters")

Our team’s expertise has matured a lot this past year. We’re now in discussions with ENS Labs for taking the lead on some of the key ENS infrastructure responsibilities for ENSv2.

As we continue to mature, with the support of the DAO and ENS Labs, we aim towards one day qualifying to “graduate” from the ENS Service Provider program. As the ENS ecosystem matures, our evolution demonstrates the success of the ENS Service Provider Program’s ability to foster organizations capable of maintaining and advancing critical components of the protocol alongside ENS Labs.

## 1.6. Requested Budget

NameHash Labs is applying for a 2-year funding stream, in addition to the 1-year stream option. Please see section 4 (Scope of Work & Budget) below for details.

## 1.7. Team

[![Our Team](https://discuss.ens.domains/uploads/db9688/optimized/2X/e/eb13fd834e10712c3d78f96ae5e9f551fefb997f_2_690x496.jpeg)Our Team1314×946 210 KB](https://discuss.ens.domains/uploads/db9688/original/2X/e/eb13fd834e10712c3d78f96ae5e9f551fefb997f.jpeg "Our Team")

Our team of 14 passionate “ENS wizards” includes:

* Seasoned founders, with more than 20 years experience building innovative technology organizations.
* Former OpenZeppelin maintainers, co-authors of ERC-1271, and auditors of ERCs such as ERC-721 and ERC-1155 (yes, those massively influential NFT standards!).
* Experts in AI and Natural Language Processing (NLP) who have won numerous international awards. Their expertise helps drive forward key ENS infrastructure such as NameGraph, NameAI, and NameGuard that help ENS grow.
* Software engineers with extensive background in smart contracts, blockchain indexing, and tokenization protocol standards.
* Developer relations (DevRel) engineers with broad experience growing developer ecosystems.
* UX/UI designers with over a decade’s experience crafting beautiful products with strong usability.
* … and many more talented engineers with years of experience and dedication building for ENS!

Additional details on our team can be found near the bottom of [our homepage](https://namehashlabs.org).

# 2. Eligibility Confirmation

## 2.1. Company Age

NameHash Labs was established in 2022.

See section 1.5 (Company Overview) above for more information about our company.

## 2.2. Team Experience

NameHash Labs has exclusively focused on building ENS infrastructure and products for more than 3 years. Our general blockchain and software development experience goes far deeper.

See section 1.7 (Team) above for more details on our experience.

## 2.3. ENS Token Endorsement

Nick Johnson (nick.eth) has confirmed with us that he will be endorsing our proposal.

## 2.4. OFAC Sanctions Compliance

We, NameHash Labs, confirm that neither our organization nor any of our employees, contractors, or executive leadership is located in, or a resident of, an OFAC-sanctioned country. We further confirm that none of our business resources are derived from or routed through any country or entity that is subject to sanctions imposed by the United States (OFAC) or equivalent regulatory bodies. We pledge to remain compliant with all applicable sanctions laws and will promptly notify the ENS DAO if our status changes.

## 2.5. Multi-Year Stream Eligibility

NameHash Labs is a [Season 1 ENS Service Provider](https://discuss.ens.domains/t/service-provider-stream-nomination-thread/18142/39) applying for a multi-year stream in Season 2.

See section 0.4 (Our ENS Infrastructure Solutions) above for more details on our Season 1 work.

# 3. Open Source Commitment

We commit to our work as an ENS Service Provider being open sourced and MIT licensed in [our GitHub](https://github.com/namehash).

# 4. Scope of Work & Budget

Please see the next post in this thread for our detailed scope of work & budget. The forum doesn’t support enough characters to fit into a single post.

# 5. Additional Information

Please refer to section 0.4 (Our ENS Infrastructure Solutions) above for info on our 8 key ENS infrastructure projects, including key metrics, user traction, successful deployments and integrations, links to GitHub repositories, websites, and more.

## 5.1. Outreach for ENS Growth

Our team has been active on the broader Ethereum conference circuit. We’ve participated in many global events to help represent ENS and advocate for it within the broader ecosystem, including:

* DevCon Bogota
* ETHGlobal NYC
* ETHGlobal London
* DevConnect Istanbul
* DevCon Bangkok (including frENSday)
* ETHDenver (2024 & 2025)
* EthCC
* ETHDubai
* deBasel Miami
* SmartCon Barcelona
* ETHGlobal SF

We look forward to continuing to engage with the community and support the promotion of ENS at more global events over the coming years.

## 5.2. Testimonials

Our team is honored to have received a number of testimonials within the ENS community, including the following:

[![Testimonial - nick.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/4/45937b058dea3ee6d9515f80ecd236058bbadb12_2_690x243.png)Testimonial - nick.eth1028×363 64.1 KB](https://discuss.ens.domains/uploads/db9688/original/2X/4/45937b058dea3ee6d9515f80ecd236058bbadb12.png "Testimonial - nick.eth")  

[![Testimonial - coltron.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/6/653f26abdd046359138285bba77e7eeb18e53898_2_690x244.png)Testimonial - coltron.eth1049×372 69.8 KB](https://discuss.ens.domains/uploads/db9688/original/2X/6/653f26abdd046359138285bba77e7eeb18e53898.png "Testimonial - coltron.eth")[![Testimonial - brantly.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/5/51dfb07e400f43bcc73a060778793b6b1cfd6a2b_2_690x242.png)Testimonial - brantly.eth1061×373 63.6 KB](https://discuss.ens.domains/uploads/db9688/original/2X/5/51dfb07e400f43bcc73a060778793b6b1cfd6a2b.png "Testimonial - brantly.eth")[![Testimonial - avsa.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/a/a32253968335c3829633bd7fd383f86b02a9229a_2_690x240.png)Testimonial - avsa.eth1050×366 73.7 KB](https://discuss.ens.domains/uploads/db9688/original/2X/a/a32253968335c3829633bd7fd383f86b02a9229a.png "Testimonial - avsa.eth")[![Testimonial - simona.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/9/92bafcdc25eadbe8949f11a96b340580c11fb225_2_690x245.png)Testimonial - simona.eth1039×369 64.3 KB](https://discuss.ens.domains/uploads/db9688/original/2X/9/92bafcdc25eadbe8949f11a96b340580c11fb225.png "Testimonial - simona.eth")[![Testimonial - matoken.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/c/cf169a9f58670e08eda1413e73abb4b7beb6e0ee_2_690x181.png)Testimonial - matoken.eth1079×284 52.1 KB](https://discuss.ens.domains/uploads/db9688/original/2X/c/cf169a9f58670e08eda1413e73abb4b7beb6e0ee.png "Testimonial - matoken.eth")  

[![Testimonial - james.eth](https://discuss.ens.domains/uploads/db9688/optimized/2X/8/8f104d6d6a9a3990e10737678ba22d4d299054ad_2_690x240.png)Testimonial - james.eth1056×368 58.2 KB](https://discuss.ens.domains/uploads/db9688/original/2X/8/8f104d6d6a9a3990e10737678ba22d4d299054ad.png "Testimonial - james.eth")

# 6. Video Introduction

Please see the video at the top of this post in section 0.1 (Proposal Summary) above.

# 7. Conflict of Interest Statement

We have no conflicts of interest.

---

# Post #2 by lightwalker.eth
Posted at: 2025-04-01T05:11:19.623Z

*(continued from first post above, the forum doesn’t support so many characters in a single post)*

# 4. Scope of Work & Budget

The budget for our “basic” scope of work is: $1.1M.

The budget for our “extended” scope of work is an additional $200k, for $1.3M (total).

We take the responsibilities in this proposal with great care. The “basic” scope is the minimum budget required to properly advance our 8 key ENS infrastructure projects over the coming year. The “extended” scope budget is recommended as it provides a high ROI for ENS.

These budgets align with our team taking a significant load of responsibility for ENS infrastructure development. This includes substantial engineering projects that are not only critical to the successful launch of ENSv2 and Namechain, but also deliver fundamental innovations for how future applications integrate with ENS and perform ENS lookups and resolution.

The budget for this scope of work represents the ENS DAO making an important investment into advancing valuable ENS infrastructure. Several of our ENS infrastructure projects are working to restoratively boost ENS DAO revenues and contribute back to the long-term financial sustainability of ENS. We hope that for every $1 the DAO invests in our team, we return multiples of that as direct revenue back to the DAO in the future.

100% of this budget is devoted to supporting our mission to help ENS grow. Outside of relatively minor overhead costs and hosting expenses, all of this budget goes to supporting the salaries of our 14 existing team members and the recruitment of additional super talented full-time engineers who will dedicate themselves to building up the ENS protocol and ENS infrastructure.

This budget will enable us to further expand our engineering capacity, adding more full-time engineers to tackle the substantial infrastructure responsibilities outlined in this proposal.

Our KPIs for each quarter are to deliver a minimum of 90%+ of that quarter’s total Target Deliverables within the quarter.

At the conclusion of each quarter, we will publish a quarterly report summarizing our delivery for the quarter to the ENS DAO.

We want to ensure we’re always doing our best to maximize value creation for ENS. The ENS Ecosystem evolves quickly. A quarter, and especially a year is a long time in the web3 world. If opportunities are identified for higher-value Target Deliverables over the duration of this proposal, we reserve the right to replace a Target Deliverable with an alternate of approximately equal or greater scope.

Additionally, some Target Deliverables may have dependencies on external parties that are not fully under our control. For example, some of our Target Deliverables are dependent on the launch of ENSv2. We cannot fully control when ENSv2 launches. If Target Deliverables become blocked due to external parties, we reserve the right to replace an impacted Target Deliverable with an alternate of approximately equal or greater scope.

We have a discussion open with ENS Labs about the possibility of an ENS Referral Program launching as part of ENSv1, rather than ENSv2. In the event the ENS DAO votes to approve and fund alternate ENS Referral Program strategies from those we have proposed, we reserve the right to replace impacted Target Deliverables with alternates of approximately equal or greater scope. If our Extended Scope is approved and the situation described in this clause is triggered, we will coordinate with Metagov Stewards on a responsible solution, such as us transferring the $50k in guaranteed ENSv2 Referral Programs funding into whatever pool of funds is servicing the alternate ENS Referral Program strategy, such that the broader intentions motivating the approval of our extended budget are followed as best as possible.

The following tables identify a quarterly breakdown of Target Deliverables for each of the ENS Infrastructure Solutions in our “basic” and “extended” scope.

Each quarter listed in these tables is relative to (the commencement date of SPP2 funding streams) + (3 months \* quarter) ~ ending day of that calendar month.

Each quarterly report will be delivered within 10 days of the conclusion of the quarter.

## 4.1. Basic Scope of Work

### 4.1.1 ENSNode

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. Transition ens-test-env from the ENS Subgraph to ENSNode in preparation for ENSv2 release.2. Coordinate with the ENS Labs team to identify and document the key requirements for transitioning the official ENS manager app and ENSjs to ENSNode and for supporting their ENSv2 requirements.3. Release “v1” of tokenized DNS name indexing.4. Complete audit of ENSv2 contracts and submit suggestions for optimized ENSv2 indexing.5. Expand multichain indexing support to 1-2 additional chains.6. Release L2 Primary Names indexing. |
| Q2 | 1. Release “v1” of ENSNode to ensure the ENS ecosystem has an indexed data solution available prior to the ENSv2 release.2. Preview release of “ENS Resolution Accelerator” technology.3. Deploy hosted instances of ENSNode with optimized uptime availability free for the ENS community to use.4. Ship “v1” of ENSNode developer docs.5. Expand multichain indexing support to 1-2 additional chains.6. Support the transition of 1-3 apps in the ENS ecosystem from the ENS Subgraph to ENSNode. |
| Q3 | 1. Ship “v1” of “ENS Resolution Accelerator” technology.2. Optimized self-hosting and DevOps to support stronger ENS protocol decentralization.3. Preview release of Offchain ENS Name indexing.4. Release “v2” of tokenized DNS name indexing.5. Expand multichain indexing support to 1-2 additional chains.6. Support the transition of 1-3 apps in the ENS ecosystem from the ENS Subgraph to ENSNode. |
| Q4 | 1. Ship “v1” of Offchain ENS Name indexing.2. Ship “v2” of “ENS Resolution Accelerator” technology.3. Optimized scalability and maximised uptime enhancements.4. Ship “v2” of ENSNode developer docs.5. Expand multichain indexing support to 1-2 additional chains.6. Support the transition of 1-3 apps in the ENS ecosystem from the ENS Subgraph to ENSNode. |

### 4.1.2. ENSRainbow

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. Release “.ensrainbow” file type format for improved portability of ENSRainbow data sets. |
| Q2 | 1. Release “Intelligent Data Set Versioning” capability, enabling a single ENSRainbow instance to grow its set of healed labels across time while maintaining stable behaviour for each connected ENSNode instance. |
| Q3 | 1. Release “ENSRainbow Searchlight Server”, which will continuously use a variety of strategies to heal otherwise unknown labels. |
| Q4 | 1. Release “ENSRainbow Searchlight Protocol”, which will enable anyone in the ENS community to submit healed labels they discovered for broader ENS community use. |

### 4.1.3. ENSAdmin

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. Ship “ENS Protocol Inspector” support for 2 additional ENS resolution scenarios.2. Expand the ENS integrator library of important ENS resolution test cases by 2 or more.3. Ship optimized ENSNode indexing status dashboard. |
| Q2 | 1. Ship “ENS Protocol Inspector” support for 2 additional ENS resolution scenarios.2. Expand the ENS integrator library of important ENS resolution test cases by 2 or more.3. Ship ENSv2 Protocol Inspector (specialized for ENSv2 contracts). |
| Q3 | 1. Ship “ENS Protocol Inspector” support for 2 additional ENS resolution scenarios.2. Expand the ENS integrator library of important ENS resolution test cases by 2 or more.3. Ship “ENS Protocol Inspector” for “ENS Resolution Accelerator”. |
| Q4 | 1. Ship “ENS Protocol Inspector” support for 2 additional ENS resolution scenarios.2. Expand the ENS integrator library of important ENS resolution test cases by 2 or more.3. Ship ENSNode DevOps dashboard for improved ENSNode operations, monitoring, and maintenance. |

### 4.1.4. ENSv2 Referral Programs (Technical Deployment)

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. Ship contracts and documentation with proposed referral program revenue sharing strategy in preparation for ENSv2 launch. |
| Q2 | 1. Ship promotional landing page microsite in preparation for ENSv2 Referral Programs launch. |
| Q3 | 1. Ship indexer and live reward tracking dashboards for ENSv2 Referral Programs launch. |
| Q4 | 1. Launch ENSv2 Referral Programs in coordination with the launch of ENSv2. |

### 4.1.5. NameGraph

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. R&D for supporting community curated name collections.2. R&D for LLM-augmented collection refinements.3. Ship 1-2 new NameGraph integrations. |
| Q2 | 1. R&D for supporting community curated name collections.2. R&D for LLM-augmented collection refinements.3. Ship 1-2 new NameGraph integrations. |
| Q3 | 1. Preview release for supporting community curated name collections.2. Preview release for LLM-augmented collection refinements.3. Ship 1-2 new NameGraph integrations. |
| Q4 | 1. Ship “v1” release for supporting community curated name collections.2. Ship “v1” release for LLM-augmented collection refinements.3. Ship 1-2 new NameGraph integrations. |

### 4.1.6. NameAI

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. Ship enhanced AI tokenizer strategies.2. Ship 1 new NameAI integration. |
| Q2 | 1. Ship enhanced internationalized name tokenizer strategies.2. Ship 1 new NameAI integration. |
| Q3 | 1. Ship “v1” release of an enhanced NameAI technology showcase demonstrating valuable strategies for multi-dimensional name scoring.2. Ship 1 new NameAI integration. |
| Q4 | 1. Ship “v2” release of an enhanced NameAI technology showcase demonstrating valuable strategies for multi-dimensional name scoring.2. Ship 1 new NameAI integration. |

### 4.1.7. NameGuard

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. R&D for rearchitecture transitioning to use of ENSNode services for improved analysis of ENS names. |
| Q2 | 1. Ship “v1” rearchitecture transitioning to use of ENSNode services for improved analysis of ENS names. |
| Q3 | 1. Ship “v2” rearchitecture transitioning core NameGuard and LabelInspector logic from Python into TypeScript packages that can be embedded directly into ENSNode or other apps / services.2. Ship 1 new ENS name configuration health check. |
| Q4 | 1. Ship 3 new ENS name configuration health checks.2. Ship NameGuard integration with the “ENS Protocol Inspector” in ENSAdmin. |

### 4.1.8. NameKit

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. R&D for rearchitecture transitioning to use of ENSNode services as an accelerated loading strategy for NameKit React hooks and UI component libraries. |
| Q2 | 1. Ship preview React Hooks and UI component library for accelerated ENS social profiles. |
| Q3 | 1. Ship “v1” React Hooks and UI component library for accelerated ENS social profiles.2. Ship integration with ENSAdmin.3. Ship integration with NameGraph.4. R&D for “Universal” ENS profile editing React hooks and UI components. |
| Q4 | 1. Ship “v1” of “Universal” ENS profile editing React hooks and UI components.2. Ship 3-6 integrations of NameKit. |

## 4.2. Extended Scope of Work

### 4.2.1. ENSv2 Referral Programs (Guaranteed $50k Funding)

| Quarter | Target Deliverables |
| --- | --- |
| (circa 2 quarters before expected ENSv2 launch) | 1. Ship 5-10 targeted outreach campaigns to prospective ENSv2 Referral Program apps and wallets, promoting the recurring revenue model opportunity for promoting the registration and renewal of .eth names. |
| (circa 1 quarter before expected ENSv2 launch) | 1. Deliver ENS integration support to apps and wallets expressing interest to participate in ENSv2 Referral Programs.2. Ship 5-10 additional targeted outreach campaigns to prospective ENSv2 Referral Program apps and wallets, promoting the recurring revenue model opportunity for promoting the registration and renewal of .eth names. |
| (quarter of ENSv2 launch) | 1. Fund ENSv2 Referral Programs contracts with guaranteed $50k.2. Deliver ENS integration support to apps and wallets expressing interest to participate in ENSv2 Referral Programs.3. Ship 5-10 additional targeted outreach campaigns to prospective ENSv2 Referral Program apps and wallets, promoting the recurring revenue model opportunity for promoting the registration and renewal of .eth names. |
| (quarter after ENSv2 launch) | 1. Report on outcomes, lessons learned, and suggestions for the future for ENS Referral Programs. |

### 4.2.2. ENS TokenScope

| Quarter | Target Deliverables |
| --- | --- |
| Q1 | 1. R&D for protocol implementation strategies to map from ENS names to their ownership controlling tokens.2. Ship support for name sales history. |
| Q2 | 1. Ship support for aggregation of onchain and offchain buy and sell order data for tokenized ENS names.2. Ship support for querying the top buy and sell orders for tokenized ENS names. |
| Q3 | 1. Ship support for updating the status of buy orders based on wallet balance changes.2. Ship support for creating new buy and sell orders for tokenized ENS names. |
| Q4 | 1. Ship support for unified queries of primary and secondary market state for tokenized ENS names.2. Ship 2-4 integrations with ENS TokenScope. |

## 4.3. Second-Year Stream Scope of Work

The ENS ecosystem changes fast. The details of specifically what may be the most impactful Target Deliverables to create value for ENS more than a year from now are likely to change.

What doesn’t change is our team’s “north star” of identifying key high-value needs in ENS and then working to solve them. We follow an opportunistic and pragmatic approach to optimise for value creation.

The scope for the second-year of our budget would include an equal or greater scope of work as the first-year. On a rolling basis, upon the delivery of our quarterly reports, we will maintain a roadmap of Target Deliverables extending at least 2 quarters into the future for each quarter in the second-year.

Target Deliverables in a second-year can confidently be assumed to include continued high-value enhancements to each of our 8 ENS Infrastructure projects in addition to new valuable ENS infrastructure project opportunities that emerge over time.

---

# Post #3 by James
Posted at: 2025-04-01T06:18:11.345Z

Dam! What a proposal - Firstly big ups for the how in-depth this proposal is, specifically 4.1 with deliverables broken down by quarter. Very impressive.

FireEyes supports Namehash’s continuous development of ENS and is excited to see how as a service provider they’re able to deliver the huge list of outcomes ![:fire:](https://discuss.ens.domains/images/emoji/twitter/fire.png?v=12 ":fire:")

---

# Post #4 by daostrat.eth
Posted at: 2025-04-01T12:19:43.820Z

Hey [@lightwalker.eth](/u/lightwalker.eth)

Thank you for submitting your application for the ENS Service Provider Program, Season 2. We are pleased to confirm that your application meets the eligibility criteria as outlined in the program design.

Good luck running for SPP2!

*-MetaGov*

---

# Post #5 by nick.eth
Posted at: 2025-04-01T13:48:00.500Z

I’m happy to endorse Namehash’s nomination as a streaming provider this term. Their subgraph replacement in particular will be vital infrastructure for ENS going forward.

---

# Post #6 by Zimtente
Posted at: 2025-04-02T06:39:17.378Z

[@lightwalker.eth](/u/lightwalker.eth) and his team @namehash are doing incredible work in the ENS space. We @vision already profit from their work they have put into NameAI and Namegraph. I def. support their proposal and look forward to continue to work with them!

![:slight_smile:](https://discuss.ens.domains/images/emoji/twitter/slight_smile.png?v=12 ":slight_smile:")

To add: @ensnode I use the ENS Subgraph for [vision.io](http://vision.io) since inception of ens.vision back March 2022. And my feedback would be that it “sucks”. There are a whole lot of unknowns and things that you have to guess and figure out by your own as nothing is documented. Especially since the introduction of the NW I had to add a whole lot of workarounds and had a whole lot of redeployments because something was not as I did expect. Example: [Subgraph Domain.expiryDate checkup - #4 by Zimtente](https://discuss.ens.domains/t/subgraph-domain-expirydate-checkup/19199/4) (there are whole lot more of these). Or that Renew Events are for some reason not considered a “Domain Event” which just makes use consume double the credits as we need to track 2 event streams from the graph instead of just one.

So I’m very much looking forward to use ensnode instead as it would make our lives @ vision much easier in terms of indexing ENS related data that we use to power vision back and frontend.

---

