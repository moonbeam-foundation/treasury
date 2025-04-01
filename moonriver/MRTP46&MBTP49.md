[Proposal: MBXX/MRXX] UnitedBloc - Treasury Proposal for Q2/Q3 2025


Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and Moonbase Alpha. Estimated call volumes have been in line with previous quarters, estimated between 600M and 1B per month, across all networks, with calls heavily weighted to Moonbeam network. Calls have remained steady over the past few months, with a slight decline in the lower half of 2024, likely due to markets remaining fairly static.

On October 3rd 2023 UnitedBloc was  [selected by the Moonbeam Treasury Council](https://forum.moonbeam.network/t/q2-q3-rpc-service-provider-treasury-proposals/1114/37)  as one of the supported RPC providers for Q4 2023, Q1-Q4 2024, Q1 2025

Motivation - Our first objective is to foster Moonbeam’s growth, it’s crucial for developers to have seamless access to top-tier RPC services. Our free public RPC service serves as a stepping stone, supporting new developers as they launch and expand their projects. No signup. No accounts or accounting, just point the app to a UB endpoint and go. If at any point the project RPC requirements exceed our capacity, we’ll guide them toward commercial service providers. Our second objective is to facilitate the RPC needs of non-profit endeavors. If community focused non-profits ever need more RPC than our public service provides, we will work with them to meet the need.

Project Overview and Team Experience - UnitedBloc members excel in Linux administration, allowing us to deploy robust servers. Each member organization takes responsibility for deploying and maintaining their individual RPC servers. This approach leverages our collective expertise for a decentralized network architecture.

Overall Cost - This proposal encompasses combined operational costs for Moonbeam, Moonriver, and Moonbase Alpha for Q2/Q3 2025. The total requested amount per quarter is $7,000 ($14,000 for Q2/Q3 combined) This is a 35% proposal cost decrease compared to previous quarters due to reduced RPC demand and deploying newer servers. This includes operating costs for 14 nodes spread across the 3 networks and 3 continents, at $325/node. The difference in the full charge to MBF is composed of GSLB DNS load balancing and KPI monitoring costs. Additionally, the price includes the day-to-day support costs for maintaining the nodes which includes client upgrades, troubleshooting assistance, and community engagement.

Metrics

Combined WS + HTTP RPC Calls

December 2024

~982,000,000

January 2025

~ 972,100,000

February 2025

~ 768,500,000

Quarterly Total 1,741,582,000

Use of Treasury Funds - As community collators reliant on community delegations, we have launched the RPC service to give back, operating with a non-profit focus. This grant covers our infrastructure costs for the RPC service across Moonbeam, Moonriver, and Moonbase Alpha. It excludes any margin or profit for UnitedBloc.

Specifications - The UnitedBloc RPC service encompasses four regions: North and South America, Europe, and Asia-Pacific. We employ global DNS load balancing to efficiently route users to UnitedBloc servers in their respective regions. Within each region, OpenResty enhances RPC requests with additional load balancing and optimization. When demand surges, we promptly adjust by adding more servers or specific services. Our design is thus scalable, flexible, and cost effective.

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

Steps to Implement - Our public RPC service has been fully operational, serving the community since early 2023.

UnitedBloc Linktree:  [unitedbloc | Twitter | Linktree](https://linktr.ee/unitedbloc)

  

4​

​​Reply

57views9likes1link

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png "blackk_magiik")](https://forum.moonbeam.network/u/blackk_magiik "blackk_magiik")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

14 days later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[5d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q2-q3-2025/2035/2?u=_yrn "Post date")

Dear  [@Blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik),

I am writing you on behalf of the Treasury Council.

First and foremost, we would like to express our sincere appreciation for your proposal. We recognize the considerable effort that went into it.

After careful consideration over the past few days, the Council members have reached a final decision: for the upcoming Q2/Q3 2025 period, we will be funding only 2 RPC teams (down from 3 in the previous period), based on the following factors:

-   Current market conditions, which require us to be cost-conscious.
-   A reduction in overall activity due to lower market conditions.
-   IBP services, which are already covered by the Polkadot treasury.

A shortlist of 2 providers for Q2/Q3 2025 has been defined following a thorough evaluation, and we’re glad to announce you that UB is included in this selection.

**At this point we need from your side the beneficiary addresses for both Moonbeam and Moonriver to trigger our Payment operations accordingly.**

Once again, thank you for your proposal and your continued partnership!!!

Best regards,  
Michele, on behalf of the Treasury Council

  

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[5d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q2-q3-2025/2035/3?u=_yrn "Post date")

Thank you  [@micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)  and MBF crew!! We as always continually appreciate the support and confidence MBF has in UB’s RPC services.

  

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[4d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q2-q3-2025/2035/4?u=_yrn "Post date")

You’re more than welcome !!!  
Whenever you can please share beneficiary addresses for both MB & MR!

Thanks again!

  

​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[4d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-unitedbloc-treasury-proposal-for-q2-q3-2025/2035/5?u=_yrn "Post date")

[@micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)  Ha whoops, guess I am bad at requesting to getting paid. Here you go good sir!

mbeam:0xfD346Be6cd55247D4b928656E0DCdC10C1660434

mriver:0x2b0B08fE83fADCAffd49dfB433244ad670c2D3ba
