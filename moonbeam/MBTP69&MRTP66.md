# [Dwellir’s Proposal for Moonbeam, Moonriver, and Moonbase Alpha RPC Services (Q2/Q3 2026)](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2026/2451/2)

## [](#p-7942-abstract-1)ABSTRACT

Dwellir is committed to empowering developers worldwide by providing instant data access and robust infrastructure tailored for web3 applications. With extensive experience supporting Moonbeam, Moonriver, Moonbase Alpha, and over 150 other blockchain networks, Dwellir sets itself apart through its ownership and operation of dedicated bare metal servers. This infrastructure approach ensures superior performance, enhanced security, full control over configurations, and consistent reliability.

This proposal specifically seeks funding to continue providing fully managed Public Archival RPC services for the Moonbeam ecosystem, utilizing distinct and specialized node software that ensures optimal performance and security. Our infrastructure, strategically located across data centers in Sweden, US-West, and Singapore, guarantees high availability, fault tolerance, efficient load balancing, and seamless operational continuity during maintenance periods.

Recognized globally for exceptional geographical performance, Dwellir’s service has processed 4.5 billion requests in Q4 2025/Q1 2026, demonstrating proven capability and robust scalability.

The proposed budget of $11,400 for six months covers comprehensive operational requirements, including traffic management, storage, memory allocation, and CPU utilization, ensuring continuous, enterprise-level service delivery that directly contributes to the reliability and growth of the Moonbeam blockchain community.

## [](#p-7942-motivation-2)MOTIVATION

The Dwellir mission is to serve developers worldwide with instant data access and a comprehensive suite of tools so that they can build web3 applications.

## [](#p-7942-project-overview-and-experience-3)PROJECT OVERVIEW AND EXPERIENCE

We currently run RPC services for Moonbeam, Moonriver and Moonbase Alpha and more than 150 other blockchain networks. Currently, we are processing 1.5 billion requests per day on average and you will see throughout this proposal that our experience within the Moonbeam ecosystem is extensive.

One of the key differentiators with Dwellir is that we own and operate our own bare metal machines which have several important effects:

**Performance:** Bare metal servers offer superior performance and low-latency communication, essential for decentralized networks to efficiently process transactions and reach consensus.

**Security:** Bare metal servers provide enhanced security and isolation, safeguarding sensitive data and assets in a decentralized network.

**Control:** With bare metal servers, node operators have full control over hardware and software configurations, ensuring adherence to network rules and consensus mechanisms.

**Reliability:** Bare metal servers offer robustness and stability, making them reliable choices for continuous operation in decentralized networks.

**Expertise:** Our team has a proven track record of creating tailor-made blockchain infrastructure that align with the Moonbeam community’s specific needs.

**Support:** We don’t just build and leave – our team stands by the community for the long haul. We engage with ongoing support, maintenance, and optimization services to keep the networks running smoothly and efficiently.

## [](#p-7942-relevant-news-4)RELEVANT NEWS

Dwellir has introduced GEO load balancing between our nodes in Europe, APAC (Singapore) and US-West ensuring a faster and more reliable experience for our users. By routing traffic to the closest and most responsive node, we minimize latency and enhance performance for Moonbeam applications. This upgrade strengthens our commitment to the community.

The new GEO load-balanced RPC endpoints have new URLs. Please update your configurations to the new URLs:

- Moonbeam: [moonbeam-rpc.n.dwellir.com](http://moonbeam-rpc.n.dwellir.com)

- Moonriver: [moonriver-rpc.n.dwellir.com](http://moonriver-rpc.n.dwellir.com)

- Moonbase: [moonbase-rpc.n.dwellir.com](http://moonbase-rpc.n.dwellir.com)

The old endpoints (*.dwellir.com without .n.) will be decommissioned soon, so we strongly recommend switching to the new addresses as soon as possible to ensure uninterrupted service.

## [](#p-7942-service-statistics-5)SERVICE STATISTICS

During Q4 2025 and so far in Q1 2026 Dwellir processed 4.5 billion requests for the Moonbeam ecosystem. We expect this to increase upon inclusion in the program.

## [](#p-7942-overall-cost-6)OVERALL COST

Total cost for six (6) months is USD 11,400

Chain
Cost per month

Moonbeam
$750

Moonriver
$750

Moonbase-alpha
$400

**Monthly Total**
**$1,900**

**Six Months Total**
**$11,400**

This includes all three services across three geographical regions (Europe, US-West, Asia). More detailed costs in the full proposal.

## [](#p-7942-specifications-7)SPECIFICATIONS

### [](#p-7942-connections-and-node-methods-8)Connections and Node Methods

Dwellir sets max connections to 10,000 concurrent WebSockets. From time to time we increase this to 30,000 to deal with events such as the ordinals rush.

Dwellir maintains multiple 2 Gigabit external connections with the option to raise this to 10 Gigabit.

Dwellir allows for tracing methods including eth_getLogs as standard.

### [](#p-7942-location-of-nodes-9)Location of Nodes

Dwellir owns all of our own hardware and currently hosts Moonbeam services across data centers in three locations:

- Sweden (multiple sites)

- US (West)

- Singapore

## [](#p-7942-use-of-treasury-funds-10)USE OF TREASURY FUNDS

To cover the costs of hardware operation and maintenance. We own and operate our own bare metal services in three locations.

### [](#p-7942-deliverables-11)Deliverables

- RPC endpoints continuously maintained for Moonbeam, Moonriver, and Moonbase-Alpha with near 100% uptime.

- Bootnodes – already up and running for seamless peer-to-peer network connectivity at zero extra cost.

## [](#p-7942-requirements-12)REQUIREMENTS

Requirement
Detail

Pricing in USD denomination
USD $11,400

Inclusion of the eth_getLogs RPC method
YES

Information about bootnode operation on all three networks
YES for all networks

Cost for 6-months
USD $11,400

## [](#p-7942-link-to-full-proposal-13)LINK TO FULL PROPOSAL

  

      [docs.google.com](https://docs.google.com/document/d/1ngls0n9jLsYUbrG_yV8zelTVPTq2LR8qtjqSN76oMIk/edit?usp=sharing)
  

  
    

### [Moonbeam RPC Services Submission Q2 2026 & Q3 2026](https://docs.google.com/document/d/1ngls0n9jLsYUbrG_yV8zelTVPTq2LR8qtjqSN76oMIk/edit?usp=sharing)

Moonbeam Public RPC Dwellir Submission  Q2 2026 & Q3 2026         Table of Contents Executive Summary	3 Mission	4 Experience	4 Type of service and nodes	5 Connections and Node Methods	5 Location of Nodes	5 Geographical Performance	6 Boot Nodes	6...

---

### Reply by _yrn

Hey [@benn_69](/u/benn_69) ,

Thank you for your proposal and for your continued support of the Moonbeam ecosystem.

Following the council’s review process, we’re happy to inform you that Dwellir has been selected to receive treasury funding for RPC service provisioning for the Q2 + Q3 2026 term.

The council recognized the strength of your offering, particularly in terms of infrastructure reliability, geographic distribution, and operational maturity. Your proposal was well-structured, competitive, and aligned with our network’s high-performance requirements.

Following our transition to stablecoin payouts, we are pleased to perform this payout in Moonbeam native USDC.

Please provide your recipient address on Moonbeam so we can proceed with the on-chain payouts.

Many thanks and kind regards,

Yaron — On behalf of the Treasury Council

---

### Reply by _yrn

Hey [@benn_69](/u/benn_69), we just experienced a bug  in the code with regards to xcUSDC payouts which requires a runtime upgrade to fix. The earliest this could be addressed is RT4300, which is targeting May 13th — so unfortunately we won’t be waiting on that. We’ll need to proceed with a final round of native token payouts to make sure the beneficiaries are covered before that. Apologies for the inconvenience.

Could you confirm that Dwellir is ok with receiving the upcoming quarterly payout of $5,700 in native tokens for now? Also, please don’t forget to publicly share your desired beneficiary address here. We’ll update asap with a new onchain proposal next. Thanks!

---

### Reply by benn_69

[@_yrn](/u/_yrn)

Moonbeam: *0xF8D757E04BF0fbd5432E743DD8612E62A9c983cf*

Moonriver: *0xF8D757E04BF0fbd5432E743DD8612E62A9c983cf*

---
*Generated by Payoutor*
*Moonbeam Proposal ID: 69*
*Moonriver Proposal ID: 66*
*Beneficiary: 0xF8D757E04BF0fbd5432E743DD8612E62A9c983cf*
*Reward: 241075.9601 GLMR*
*Submitted by: Yaron*
