
[Proposal: MB 35/MR 31] UnitedBloc - Treasury Proposal for Q4 2024/Q1 2025

Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and Moonbase Alpha. This initiative rapidly gained traction within the user and developer community. The RPC service responded to over 10 billion* requests in 1H2024 across all three chains. Calls have remained steady over the past few months, with a slight decline in February, likely due to markets remaining fairly static.

On October 3rd UnitedBloc was  [selected by the Moonbeam Treasury Council](https://forum.moonbeam.network/t/q2-q3-rpc-service-provider-treasury-proposals/1114/37)  as one of the supported RPC providers for Q4 2023 and Q1 2024-Q1 2025.

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

~ 1,212M

![Screenshot 2024-08-30 063546](https://forum.moonbeam.network/uploads/db2361/original/2X/3/3f981ef48ba7ca9234ee33c8c41062c4a889a6a7.png)

-   May was an anomalous month due to two separate network attacks on our RPC services. Both were DoS attacks, with a DDoS attack originating from various locations in E/SE-Asia and a second DoS attack connecting over WS to our US-W node.

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

[https://moonbase.unitedbloc.com](https://moonbase.unitedbloc.com/)

wss://moonbase.unitedbloc.com

[https://moonriver.unitedbloc.com](https://moonriver.unitedbloc.com/)

wss://moonriver.unitedbloc.com

[https://moonbeam.unitedbloc.com](https://moonbeam.unitedbloc.com/)

wss://moonbeam.unitedbloc.com

Steps to Implement - Our public RPC service has been fully operational, serving the community since early 2023.

The full proposal can be found here:  [UB Moonbeam RPC proposal - Retroactive Funding Proposal for Q3 2023 - Google Docs](https://docs.google.com/document/d/1hepttv39uZu0iLUVHQychuhsg0SnhYSmmFlOQTIwvbs)

UnitedBloc Linktree:  [unitedbloc | Twitter | Linktree](https://linktr.ee/unitedbloc)

  

3​

​​Reply

-   [[Proposal: XX] RadiumBlock RPC and Bootnode Services for Moonbeam, Moonriver, and Moonbase-alpha for Q4 2024/Q1 2025](https://forum.moonbeam.network/t/proposal-xx-radiumblock-rpc-and-bootnode-services-for-moonbeam-moonriver-and-moonbase-alpha-for-q4-2024-q1-2025/1827/11)
-   [Treasury Transparency Report 2024 H2](https://forum.moonbeam.network/t/treasury-transparency-report-2024-h2/1978)

163views28likes6links6users

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png "blackk_magiik")](https://forum.moonbeam.network/u/blackk_magiik "blackk_magiik")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png "aaron.mbf")](https://forum.moonbeam.network/u/aaron.mbf "aaron.mbf")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/dev0_sik/96/37_2.png "dev0_sik")](https://forum.moonbeam.network/u/dev0_sik "dev0_sik")

read4  min

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/2?u=_yrn "Post date")

Dear  [@blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)  ,

The  [@TreasuryCouncil](https://forum.moonbeam.network/groups/treasurycouncil)  would like to thank you for submitting the above RPC service proposal!

I am starting here a round of questions / feedback, other Treasury members could join afterwards.

With reference to your proposal my question is specifically about this point you reported in the proposal:

“ * May was an anomalous month due to two separate network attacks on our RPC services. Both were DoS attacks, with a DDoS attack originating from various locations in E/SE-Asia and a second DoS attack connecting over WS to our US-W node.

In both events, each attack only limited services in one region, and while we never want to see a degraded service, this was a good stress test and in many ways proved the robustness of our implementation. It also showed that we have a very high ceiling before load becomes an issue with our globally distributed RPC service. Regardless, we have implemented additional limits and other protections to our base configuration which will only be triggered in the event that there is abuse of the service."

Can you kindly better describe/detail which kind of additional limits/protections did you implement ?

To stay on schedule we’d appreciate a reply in a timely manner, ideally by next Monday, September 9th.

Thanks & kind regards  
Michele

  

​

​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/3?u=_yrn "Post date")

[@micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)  We noticed some peculiar WSS connections so we implemented a memory utilization improvement along with some best security practices pertaining to WSS/HTTP type connections. This seemed to have helped with stability.

  

​

1​

​​Reply

16 days later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/lina.k.m/96/116_2.png)](https://forum.moonbeam.network/u/lina.k.m)

[lina.k.m](https://forum.moonbeam.network/u/lina.k.m)Treasury Council Member

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/4?u=_yrn "Post date")

Hi  [@blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik), the Treasury Council has carefully reviewed your proposal and, considering your key strengths in decentralization, latency, and availability, we are pleased to inform you that you are among the three RPC providers selected for Q4 2024 / Q1 2025. This message serves as your first support signal, with two additional signals to follow soon. We will also provide the 30-day moving average price information to assist you in preparing your on-chain proposal.  
While we noted that your pricing was on the higher side and that the package does not include trace+API, your extensive geographic coverage, quality of service, and the completeness of your offering (including boot nodes and eth.getLogs), along with your active participation in the Moonbeam community, made your proposal stand out. We are glad to have you guys onboard!

  

2 Replies

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/5?u=_yrn "Post date")

Signaling support, marking  #2  out of 3.

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/lina.k.m/48/116_2.png "lina.k.m")lina.k.m

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/6?u=_yrn "Post date")

Hi  [@lina.k.m](https://forum.moonbeam.network/u/lina.k.m)  Thank you!! UnitedBloc is greatly appreciative of Moonbeams continued support! Also UB does offer trace on RPC nodes, but if its trace with some sort of API functionality then you are correct.

  

1 Reply

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aaron.mbf/96/70_2.png)](https://forum.moonbeam.network/u/aaron.mbf)

[aaron.mbf](https://forum.moonbeam.network/u/aaron.mbf)[Technical Council member](https://forum.moonbeam.network/g/TreasuryCouncil)

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/7?u=_yrn "Post date")

Also signaling support (3 of 3). 30 day moving average to come shortly.

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/48/1067_2.png "blackk_magiik")blackk_magiik

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/8?u=_yrn "Post date")

Dear  [@blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)  please find here below the 30dma info:

GLMR price: 0.166 USD  
MOVR price: 9.38 USD

Please create accordingly your On-chain proposals.

Deadline for such creation: Tuesday 24th

Thanks a lot in advance!!!

BR

Michele

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/9?u=_yrn "Post date")

thanks  [@micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)  !! I am assuming this is only for Q4 filing and we file Q1 2025 at a later date?

  

2 Replies

​

​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/10?u=_yrn "Post date")

Exactly:  
Onchain proposals to be created now is only about Q4 2024 Payments!

Thanks!!!

BR

Michele

  

​

​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[Sep 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/11?u=_yrn "Post date")

submitted!

![](https://forum.moonbeam.network/uploads/db2361/original/2X/1/17efd57479b8b91a90f74027a8b98d8993434916.png)[moonbeam.polkassembly.network](https://moonbeam.polkassembly.network/treasury/35)

![](https://forum.moonbeam.network/uploads/db2361/original/2X/1/1f4436a1b9cda705e2f8b0ba3629b4bbfe43d6b4.png)

### [UnitedBloc - Treasury Proposal for Q4 2024/Q1 2025](https://moonbeam.polkassembly.network/treasury/35)

This is for Q4 2024 treasury submission Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam,...

![](https://forum.moonbeam.network/uploads/db2361/original/2X/d/d9614a3e4b62743713430d63c935851e3dec8c59.png)[moonriver.polkassembly.network](https://moonriver.polkassembly.network/treasury/31)

![](https://forum.moonbeam.network/uploads/db2361/original/2X/8/825dc30b3d522eceb545fba7bf2ffa4b3164b2ca.png)

### [UnitedBloc - Treasury Proposal for Q4 2024/Q1 2025](https://moonriver.polkassembly.network/treasury/31)

This is for Q4 treasury submission Abstract - UnitedBloc is a group of community collators who have been actively involved with Moonbeam since the early testnet phase. In early 2023, we introduced our public RPC service for Moonbeam, Moonriver, and...

  

​

1​

​​Reply

11 days later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[Oct 2024](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/12?u=_yrn "Post date")

Treasury Council voting operations completed: proposal approved Onchain!

  

​

1​

​​Reply

2 months later

[![](https://forum.moonbeam.network/uploads/db2361/original/2X/7/7ee46540c2162817dc30b8372c64f8bb81307cea.png "system")](https://forum.moonbeam.network/u/system)

Closed  on Dec 4, 2024

This topic was automatically closed 60 days after the last reply. New replies are no longer allowed.

  

1 month later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

1

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/48/1067_2.png "blackk_magiik")blackk_magiik

[Jan 10](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/14?u=_yrn "Post date")

> I am assuming this is only for Q4 filing and we file Q1 2025 at a later date?

Dear  [@blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik),

the day has come!

Please proceed with submitting your Treasury Proposal for the RPC services Q1 2025 payout on-chain. As before, please split the agreed quarterly cost in a 60/40 ratio between GLMR and MOVR using the EMA30 prices below.

GLMR: $ 0.265  
MOVR: $ 13.716

As per today’s Subscan data (provided by Coingecko) for  [MOVR](https://moonriver.subscan.io/tools/price_converter?value=1&type=time&from=MOVR&to=USD&time=1736463600)  and  
[GLMR](https://moonbeam.subscan.io/tools/price_converter?value=1&type=time&from=GLMR&to=USD&time=1736463600).

Once on-chain, we will make sure the Proposal is converted to a Council Motion and payed out asap.

Thank you so much!  
Yaron

  

​

2

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/lina.k.m/48/116_2.png "lina.k.m")](https://forum.moonbeam.network/u/lina.k.m)

Opened  on Jan 14

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/dev0_sik/96/37_2.png)](https://forum.moonbeam.network/u/dev0_sik)

[dev0_sik](https://forum.moonbeam.network/u/dev0_sik)Treasury Council Member

[Jan 14](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/16?u=_yrn "Post date")

Hey UB - please hold off from submitting treasury proposals right now.  
With runtime 3300 the treasury.propose extrinsic was somehow removed rendering it unable to submit a spending proposal directly to the treasury (which is required to transform it into a motion by the treasury council).

We’ll keep you posted and sorry for the inconvenience and delays caused by this.  ![:pray:](https://forum.moonbeam.network/images/emoji/twitter/pray.png?v=12 ":pray:")

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png)](https://forum.moonbeam.network/u/blackk_magiik)

[blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)

[Jan 15](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/17?u=_yrn "Post date")

Thanks  [@dev0_sik](https://forum.moonbeam.network/u/dev0_sik)  for the heads up

  

​

2​

​​Reply

1 month later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[3d](https://forum.moonbeam.network/t/proposal-mb35-mr-31-unitedbloc-treasury-proposal-for-q4-2024-q1-2025/1828/18?u=_yrn "Post date")

Hey  [@blackk_magiik](https://forum.moonbeam.network/u/blackk_magiik)  ![:magic_wand:](https://forum.moonbeam.network/images/emoji/twitter/magic_wand.png?v=12 ":magic_wand:")

RT3401 is now enacted on both Moonbeam and Moonriver and the Treasury Council is ready to conduct your awaited payouts via the new  [Treasury Proposal flow](https://forum.moonbeam.network/t/runtime-rt3400-schedule/1954/6).

For that matter, please provide us with a beneficiary address of your choice and the Treasury Council will process your proposal asap.

We’ve captured the EMA30 price for MOVR at $ 8.483093 at block  [10380992](https://moonriver.subscan.io/tools/price_converter?value=1&type=block&from=MOVR&to=USD&time=10380992)  and at $ 0.150840 at  [9673865](https://moonbeam.subscan.io/tools/price_converter?value=1&type=block&from=GLMR&to=USD&time=9673865)  for GLMR.

This will result in a total payout of 85,918.85 GLMR and 1,018.50 MOVR to settle your request of $ 21,600.

Again, thanks you for your patience!  
yaron
