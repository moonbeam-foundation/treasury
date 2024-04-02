
Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and Moonbase Alpha. This initiative rapidly gained traction within the user and developer community, with the RPC serving over 5 billion requests in 2H2023 across all three chains. 4Q2023 saw a drop in requests from 3Q2023, but we saw a trend reversal in December, and currently as of January 10th holding at over 1Bln requests in the trailing 30 days.

On October 3rd UnitedBloc was [selected by the Moonbeam Treasury Council](https://forum.moonbeam.network/t/q2-q3-rpc-service-provider-treasury-proposals/1114/37) as one of the supported RPC providers for Q4 2023 and Q1 2024.

Motivation - Our first objective is to foster Moonbeam’s growth, it’s crucial for developers to have seamless access to top-tier RPC services. Our free public RPC service serves as a stepping stone, supporting new developers as they launch and expand their projects. No signup. No accounts or accounting, just point the app to a UB endpoint and go. If at any point the project RPC requirements exceed our capacity, we’ll guide them toward commercial service providers. Our second objective is to facilitate the RPC needs of non-profit endeavors. If community focused non-profits ever need more RPC than our public service provides, we will work with them to meet the need.

Project Overview and Team Experience - UnitedBloc members excel in Linux administration, allowing us to deploy robust servers. Each member organization takes responsibility for deploying and maintaining their individual RPC servers. This approach leverages our collective expertise for a decentralized network architecture.

Overall Cost - This proposal encompasses combined operational costs for Moonbeam, Moonriver, and Moonbase Alpha for Q1 2024. The total requested amount is $5,400 (50% of Q3/Q4), and we request 7,805.35 GLMR($3,240 USD) and 109.40 MOVR ($2,160 USD) in a 60/40 split using a TWAP 30 day from Jan 11th (Coinmarketcap data). UnitedBloc has elected to offer a one-time reduction in the Q1 proposal of 50% due to the recent market increase and efficient UB treasury management.

Metrics

Month Combined WS + HTTP RPC Calls

October ~692,000,000

November ~545,000,000

December ~982,000,000

Quarterly Total 2,219,000,000

Use of Treasury Funds - As community collators reliant on community delegations, we have launched the RPC service to give back, operating with a non-profit focus. This grant covers our infrastructure costs for the RPC service across Moonbeam, Moonriver, and Moonbase Alpha, including the provision of boot nodes for all three networks. It excludes any margin or profit for UnitedBloc.

Specifications - The UnitedBloc RPC service encompasses four regions: North and South America, Europe, and Asia-Pacific. In December the service responded to nearly 1 billion calls across all three networks. We employ global DNS load balancing to efficiently route users to UnitedBloc servers in their respective regions. Within each region, OpenResty enhances RPC requests with additional load balancing and optimization. When demand surges, we promptly adjust by adding more servers or specific services. Our design is thus scalable, flexible, and cost effective.

We provide our endpoints at the following addresses:

[https://moonbase.unitedbloc.com](https://moonbase.unitedbloc.com)

wss://moonbase.unitedbloc.com

[https://moonriver.unitedbloc.com](https://moonriver.unitedbloc.com)

wss://moonriver.unitedbloc.com

[https://moonbeam.unitedbloc.com](https://moonbeam.unitedbloc.com)

wss://moonbeam.unitedbloc.com

Steps to Implement - Our public RPC service has been fully operational, serving the community since early 2023.

UnitedBloc Linktree: [unitedbloc | Twitter | Linktree 1](https://linktr.ee/unitedbloc)