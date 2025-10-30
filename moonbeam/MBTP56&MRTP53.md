# [[Proposal: MBXX/MRXX] UnitedBloc - Treasury Proposal for Q4/Q1 2026](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q4-q1-2026/2294)

[Governance](https://forum.moonbeam.network/c/governance/2)[Treasury Proposals](https://forum.moonbeam.network/c/governance/treasury-proposals/8)

[moonbeam](https://forum.moonbeam.network/tag/moonbeam)[moonriver](https://forum.moonbeam.network/tag/moonriver)[moonbase-alpha](https://forum.moonbeam.network/tag/moonbase-alpha)

44views12likes1link

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png "blackk_magiik")](https://forum.moonbeam.network/u/blackk_magiik "blackk_magiik")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[Oct 11](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q4-q1-2026/2294/1 "Jump to the first post")

[6d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q4-q1-2026/2294/4)

​

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

1

[19d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q4-q1-2026/2294?u=_yrn "Post date")

**Forum Post: UnitedBloc - Treasury Proposal for Q4/Q1 2026**

**Abstract -**  UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and Moonbase Alpha. Estimated call volumes have been in line with previous quarters, estimated between 600M and 1B per month, across all networks, with calls heavily weighted to Moonbeam network. Calls have remained steady over the past few months, with a slight decline in the lower half of 2024, likely due to markets remaining fairly static.

On October 3rd 2023 UnitedBloc was  [selected by the Moonbeam Treasury Council](https://forum.moonbeam.network/t/q2-q3-rpc-service-provider-treasury-proposals/1114/37)  as one of the supported RPC providers for Q4 2023, Q1-Q4 2024, Q1-Q3 2025

**Motivation -**  Our first objective is to foster Moonbeam’s growth, it’s crucial for developers to have seamless access to top-tier RPC services. Our free public RPC service serves as a stepping stone, supporting new developers as they launch and expand their projects. No signup. No accounts or accounting, just point the app to a UB endpoint and go. If at any point the project RPC requirements exceed our capacity, we’ll guide them toward commercial service providers. Our second objective is to facilitate the RPC needs of non-profit endeavors. If community focused non-profits ever need more RPC than our public service provides, we will work with them to meet the need.

**Project Overview and Team Experience -**  UnitedBloc members excel in Linux administration, allowing us to deploy robust servers. Each member organization takes responsibility for deploying and maintaining their individual RPC servers. This approach leverages our collective expertise for a decentralized network architecture.

**Overall Cost**  - This proposal encompasses combined operational costs for Moonbeam, Moonriver, and Moonbase Alpha for Q4/Q1 2026. The total requested amount per quarter is $7,000 ($14,000 for Q4/Q1 2026 combined) This is a 35% proposal cost decrease compared to previous quarters due to reduced RPC demand and deploying newer servers. This includes operating costs for 14 nodes spread across the 3 networks and 3 continents, at $325/node. The difference in the full charge to MBF is composed of GSLB DNS load balancing and KPI monitoring costs. Additionally, the price includes the day-to-day support costs for maintaining the nodes which includes client upgrades, troubleshooting assistance, and community engagement.

**Metrics**

Combined WS + HTTP RPC Calls

_June 2025_

_July 2025_

August 2025

_**Quarterly Total**_

**Use of Treasury Funds -**  As community collators reliant on community delegations, we have launched the RPC service to give back, operating with a non-profit focus. This grant covers our infrastructure costs for the RPC service across Moonbeam, Moonriver, and Moonbase Alpha. It excludes any margin or profit for UnitedBloc.

**Specifications -**  The UnitedBloc RPC service encompasses four regions: North and South America, Europe, and Asia-Pacific. We employ global DNS load balancing to efficiently route users to UnitedBloc servers in their respective regions. Within each region, OpenResty enhances RPC requests with additional load balancing and optimization. When demand surges, we promptly adjust by adding more servers or specific services. Our design is thus scalable, flexible, and cost effective.

RPC Services Inclusion:

-   Bootnodes on all 3 networks
    
-   Eth_getlogs
    
-   Trace calling
    

We provide our endpoints at the following addresses:

[https://moonbase.unitedbloc.com](https://moonbase.unitedbloc.com/)

wss://moonbase.unitedbloc.com

[https://moonriver.unitedbloc.com](https://moonriver.unitedbloc.com/)

wss://moonriver.unitedbloc.com

[https://moonbeam.unitedbloc.com](https://moonbeam.unitedbloc.com/)

wss://moonbeam.unitedbloc.com

**Steps to Implement -**  Our public RPC service has been fully operational, serving the community since early 2023.

UnitedBloc Linktree:  [https://linktr.ee/unitedbloc](https://linktr.ee/unitedbloc)