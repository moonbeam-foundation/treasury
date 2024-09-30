[Proposal: MB 35/MR 31] UnitedBloc - Treasury Proposal for Q4 2024/Q1 2025

Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and Moonbase Alpha. This initiative rapidly gained traction within the user and developer community. The RPC service responded to over 10 billion* requests in 1H2024 across all three chains. Calls have remained steady over the past few months, with a slight decline in February, likely due to markets remaining fairly static.

On October 3rd UnitedBloc was selected by the Moonbeam Treasury Council as one of the supported RPC providers for Q4 2023 and Q1 2024-Q1 2025.

Motivation - Our first objective is to foster Moonbeam’s growth, it’s crucial for developers to have seamless access to top-tier RPC services. Our free public RPC service serves as a stepping stone, supporting new developers as they launch and expand their projects. No signup. No accounts or accounting, just point the app to a UB endpoint and go. If at any point the project RPC requirements exceed our capacity, we’ll guide them toward commercial service providers. Our second objective is to facilitate the RPC needs of non-profit endeavors. If community focused non-profits ever need more RPC than our public service provides, we will work with them to meet the need.

Project Overview and Team Experience - UnitedBloc members excel in Linux administration, allowing us to deploy robust servers. Each member organization takes responsibility for deploying and maintaining their individual RPC servers. This approach leverages our collective expertise for a decentralized network architecture.

Overall Cost - This proposal encompasses combined operational costs for Moonbeam, Moonriver, and Moonbase Alpha for Q4 2024/Q1 2025. The total requested amount per quarter is $10,800, and we request 38,802.40 GLMR ($6,480 USD) and 488.85 MOVR ($4,320 USD) in a 60/40 split using a TWAP 30D of $0.167 for GLMR and of $8.837 for MOVR, as of August 29th, 2024 (CoinGecko data).

Metrics

Metrics 2024Q2

Combined WS + HTTP RPC Calls across all chains

Apr 2024

~1,590M

May 2024

~5,162M*

June 2024
    1,212M

Screenshot 2024-08-30 063546

    May was an anomalous month due to two separate network attacks on our RPC services. Both were DoS attacks, with a DDoS attack originating from various locations in E/SE-Asia and a second DoS attack connecting over WS to our US-W node.

In both events, each attack only limited services in one region, and while we never want to see a degraded service, this was a good stress test and in many ways proved the robustness of our implementation. It also showed that we have a very high ceiling before load becomes an issue with our globally distributed RPC service. Regardless, we have implemented additional limits and other protections to our base configuration which will only be triggered in the event that there is abuse of the service.

Metrics 2024Q3

Combined WS + HTTP RPC Calls

July 2024

~922M

Aug 2024

TBD

Sept 2024

TBD

Quarterly Total: TBD

Use of Treasury Funds - As community collators reliant on community delegations, we have launched the RPC service to give back, operating with a non-profit focus. This grant covers our infrastructure costs for the RPC service across Moonbeam, Moonriver, and Moonbase Alpha, including the provision of boot nodes for all three networks. It excludes any margin or profit for UnitedBloc.

Specifications - The UnitedBloc RPC service encompasses four regions: North and South America, Europe, and Asia-Pacific. In 2Q2024 the service responded to over 6.375 billion calls across all three networks (note: more than 40% of these calls were likely not legitimate calls and due to network attacks on our service, more detail is provided in a previous section). The data for 3Q2024 is currently not complete, but is trending downward to ~2.8B calls, in line with the wider industry slowdown. We employ global DNS load balancing to efficiently route users to UnitedBloc servers in their respective regions. We also include eth_getLogs at no additional costs across all 3 networks. Within each region, OpenResty enhances RPC requests with additional load balancing and optimization. When demand surges, we promptly adjust by adding more servers or specific services. Our design is thus scalable, flexible, and cost effective.

We provide our endpoints at the following addresses:

https://moonbase.unitedbloc.com 1

wss://moonbase.unitedbloc.com

https://moonriver.unitedbloc.com

wss://moonriver.unitedbloc.com

https://moonbeam.unitedbloc.com 2

wss://moonbeam.unitedbloc.com

Steps to Implement - Our public RPC service has been fully operational, serving the community since early 2023.

The full proposal can be found here: UB Moonbeam RPC proposal - Retroactive Funding Proposal for Q3 2023 - Google Docs 4

UnitedBloc Linktree: unitedbloc | Twitter | Linktree
HTML selection 1 characters 1 words 1 paragraphs
