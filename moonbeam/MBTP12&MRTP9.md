# [Moonbeam Multisig support and optimization for Moonbeam, Moonriver and Moonbase](https://forum.moonbeam.foundation/t/proposal-mb12-mr9-moonbeam-multisig-support-and-optimization-for-moonbeam-moonriver-and-moonbase/714)




Moonbeam Multisig Official Link:  [https://multisig.moonbeam.network  
5](https://multisig.moonbeam.network/)Staging Environment:  [https://staging.multisig.moonbeam.network  3](https://staging.multisig.moonbeam.network/)


**Abstract**

This proposal aims to show our intention to be part of the Moonbeam treasury program for supporting our well-established Moonbeam Multisig (aka Moonbeam Safe); GLMR will be fully converted to productive hours, covering infrastructure costs, and incentivizing team members to be committed in order to proactively improve key component of Moonbeam’s ecosystem.

**Motivation**

Moonbeam Multisig is a fork of Gnosis Safe, which is well known as the most trusted platform to store digital assets on EVM due to its programmability. We consider this project a successful case where community users, DAOs and DeFi projects trust and use it to safely store assets and interact with Smart Contracts which directly supports TVL growth and would keep benefiting the Moonbeam community.

**Project Overview and Team Experience**

As the upstream Safe codebase is being constantly updated and changed by the Safe team, new releases need to be merged making sure it is updated and compatible with the Moonbeam Multisig instance.

Regular Safe updates will be performed and released on Moonbeam networks (Moonbeam, Moonriver and Moonbase). Updates consider Frontend (mainly user experience improvements), Backend services and Smart Contract.

Optimization also includes research and implementation of such features as Safe dApps, Modules, Guards, External Wallets Connectors, and customizations according to community needs.

Our team is a combination of management and development skills:

* Field CTO: Ivan.
* Project Manager: Eduardo.
* Blockchain Engineers: Nick, Marta, and Nikita.
* DevOps Engineers: Leonid, and Ilya.

Protofire DAO team:

* Worked as part of the Gnosis team on delivery of web and desktop versions of Gnosis Safe.

* Delivered Gnosis Safe Apps (such as Compound, Synthetix Mintr Safe App, designed ENS Manager).
* Created a devkit to improve the synchronization of the code in the Gnosis DApps.
* Is a Gnosis Chain and Gnosis Beacon Chain validator.
* Have been deploying and maintaining Gnosis Safe instances on several networks: Evmos, Velas, Astar, Cronos to name a few.
* Is an active member of the Safe community ([Safe Guardians](https://guardians.gnosis-safe.io)); we use our power to contribute positively to the ecosystem, aligning with Safe vision to drive the adoption of smart contract wallets.

**Rationale**

Moonbeam Multisig adds value to the ecosystem in the following ways:

* Gives the community a trusted custody option for asset management. Safe smart contracts have passed the highest possible security standards in the industry including Formal Verification. [Read more](https://github.com/safe-global/safe-contracts/blob/78494bcdbc61b3db52308a25f0556c42cf656ab1/docs/Gnosis_Safe_Formal_Verification_Report_1_0_0.pdf).

* Allows Protocols to deploy and interact with smart contracts in a secure manner which attracts top protocols, increases adoption and TVL.

Moonbeam Multisig attracts high-net-worth individuals, companies, holders, funds, developers, DAOs, and investors due to its reputation and programmability.

**Key Terms *(optional)***

Safe/Gnosis Safe/Multisig Wallet: multi-signature smart contract wallet that allows users to define a list of owner/signer accounts and a threshold number of signers required to confirm a transaction.

**Overall Cost**

Protofire DAO is requesting funding for 6 months of maintenance. Subsequent maintenance funding requests will be initiated one month prior to the expiration of the previous Treasury Grant. 
Funds disbursement: upfront. Funds remaining from the past month will be moved to the following month.

Total cost: 45,600 USD (equals a monthly cost of $7,6k) equivalent to 80/20 respectively in GLMR and MOVR.

The conversion rate will be set as the 30-day twap (time-weighted average price).

**Use of Treasury Funds** 

Treasury Funds will be allocated as follows:

|Title|Costs|
| --- | --- |
|Infra Costs|$1,200.00|
|Support and Optimization|$6,400.00|

Infra Costs include:

|AWS Service|Purpose|Infra Costs, %|
| --- | --- | --- |
|ECS|Safe microservices|63%|
|CloudWatch|Logs, metrics and alarms|12%|
|RDS|Safe database|10%|
|Other (ELB, WAF, ElastiCache, Route53, S3, CodePipeline, ECR, Lambda)|Load balancing, security, cache, dns, static files, deployment pipelines, docker images repository, monitoring functions)|15%|

![infra-costs-1](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/a8734d3d45ebc6d379ed879a9b14b692f581072c.jpeg)
Support and Optimization include:

* Safe Updates: Regular Gnosis Safe updates will be performed and released on the supported networks. Updates consider Frontend (mainly user experience improvements), Backend services and Smart Contract.

* Safe Features: Research and implementation of features like Safe dApps, Modules, Guards, External Wallets Connectors, client customization, etc.

* Infrastructure Support & Monitoring: DevOps support and monitoring, covering all aspects of infrastructure security, architecture optimization, monitoring and CI/CD pipeline enhancement in order to improve cost-effectiveness and scalability.

* General Support: General support is provided to Moonbeam community, business, and technical teams considering incidents analysis and troubleshooting, research, and general inquiries.

We expect distributing hours as:

|Role|% Expected - Productive Hours Distribution|
| --- | --- |
|Management|10%|
|Blockchain Eng.|70%|
|DevOps Eng.|20%|


**Specifications**

Safe Global Licenses describe all the third-party software that may compose (in small portions) our Moonbeam Multisig solution:

https://safe.global/licenses (only Web section is applicable).

**Steps to Implement**

Moonbeam Multisig is currently in the maintenance phase; funds will be allocated to cover only infrastructure resources and team working hours on maintenance, updates and optimizations.

**On-chain Application Details**

Total cost: 45,600 USD (equals a monthly cost of $7,6k) equivalent to 80/20 respectively in GLMR and MOVR.

|Token|Amount|call hash|
| --- | --- | --- |
|GLMR|129883|0x1ed1310ec8bede48a044db247fb0e9266c6d401675cd61db582986551fa45e31|
|MOVR|1431|0xf57f0cbc559bb1cc49dd08073c39abca50a40e6dc0ac0f9440994f20e83e6d94|

|Token|Proposal ID|Link|
| --- | --- | --- |
|GLMR|12|https://moonbeam.polkassembly.io/treasury/12|
|MOVR|09|https://moonriver.polkassembly.network/treasury/9|


Base spreadsheet for calculating 30-day TWAP and respective proposal values:
https://docs.google.com/spreadsheets/d/181fOng3P6Gsqh_yz3gK3QRCsJflgwZn-0ZPMK04eCKw/edit?usp=sharing
