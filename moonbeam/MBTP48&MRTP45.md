Dwellir’s Proposal for Moonbeam, Moonriver, and Moonbase Alpha RPC Services (Q2-Q3, 2025)


## ABSTRACT

Dwellir is committed to empowering developers worldwide by providing instant data access and robust infrastructure tailored for web3 applications. With extensive experience supporting Moonbeam, Moonriver, Moonbase Alpha, and over 100 other blockchain networks, Dwellir sets itself apart through its ownership and operation of dedicated bare metal servers. This infrastructure approach ensures superior performance, enhanced security, full control over configurations, and consistent reliability.

This proposal specifically seeks funding to continue providing fully managed Public Archival RPC services for the Moonbeam ecosystem, utilizing distinct and specialized node software that ensures optimal performance and security. Our infrastructure, strategically located across data centers in Sweden, Tunisia, and Singapore, guarantees high availability, fault tolerance, efficient load balancing, and seamless operational continuity during maintenance periods.

Recognized globally for exceptional geographical performance, Dwellir’s service has processed over 4.2 billion requests for the Moonbeam ecosystem from Q4 2024 to Q1 2025 alone, demonstrating proven capability and robust scalability.

The proposed budget of $10,913.06 for six months covers comprehensive operational requirements, including traffic management, storage, memory allocation, and CPU utilization, ensuring continuous, enterprise-level service delivery that directly contributes to the reliability and growth of the Moonbeam blockchain community.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-motivation-2)MOTIVATION

The Dwellir mission is to serve developers worldwide with instant data access and a comprehensive suite of tools so that they can build web3 applications.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-project-overview-and-experience-3)PROJECT OVERVIEW AND EXPERIENCE

We currently run RPC services for Moonbeam, Moonriver and Moonbase Alpha and more than 150 other blockchain networks. Currently, we are processing 1.4 billion requests per day on average and you will see throughout this proposal that our experience within the Moonbeam ecosystem is extensive.

One of the key differentiators with Dwellir is that we own and operate our own bare metal machines which have several important effects.

Performance: Bare metal servers offer superior performance and low-latency communication, essential for decentralized networks to efficiently process transactions and reach consensus.

Security: Bare metal servers provide enhanced security and isolation, safeguarding sensitive data and assets in a decentralized network.

Control: With bare metal servers, node operators have full control over hardware and software configurations, ensuring adherence to network rules and consensus mechanisms.

Reliability: Bare metal servers offer robustness and stability, making them reliable choices for continuous operation in decentralized networks.

Expertise: Our team has a proven track record of creating tailor-made blockchain infrastructure that align with the Moonbeam community’s specific needs.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-relevant-news-4)RELEVANT NEWS

Dwellir has introduced GEO load balancing between our nodes in Europe and APAC (Singapore), ensuring a faster and more reliable experience for our users. By routing traffic to the closest and most responsive node, we minimize latency and enhance performance for Moonbeam applications. This upgrade strengthens our commitment to the community.

The new GEO load-balanced RPC endpoints have new URLs. Please update your configurations to the new URLs:

-   Moonbeam:  [moonbeam-rpc.n.dwellir.com](http://moonbeam-rpc.n.dwellir.com/)
-   Moonriver:  [moonriver-rpc.n.dwellir.com](http://moonriver-rpc.n.dwellir.com/)
-   Moonbase:  [moonbase-rpc.n.dwellir.com](http://moonbase-rpc.n.dwellir.com/)

The old endpoints (*.dwellir.com without .n.) will be decommissioned soon, so we strongly recommend switching to the new addresses as soon as possible to ensure uninterrupted service.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-service-statistics-5)SERVICE STATISTICS

[![Screenshot 2025-03-14 at 08.38.34](https://forum.moonbeam.network/uploads/db2361/optimized/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d_2_411x500.png)](https://forum.moonbeam.network/uploads/db2361/original/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d.png "Screenshot 2025-03-14 at 08.38.34")

Screenshot 2025-03-14 at 08.38.34638×776 95.4 KB

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-overall-cost-6)OVERALL COST

The total budget for the proposal is  **$10,913.06**  for Q2 and Q3 of 2025, covering:  
**$1,818.84 per month**  for RPC services, boot nodes, and infrastructure maintenance.

Monthly Subtotal

$1,732.23

Monthly Operations (5%)

$86.61

Monthly Total

$1,818.84

Quarterly Total

$5,456.53

Six Months Total

$10,913.06

_This includes all three services across three geographical regions (Europe, Asia, North Africa). More detailed costs in the full proposal._

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-specifications-7)SPECIFICATIONS

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-connections-and-node-methods-8)Connections and Node Methods

Dwellir sets max connections to 10,000 concurrent WebSockets. From time to time we increase this to 30,000 to deal with events such as the ordinals rush.

Dwellir maintains multiple 2 Gigabit external connections with the option to raise this to 10 Gigabit.

Dwellir allows for tracing methods including eth_getLogs as standard.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-location-of-nodes-9)Location of Nodes

Dwellir owns all of our own hardware and current we host services across data centers in four locations:

1.  Sweden (site 1)
2.  Sweden (site 2)
3.  Tunisia
4.  Nigeria*
5.  Singapore

*Nigeria is where we host services that are connected to the IBP program. These services ARE NOT included in this proposal. We DO NOT use that datacenter or equipment in order to fulfill other proposals.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-use-of-treasury-funds-10)USE OF TREASURY FUNDS

To cover the costs of hardware operation and maintenance. We own and operate our own bare metal services in 4 locations.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-deliverables-11)Deliverables

-   **RPC endpoints**  continuously maintained for Moonbeam, Moonriver, and Moonbase-Alpha with near 100% uptime.
-   **Bootnodes**  - already up and running for seamless peer-to-peer network connectivity.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-requirements-12)REQUIREMENTS

Estimated call volumes = 4.2 billion  
Pricing in USD denomination = USD $10,913.06  
Inclusion of the  `eth_getLogs`  RPC method : YES  
Information about bootnode operation on all three networks: YES for all networks

**Cost for 6-months: USD $10,913.06**

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-link-to-full-proposal-13)LINK TO FULL PROPOSAL

[Link to full proposal](https://docs.google.com/document/d/1eRs7ey7Qwl-JWSO2Yl9oBGHB6HTe5qFYpSteCirO2e4/edit?usp=sharing)

  

1 Reply

1​

​​Reply

66views13likes1link

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png "benn_69")](https://forum.moonbeam.network/u/benn_69 "benn_69")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png "aaron.mbf")](https://forum.moonbeam.network/u/aaron.mbf "aaron.mbf")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[18d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/2?u=_yrn "Post date")

Hey  [@benn_69](https://forum.moonbeam.network/u/benn_69)! Thanks for your submission, much appreciated!  
Quick rapid fire Q — Would you consider to route calls to the old Dwellir endpoint URLs fwd to the new ones internally, instead of decommissioning them entirely? That would be awesome.  
RPC URL configs like these tend to be sticky among users and dApps which might cause some issues and possibly lead to a significant decrease in calls to the Dwellir endpoints with fallbacks in place.  
Thanks so much so for your submission! You’ll be hearing from us soon™️

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/3?u=_yrn "Post date")

[@benn_69](https://forum.moonbeam.network/u/benn_69)  sorry to bump this, but I’d appreciate a quick thumbs up or down on the endpoint null routing issue as the Treasury Council is keen to conclude its decision process in time. Thank you!

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/4?u=_yrn "Post date")

We can fix a solution so that other users can use previous URLs and we will route traffic.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/5?u=_yrn "Post date")

That’s awesome, thanks!  ![:raised_hands:](https://forum.moonbeam.network/images/emoji/twitter/raised_hands.png?v=12 ":raised_hands:")

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png)](https://forum.moonbeam.network/u/aaron.mbf)

[aaron.mbf](https://forum.moonbeam.network/u/aaron.mbf)[Technical Council member](https://forum.moonbeam.network/g/TreasuryCouncil)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/6?u=_yrn "Post date")

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/48/109_2.png)  benn_69:

> SERVICE STATISTICS

Any idea why the sudden drop in requests to Moonbeam in December?

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/7?u=_yrn "Post date")

Nothing obvious stands out on our end. We occasionally see similar behavior across our services.

Toward the end of last year, we had discussions with several wallet providers (Talisman, Subwallet, and Fearless) to help optimize their RPC calls to our nodes, which could have contributed to this change.

It’s also possible that some public usage shifted toward our API service—we’ve noticed increased activity there.

**TL;DR:**  Our team hasn’t identified any significant insights from available reports.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8?u=_yrn "Post date")

Dear  [@Benn_69](https://forum.moonbeam.network/u/benn_69),

I am writing you on behalf of the Treasury Council.

First and foremost, we would like to express our sincere appreciation for your proposal. We recognize the considerable effort that went into it.

After careful consideration over the past few days, the Council members have reached a final decision: for the upcoming Q2/Q3 2025 period, we will be funding only 2 RPC teams (down from 3 in the previous period), based on the following factors:

-   Current market conditions, which require us to be cost-conscious.
-   A reduction in overall activity due to lower market conditions.
-   IBP services, which are already covered by the Polkadot treasury.

A shortlist of 2 providers for Q2/Q3 2025 has been defined following a thorough evaluation, and we’re glad to announce you that Dwellir is included in this selection.

**At this point we need from your side the beneficiary addresses for both Moonbeam and Moonriver to trigger our Payment operations accordingly.**

Once again, thank you for your proposal and your continued partnership!!!

Best regards,  
Michele, on behalf of the Treasury Council

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/9?u=_yrn "Post date")

Thank you for entrusting us! We’re very honoured to grow with Moonbeam.

The beneficiary address for both GLMR and MOVR is:

0xF8D757E04BF0fbd5432E743DD8612E62A9c983c## ABSTRACT

Dwellir is committed to empowering developers worldwide by providing instant data access and robust infrastructure tailored for web3 applications. With extensive experience supporting Moonbeam, Moonriver, Moonbase Alpha, and over 100 other blockchain networks, Dwellir sets itself apart through its ownership and operation of dedicated bare metal servers. This infrastructure approach ensures superior performance, enhanced security, full control over configurations, and consistent reliability.

This proposal specifically seeks funding to continue providing fully managed Public Archival RPC services for the Moonbeam ecosystem, utilizing distinct and specialized node software that ensures optimal performance and security. Our infrastructure, strategically located across data centers in Sweden, Tunisia, and Singapore, guarantees high availability, fault tolerance, efficient load balancing, and seamless operational continuity during maintenance periods.

Recognized globally for exceptional geographical performance, Dwellir’s service has processed over 4.2 billion requests for the Moonbeam ecosystem from Q4 2024 to Q1 2025 alone, demonstrating proven capability and robust scalability.

The proposed budget of $10,913.06 for six months covers comprehensive operational requirements, including traffic management, storage, memory allocation, and CPU utilization, ensuring continuous, enterprise-level service delivery that directly contributes to the reliability and growth of the Moonbeam blockchain community.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-motivation-2)MOTIVATION

The Dwellir mission is to serve developers worldwide with instant data access and a comprehensive suite of tools so that they can build web3 applications.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-project-overview-and-experience-3)PROJECT OVERVIEW AND EXPERIENCE

We currently run RPC services for Moonbeam, Moonriver and Moonbase Alpha and more than 150 other blockchain networks. Currently, we are processing 1.4 billion requests per day on average and you will see throughout this proposal that our experience within the Moonbeam ecosystem is extensive.

One of the key differentiators with Dwellir is that we own and operate our own bare metal machines which have several important effects.

Performance: Bare metal servers offer superior performance and low-latency communication, essential for decentralized networks to efficiently process transactions and reach consensus.

Security: Bare metal servers provide enhanced security and isolation, safeguarding sensitive data and assets in a decentralized network.

Control: With bare metal servers, node operators have full control over hardware and software configurations, ensuring adherence to network rules and consensus mechanisms.

Reliability: Bare metal servers offer robustness and stability, making them reliable choices for continuous operation in decentralized networks.

Expertise: Our team has a proven track record of creating tailor-made blockchain infrastructure that align with the Moonbeam community’s specific needs.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-relevant-news-4)RELEVANT NEWS

Dwellir has introduced GEO load balancing between our nodes in Europe and APAC (Singapore), ensuring a faster and more reliable experience for our users. By routing traffic to the closest and most responsive node, we minimize latency and enhance performance for Moonbeam applications. This upgrade strengthens our commitment to the community.

The new GEO load-balanced RPC endpoints have new URLs. Please update your configurations to the new URLs:

-   Moonbeam:  [moonbeam-rpc.n.dwellir.com](http://moonbeam-rpc.n.dwellir.com/)
-   Moonriver:  [moonriver-rpc.n.dwellir.com](http://moonriver-rpc.n.dwellir.com/)
-   Moonbase:  [moonbase-rpc.n.dwellir.com](http://moonbase-rpc.n.dwellir.com/)

The old endpoints (*.dwellir.com without .n.) will be decommissioned soon, so we strongly recommend switching to the new addresses as soon as possible to ensure uninterrupted service.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-service-statistics-5)SERVICE STATISTICS

[![Screenshot 2025-03-14 at 08.38.34](https://forum.moonbeam.network/uploads/db2361/optimized/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d_2_411x500.png)](https://forum.moonbeam.network/uploads/db2361/original/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d.png "Screenshot 2025-03-14 at 08.38.34")

Screenshot 2025-03-14 at 08.38.34638×776 95.4 KB

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-overall-cost-6)OVERALL COST

The total budget for the proposal is  **$10,913.06**  for Q2 and Q3 of 2025, covering:  
**$1,818.84 per month**  for RPC services, boot nodes, and infrastructure maintenance.

Monthly Subtotal

$1,732.23

Monthly Operations (5%)

$86.61

Monthly Total

$1,818.84

Quarterly Total

$5,456.53

Six Months Total

$10,913.06

_This includes all three services across three geographical regions (Europe, Asia, North Africa). More detailed costs in the full proposal._

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-specifications-7)SPECIFICATIONS

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-connections-and-node-methods-8)Connections and Node Methods

Dwellir sets max connections to 10,000 concurrent WebSockets. From time to time we increase this to 30,000 to deal with events such as the ordinals rush.

Dwellir maintains multiple 2 Gigabit external connections with the option to raise this to 10 Gigabit.

Dwellir allows for tracing methods including eth_getLogs as standard.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-location-of-nodes-9)Location of Nodes

Dwellir owns all of our own hardware and current we host services across data centers in four locations:

1.  Sweden (site 1)
2.  Sweden (site 2)
3.  Tunisia
4.  Nigeria*
5.  Singapore

*Nigeria is where we host services that are connected to the IBP program. These services ARE NOT included in this proposal. We DO NOT use that datacenter or equipment in order to fulfill other proposals.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-use-of-treasury-funds-10)USE OF TREASURY FUNDS

To cover the costs of hardware operation and maintenance. We own and operate our own bare metal services in 4 locations.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-deliverables-11)Deliverables

-   **RPC endpoints**  continuously maintained for Moonbeam, Moonriver, and Moonbase-Alpha with near 100% uptime.
-   **Bootnodes**  - already up and running for seamless peer-to-peer network connectivity.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-requirements-12)REQUIREMENTS

Estimated call volumes = 4.2 billion  
Pricing in USD denomination = USD $10,913.06  
Inclusion of the  `eth_getLogs`  RPC method : YES  
Information about bootnode operation on all three networks: YES for all networks

**Cost for 6-months: USD $10,913.06**

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-link-to-full-proposal-13)LINK TO FULL PROPOSAL

[Link to full proposal](https://docs.google.com/document/d/1eRs7ey7Qwl-JWSO2Yl9oBGHB6HTe5qFYpSteCirO2e4/edit?usp=sharing)

  

1 Reply

1​

​​Reply

66views13likes1link

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png "benn_69")](https://forum.moonbeam.network/u/benn_69 "benn_69")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png "aaron.mbf")](https://forum.moonbeam.network/u/aaron.mbf "aaron.mbf")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[18d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/2?u=_yrn "Post date")

Hey  [@benn_69](https://forum.moonbeam.network/u/benn_69)! Thanks for your submission, much appreciated!  
Quick rapid fire Q — Would you consider to route calls to the old Dwellir endpoint URLs fwd to the new ones internally, instead of decommissioning them entirely? That would be awesome.  
RPC URL configs like these tend to be sticky among users and dApps which might cause some issues and possibly lead to a significant decrease in calls to the Dwellir endpoints with fallbacks in place.  
Thanks so much so for your submission! You’ll be hearing from us soon™️

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/3?u=_yrn "Post date")

[@benn_69](https://forum.moonbeam.network/u/benn_69)  sorry to bump this, but I’d appreciate a quick thumbs up or down on the endpoint null routing issue as the Treasury Council is keen to conclude its decision process in time. Thank you!

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/4?u=_yrn "Post date")

We can fix a solution so that other users can use previous URLs and we will route traffic.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/5?u=_yrn "Post date")

That’s awesome, thanks!  ![:raised_hands:](https://forum.moonbeam.network/images/emoji/twitter/raised_hands.png?v=12 ":raised_hands:")

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png)](https://forum.moonbeam.network/u/aaron.mbf)

[aaron.mbf](https://forum.moonbeam.network/u/aaron.mbf)[Technical Council member](https://forum.moonbeam.network/g/TreasuryCouncil)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/6?u=_yrn "Post date")

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/48/109_2.png)  benn_69:

> SERVICE STATISTICS

Any idea why the sudden drop in requests to Moonbeam in December?

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/7?u=_yrn "Post date")

Nothing obvious stands out on our end. We occasionally see similar behavior across our services.

Toward the end of last year, we had discussions with several wallet providers (Talisman, Subwallet, and Fearless) to help optimize their RPC calls to our nodes, which could have contributed to this change.

It’s also possible that some public usage shifted toward our API service—we’ve noticed increased activity there.

**TL;DR:**  Our team hasn’t identified any significant insights from available reports.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8?u=_yrn "Post date")

Dear  [@Benn_69](https://forum.moonbeam.network/u/benn_69),

I am writing you on behalf of the Treasury Council.

First and foremost, we would like to express our sincere appreciation for your proposal. We recognize the considerable effort that went into it.

After careful consideration over the past few days, the Council members have reached a final decision: for the upcoming Q2/Q3 2025 period, we will be funding only 2 RPC teams (down from 3 in the previous period), based on the following factors:

-   Current market conditions, which require us to be cost-conscious.
-   A reduction in overall activity due to lower market conditions.
-   IBP services, which are already covered by the Polkadot treasury.

A shortlist of 2 providers for Q2/Q3 2025 has been defined following a thorough evaluation, and we’re glad to announce you that Dwellir is included in this selection.

**At this point we need from your side the beneficiary addresses for both Moonbeam and Moonriver to trigger our Payment operations accordingly.**

Once again, thank you for your proposal and your continued partnership!!!

Best regards,  
Michele, on behalf of the Treasury Council

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/9?u=_yrn "Post date")

Thank you for entrusting us! We’re very honoured to grow with Moonbeam.

The beneficiary address for both GLMR and MOVR is:

0xF8D757E04BF0fbd5432E743DD8612E62A9c983cf## ABSTRACT

Dwellir is committed to empowering developers worldwide by providing instant data access and robust infrastructure tailored for web3 applications. With extensive experience supporting Moonbeam, Moonriver, Moonbase Alpha, and over 100 other blockchain networks, Dwellir sets itself apart through its ownership and operation of dedicated bare metal servers. This infrastructure approach ensures superior performance, enhanced security, full control over configurations, and consistent reliability.

This proposal specifically seeks funding to continue providing fully managed Public Archival RPC services for the Moonbeam ecosystem, utilizing distinct and specialized node software that ensures optimal performance and security. Our infrastructure, strategically located across data centers in Sweden, Tunisia, and Singapore, guarantees high availability, fault tolerance, efficient load balancing, and seamless operational continuity during maintenance periods.

Recognized globally for exceptional geographical performance, Dwellir’s service has processed over 4.2 billion requests for the Moonbeam ecosystem from Q4 2024 to Q1 2025 alone, demonstrating proven capability and robust scalability.

The proposed budget of $10,913.06 for six months covers comprehensive operational requirements, including traffic management, storage, memory allocation, and CPU utilization, ensuring continuous, enterprise-level service delivery that directly contributes to the reliability and growth of the Moonbeam blockchain community.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-motivation-2)MOTIVATION

The Dwellir mission is to serve developers worldwide with instant data access and a comprehensive suite of tools so that they can build web3 applications.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-project-overview-and-experience-3)PROJECT OVERVIEW AND EXPERIENCE

We currently run RPC services for Moonbeam, Moonriver and Moonbase Alpha and more than 150 other blockchain networks. Currently, we are processing 1.4 billion requests per day on average and you will see throughout this proposal that our experience within the Moonbeam ecosystem is extensive.

One of the key differentiators with Dwellir is that we own and operate our own bare metal machines which have several important effects.

Performance: Bare metal servers offer superior performance and low-latency communication, essential for decentralized networks to efficiently process transactions and reach consensus.

Security: Bare metal servers provide enhanced security and isolation, safeguarding sensitive data and assets in a decentralized network.

Control: With bare metal servers, node operators have full control over hardware and software configurations, ensuring adherence to network rules and consensus mechanisms.

Reliability: Bare metal servers offer robustness and stability, making them reliable choices for continuous operation in decentralized networks.

Expertise: Our team has a proven track record of creating tailor-made blockchain infrastructure that align with the Moonbeam community’s specific needs.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-relevant-news-4)RELEVANT NEWS

Dwellir has introduced GEO load balancing between our nodes in Europe and APAC (Singapore), ensuring a faster and more reliable experience for our users. By routing traffic to the closest and most responsive node, we minimize latency and enhance performance for Moonbeam applications. This upgrade strengthens our commitment to the community.

The new GEO load-balanced RPC endpoints have new URLs. Please update your configurations to the new URLs:

-   Moonbeam:  [moonbeam-rpc.n.dwellir.com](http://moonbeam-rpc.n.dwellir.com/)
-   Moonriver:  [moonriver-rpc.n.dwellir.com](http://moonriver-rpc.n.dwellir.com/)
-   Moonbase:  [moonbase-rpc.n.dwellir.com](http://moonbase-rpc.n.dwellir.com/)

The old endpoints (*.dwellir.com without .n.) will be decommissioned soon, so we strongly recommend switching to the new addresses as soon as possible to ensure uninterrupted service.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-service-statistics-5)SERVICE STATISTICS

[![Screenshot 2025-03-14 at 08.38.34](https://forum.moonbeam.network/uploads/db2361/optimized/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d_2_411x500.png)](https://forum.moonbeam.network/uploads/db2361/original/2X/0/041183d63b2e3b0385fa1cb8e4b756e7ef59501d.png "Screenshot 2025-03-14 at 08.38.34")

Screenshot 2025-03-14 at 08.38.34638×776 95.4 KB

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-overall-cost-6)OVERALL COST

The total budget for the proposal is  **$10,913.06**  for Q2 and Q3 of 2025, covering:  
**$1,818.84 per month**  for RPC services, boot nodes, and infrastructure maintenance.

Monthly Subtotal

$1,732.23

Monthly Operations (5%)

$86.61

Monthly Total

$1,818.84

Quarterly Total

$5,456.53

Six Months Total

$10,913.06

_This includes all three services across three geographical regions (Europe, Asia, North Africa). More detailed costs in the full proposal._

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-specifications-7)SPECIFICATIONS

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-connections-and-node-methods-8)Connections and Node Methods

Dwellir sets max connections to 10,000 concurrent WebSockets. From time to time we increase this to 30,000 to deal with events such as the ordinals rush.

Dwellir maintains multiple 2 Gigabit external connections with the option to raise this to 10 Gigabit.

Dwellir allows for tracing methods including eth_getLogs as standard.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-location-of-nodes-9)Location of Nodes

Dwellir owns all of our own hardware and current we host services across data centers in four locations:

1.  Sweden (site 1)
2.  Sweden (site 2)
3.  Tunisia
4.  Nigeria*
5.  Singapore

*Nigeria is where we host services that are connected to the IBP program. These services ARE NOT included in this proposal. We DO NOT use that datacenter or equipment in order to fulfill other proposals.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-use-of-treasury-funds-10)USE OF TREASURY FUNDS

To cover the costs of hardware operation and maintenance. We own and operate our own bare metal services in 4 locations.

### [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-deliverables-11)Deliverables

-   **RPC endpoints**  continuously maintained for Moonbeam, Moonriver, and Moonbase-Alpha with near 100% uptime.
-   **Bootnodes**  - already up and running for seamless peer-to-peer network connectivity.

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-requirements-12)REQUIREMENTS

Estimated call volumes = 4.2 billion  
Pricing in USD denomination = USD $10,913.06  
Inclusion of the  `eth_getLogs`  RPC method : YES  
Information about bootnode operation on all three networks: YES for all networks

**Cost for 6-months: USD $10,913.06**

## [](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8#p-7010-link-to-full-proposal-13)LINK TO FULL PROPOSAL

[Link to full proposal](https://docs.google.com/document/d/1eRs7ey7Qwl-JWSO2Yl9oBGHB6HTe5qFYpSteCirO2e4/edit?usp=sharing)

  

1 Reply

1​

​​Reply

66views13likes1link

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png "benn_69")](https://forum.moonbeam.network/u/benn_69 "benn_69")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png "aaron.mbf")](https://forum.moonbeam.network/u/aaron.mbf "aaron.mbf")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[18d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/2?u=_yrn "Post date")

Hey  [@benn_69](https://forum.moonbeam.network/u/benn_69)! Thanks for your submission, much appreciated!  
Quick rapid fire Q — Would you consider to route calls to the old Dwellir endpoint URLs fwd to the new ones internally, instead of decommissioning them entirely? That would be awesome.  
RPC URL configs like these tend to be sticky among users and dApps which might cause some issues and possibly lead to a significant decrease in calls to the Dwellir endpoints with fallbacks in place.  
Thanks so much so for your submission! You’ll be hearing from us soon™️

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/3?u=_yrn "Post date")

[@benn_69](https://forum.moonbeam.network/u/benn_69)  sorry to bump this, but I’d appreciate a quick thumbs up or down on the endpoint null routing issue as the Treasury Council is keen to conclude its decision process in time. Thank you!

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/4?u=_yrn "Post date")

We can fix a solution so that other users can use previous URLs and we will route traffic.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[11d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/5?u=_yrn "Post date")

That’s awesome, thanks!  ![:raised_hands:](https://forum.moonbeam.network/images/emoji/twitter/raised_hands.png?v=12 ":raised_hands:")

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png)](https://forum.moonbeam.network/u/aaron.mbf)

[aaron.mbf](https://forum.moonbeam.network/u/aaron.mbf)[Technical Council member](https://forum.moonbeam.network/g/TreasuryCouncil)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/6?u=_yrn "Post date")

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/48/109_2.png)  benn_69:

> SERVICE STATISTICS

Any idea why the sudden drop in requests to Moonbeam in December?

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[8d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/7?u=_yrn "Post date")

Nothing obvious stands out on our end. We occasionally see similar behavior across our services.

Toward the end of last year, we had discussions with several wallet providers (Talisman, Subwallet, and Fearless) to help optimize their RPC calls to our nodes, which could have contributed to this change.

It’s also possible that some public usage shifted toward our API service—we’ve noticed increased activity there.

**TL;DR:**  Our team hasn’t identified any significant insights from available reports.

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/8?u=_yrn "Post date")

Dear  [@Benn_69](https://forum.moonbeam.network/u/benn_69),

I am writing you on behalf of the Treasury Council.

First and foremost, we would like to express our sincere appreciation for your proposal. We recognize the considerable effort that went into it.

After careful consideration over the past few days, the Council members have reached a final decision: for the upcoming Q2/Q3 2025 period, we will be funding only 2 RPC teams (down from 3 in the previous period), based on the following factors:

-   Current market conditions, which require us to be cost-conscious.
-   A reduction in overall activity due to lower market conditions.
-   IBP services, which are already covered by the Polkadot treasury.

A shortlist of 2 providers for Q2/Q3 2025 has been defined following a thorough evaluation, and we’re glad to announce you that Dwellir is included in this selection.

**At this point we need from your side the beneficiary addresses for both Moonbeam and Moonriver to trigger our Payment operations accordingly.**

Once again, thank you for your proposal and your continued partnership!!!

Best regards,  
Michele, on behalf of the Treasury Council

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/benn_69/96/109_2.png)](https://forum.moonbeam.network/u/benn_69)

[benn_69](https://forum.moonbeam.network/u/benn_69)

[5d](https://forum.moonbeam.network/t/dwellir-s-proposal-for-moonbeam-moonriver-and-moonbase-alpha-rpc-services-q2-q3-2025/2041/9?u=_yrn "Post date")

Thank you for entrusting us! We’re very honoured to grow with Moonbeam.

The beneficiary address for both GLMR and MOVR is:

0xF8D757E04BF0fbd5432E743DD8612E62A9c983cff
