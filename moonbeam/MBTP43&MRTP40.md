
[esantos089](https://forum.moonbeam.network/u/esantos089)

[29d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998?u=_yrn "Post date")

**Title**  - [Proposal:] [Status: Submitted] Moonbeam Multisig Support as a Service: Moonbeam, Moonriver, and Moonbase for 2nd Semester/2024.

Moonbeam Multisig Official Link:  [https://multisig.moonbeam.network](https://multisig.moonbeam.network/)  
Staging Environment:  [https://staging.multisig.moonbeam.network](https://staging.multisig.moonbeam.network/)

**Abstract**

This proposal aims to secure funding to continue supporting the Moonbeam Multisig project, which is a fork of Safe that maintains the same UX/UI while incorporating integrations specific to the Moonbeam ecosystem.

Our service support proposal focuses on ensuring continuous operation, addressing any situation requiring personalized attention, such as incidents, bugs, research, dApp support, and community engagement. Additionally, we will continue working on new integrations.

We also commit to being ready for the rollout of new versions of Safe’s Smart Contracts (v1.4.0 and beyond), followed by ongoing support and the integration of new technologies.

All tokens received through this grant will be exclusively dedicated to covering infrastructure costs (Amazon AWS), proportional costs for subscriptions used by the solution (Coingecko, Sentry, and any other necessary services), compensating Protofire, and distributing tokens among developers involved in this support service (base compensation + performance-based bonuses).

**Motivation**

Moonbeam Multisig is a fork of Safe, which is well known as the most trusted platform to store digital assets on EVM due to its programmability. We consider this project a successful case where community users, DAOs and DeFi projects trust and use it to safely store assets and interact with Smart Contracts which directly supports TVL growth and would keep benefiting the Moonbeam community.

**Project Overview and Team Experience**

As the upstream Safe codebase is being constantly updated and changed by the Safe team, new releases need to be merged making sure it is updated and compatible with the Moonbeam Multisig instance.

Regular Safe updates will be performed and released on Moonbeam networks (Moonbeam, Moonriver and Moonbase). Updates consider Frontend (mainly user experience improvements), Backend services and Smart Contract.

Optimization also includes research and implementation of such features as Safe dApps, Modules, Guards, External Wallets Connectors, and customizations according to community needs.

Our team is a combination of management and development skills:

-   Strategic Leader: Ivan.
    
-   Project Manager: Eduardo.
    
-   Software Architect: Nick.
    
-   Blockchain Engineers: Marta, Nikita, Den, Leoni, and Ana.
    
-   DevOps Engineers: Leonid, and Ilya.
    
-   QA Engineer: Anton, and Ulada.
    

Protofire DAO team:

-   Is a formal partner (formal agreement) with the Safe team, being recognized as an official deployer.
    
-   Worked as part of the Gnosis team on delivery of web and desktop versions of Gnosis Safe.
    
-   Delivered Gnosis Safe Apps (such as Compound, Synthetix Mintr Safe App, designed ENS Manager).
    
-   Created a devkit to improve the synchronization of the code in the Gnosis DApps.
    
-   Is a Gnosis Chain and Gnosis Beacon Chain validator.
    
-   Have been deploying and maintaining Safe instances over 40 chains such as: Evmos, Astar, Scroll, Mantle, Linea, Cronos, Holesky, Neon EVM, Rootstock to name a few.
    
-   Is an active member of the Safe community ([Safe Guardians](https://forum.safe.global/t/guardians-gather/265)); we use our power to contribute positively to the ecosystem, aligning with Safe vision to drive the adoption of smart contract wallets.
    

**Rationale**

Moonbeam Multisig adds value to the ecosystem in the following ways:

-   Gives the community a trusted custody option for asset management. Safe smart contracts have passed the highest possible security standards in the industry including Formal Verification.  [Check it out](https://github.com/safe-global/safe-contracts/tree/78494bcdbc61b3db52308a25f0556c42cf656ab1/docs).
    
-   Allows Protocols to deploy and interact with smart contracts in a secure manner which attracts top protocols, increases adoption and TVL.
    
-   Moonbeam Multisig attracts high-net-worth individuals, companies, holders, funds, developers, DAOs, and investors due to its reputation and programmability.
    
-   By allowing multiple signers to approve transactions, Moonbeam Multisig fosters decentralized decision-making, which aligns with the core principles of blockchain technology. This enables organizations and DAOs to manage funds and execute decisions in a more democratic and transparent manner.
    
-   Moonbeam Multisig is highly customizable, allowing users to set different rules and thresholds for transactions. This flexibility supports a wide range of use cases, from personal wallets to complex organizational structures, thereby adding versatility to blockchain operations.
    

**Key Terms**

1.  Multisig (Multisignature): A key feature of the Safe Wallet, requiring multiple private keys (signers) to authorize a transaction, enhancing security and reducing the risk of unauthorized access.
2.  Safe Modules/Guards: Extensions that add custom functionalities to the Safe Wallet or restrict its basic functionality, allowing users to tailor the wallet to their specific needs, such as adding new approval mechanisms or integrating with other services.
3.  Threshold: The minimum number of approvals required to execute a transaction from the Safe Wallet. This threshold can be adjusted based on the security needs of the users.

**Overall Cost**

We are transitioning our support model from a Time & Materials (T&M) approach to a more flexible support-as-a-service model. With the team expansion and our new service model, which allows us to operate based on priorities regardless of approved budget, we have managed to reduce monthly costs by approximately 40% compared to the previous grant (1st semester 2024).

We are requesting funds to cover the current semester, the second half of 2024, from July (last month; we have temporarily assigned the balance as an expense) through December.

Requested Funds: $27,000 (equivalent in GLMR and MOVR tokens considering conversion rate*).

-   The conversion rate will be set as the 30-day twap (time-weighted average price).

**Use of Treasury Funds**

Treasury Funds with potentially 25% allocated exclusively to infrastructure costs, and 75% covering the team, support areas (legal, finance, HR), and bonuses for members who achieve outstanding performance/feedback in the Moonbeam Multisig context.

Title

Costs

Infra Costs

$1000.00

Safe Support as a Service

$3,500.00

**Total**

**$4,500.00**

Expected Infra Costs Distribution:

AWS Service

Purpose

Infra Costs, %

ECS

Safe microservices

63%

CloudWatch

Logs, metrics and alarms

12%

RDS

Safe database

10%

|Other (ELB, WAF, ElastiCache, Route53, S3, CodePipeline, ECR, Lambda)|Load balancing, security, cache, dns, static files, deployment pipelines, docker images repository, monitoring functions)|15%|

![infra-costs-1](https://forum.moonbeam.network/uploads/db2361/original/1X/a8734d3d45ebc6d379ed879a9b14b692f581072c.jpeg)

Safe as a Service includes:

-   Safe Updates: Regular Safe updates will be performed and released on the supported networks (Moonbeam, Moonriver, and Moonbase). Updates consider Frontend (mainly user experience improvements), Backend services and Smart Contract.
    
-   Safe Features: Research and implementation of features like Safe dApps, Safe Modules, Safe Guards, External Wallets Connectors, client customization, etc.
    
-   Infrastructure Support & Monitoring: DevOps support and monitoring, covering all aspects of infrastructure security, architecture optimization, monitoring and CI/CD pipeline enhancement in order to improve cost-effectiveness and scalability.
    
-   General Support: General support is provided to Moonbeam community, business, and technical teams considering incidents analysis and troubleshooting, research, and general inquiries.
    

**Specifications**

Safe Global Licenses describe all the third-party software that may compose (in small portions) our Moonbeam Multisig solution:

[Safe{Wallet} – Licenses](https://app.safe.global/licenses)  (only Web section is applicable).

**Steps to Implement**

Moonbeam Multisig is currently in the support phase; funds will be allocated to cover it

**On-chain Application Details**

Total cost: 27,000 USD (equals a monthly cost of $4,500) equivalent to 60/40 respectively in GLMR and MOVR.

Token

Amount

call hash

GLMR

72222

TO BE DONE

MOVR

918

TO BE DONE

Token

Proposal ID

Link

GLMR

#

TO BE DONE

MOVR

#

TO BE DONE

Base spreadsheet for calculating 30-day TWAP and respective proposal values:

[2025-Semester-1 Moonbeam Multisig Support Treasury Proposal](https://docs.google.com/spreadsheets/d/11LyiCr0-ZRi6OFHz3_8K4t-O71Jisqz5un6Z1rwcjcI/edit?usp=sharing)

----------

Comment with extra data:

  

​

​​Reply

64views10likes3links

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/esantos089/96/566_2.png "Eduardo")](https://forum.moonbeam.network/u/esantos089 "esantos089")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png "_yrn_")](https://forum.moonbeam.network/u/_yrn "_yrn")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png "micheleicebergnodes")](https://forum.moonbeam.network/u/micheleicebergnodes "micheleicebergnodes")

read4  min

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/esantos089/96/566_2.png)](https://forum.moonbeam.network/u/esantos089)

[esantos089](https://forum.moonbeam.network/u/esantos089)

[29d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998/2?u=_yrn "Post date")

Just to add more information here:

**Safe{Wallet} Partner Label:**

We will add a Safe{Wallet} Partner label to the Moonbeam Multisig UI, which represents the partnership with Safe that only a few instances possess. Additionally, we have access to premium support from Safe team for tickets when needed.

[![Safe{Wallet} Partner](https://forum.moonbeam.network/uploads/db2361/optimized/2X/9/97b3a40f7d7ab2a7ad7ee21cc1f33c9427b1f897_2_516x499.png)](https://forum.moonbeam.network/uploads/db2361/original/2X/9/97b3a40f7d7ab2a7ad7ee21cc1f33c9427b1f897.png "Safe{Wallet} Partner")

Safe{Wallet} Partner738×714 26.7 KB

**Previous Activities:**

Attached is the activity spreadsheet detailing what we have carried out over the past 6 months.

[docs.google.com](https://docs.google.com/spreadsheets/d/1GsswmYIPa42mSg6M8jokadBQvexlTgGv1sM2V_i6xQo/edit?usp=sharing)

[](https://docs.google.com/spreadsheets/d/1GsswmYIPa42mSg6M8jokadBQvexlTgGv1sM2V_i6xQo/edit?usp=sharing)

### [2025-Semester-1 Moonbeam - Performed Tasks](https://docs.google.com/spreadsheets/d/1GsswmYIPa42mSg6M8jokadBQvexlTgGv1sM2V_i6xQo/edit?usp=sharing)

This Sheet is private

There are also more generic activities that are not listed here, as we provide Safe as a service. This includes routine actions such as tuning, monitoring, and incident resolution that may go untracked.

**Native Swap / Bridge:**

An important point to highlight is that we recently introduced native Swap functionality (using LIFI ([https://li.fi](https://li.fi/)) as the base).

[![Native Swap](https://forum.moonbeam.network/uploads/db2361/optimized/2X/b/b0e43442eb9d8ff1135a3721d8a1cb33bee93479_2_690x430.jpeg)](https://forum.moonbeam.network/uploads/db2361/original/2X/b/b0e43442eb9d8ff1135a3721d8a1cb33bee93479.jpeg "Native Swap")

Native Swap1850×1154 141 KB

We also plan to enable native bridge options (R&D in progress).

  

​

3​

​​Reply

19 days later

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/micheleicebergnodes/96/1267_2.png)](https://forum.moonbeam.network/u/micheleicebergnodes)

[micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)Treasury Council Member

[10d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998/3?u=_yrn "Post date")

Dear  [@esantos089](https://forum.moonbeam.network/u/esantos089)  Eduardo,  
first of all thank you for this detailed post and moreover for the optimizations applied from your side (Safe team), much appreciated indeed!

Hereby we confirm to have reviewed subject proposal and treasury council members agreed to proceed, that is, we will fund the Multisig project as per your proposal.

From an operative viewpoint, New Spending Flow will be active after the related Hotfix implementation, that is, 18-02-2025.  
Soon after this date we will start our internal procedures to put in place all the pending payments, so we can expect to complete subject process within February 2025 (if any variations, we will keep you updated).  
30d ema prices info will be shared once we will be fully operative on-chain.

Thanks again for your pro-activeness in the optimization activities you put in place!

We will keep you posted!

Michele

  

​

2​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/esantos089/96/566_2.png)](https://forum.moonbeam.network/u/esantos089)

[esantos089](https://forum.moonbeam.network/u/esantos089)

[9d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998/4?u=_yrn "Post date")

Hi  [@micheleicebergnodes](https://forum.moonbeam.network/u/micheleicebergnodes)  , thanks for the heads up!

  

​

1​

​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[3d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998/5?u=_yrn "Post date")

Hey  [@esantos089](https://forum.moonbeam.network/u/esantos089)

RT3401 is now enacted on both Moonbeam and Moonriver and the Treasury Council is ready to conduct your awaited payouts via the new  [Treasury Proposal flow](https://forum.moonbeam.network/t/runtime-rt3400-schedule/1954/6).

For that matter, please provide us with a beneficiary address of your choice and the Treasury Council will process your proposal asap.

We’ve captured the EMA30 price for MOVR at $ 8.483093 at block  [10380992](https://moonriver.subscan.io/tools/price_converter?value=1&type=block&from=MOVR&to=USD&time=10380992)  and at $ 0.150840 at  [9673865](https://moonbeam.subscan.io/tools/price_converter?value=1&type=block&from=GLMR&to=USD&time=9673865)  for GLMR.

This will result in a total payout of 107,398.57 GLMR and 1,273.12 MOVR to settle your request of $ 27,000.

Again, thanks you for your patience!  
yaron

  

​

1

​​​Reply

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/esantos089/96/566_2.png)](https://forum.moonbeam.network/u/esantos089)

[esantos089](https://forum.moonbeam.network/u/esantos089)

[2d](https://forum.moonbeam.network/t/proposal-mbxx-mrxx-moonbeam-multisig-support-and-optimization-services-for-moonbeam-moonriver-and-moonbase-for-1st-semester-2025/1998/6?u=_yrn "Post date")

Hey  [@_yrn](https://forum.moonbeam.network/u/_yrn)  ,  
Thanks for getting back to me and for recalculating based on the EMA30; I really appreciate it.

Below is our Beneficiary Wallet:  
0x4DA9a7f9e2381C0D663116Ed8dE297BAd1DB951c
