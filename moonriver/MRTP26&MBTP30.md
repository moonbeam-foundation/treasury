# [Proposal: MB11 & 30 / MR8 & 26] StakeGlmr.com and StakeMovr.com V2 - Treasury Proposal

# Abstract

StakeBaby (Skinny Bottle Ltd.) proposes a complete revamp of stakeglmr.com and stakemovr.com, to address limitations in the current code base. The new architecture will improve flexibility, expandability, and future-proof the design. The new platform will have faster load times, improved user experience, and an advanced staking interface that promotes diversification across multiple collators. The proposed setup will be cost-efficient, durable, and fast, using a two-layer approach for API durability and near-real-time performance at a lower operational cost.
![|624x305](upload://jVZi2fZBkJBksnKhmSR1NY0L36Z.jpeg)
*Screenshot of custom UI components we have made for the new dashboard. This is just a template - not related to staking*

# Motivation

StakeBaby has supported over 100,000 unique Moonbeam and Moonriver users in making well-informed staking decisions by offering dependable and relevant data. This was achieved through self-funding and collation income. While this approach allowed us to serve the community, it led to a code base that is difficult to maintain and expand. As a result, we plan to replace the old code and develop a new system designed to 1) facilitate the addition of new features, and 2) enhance the overall staking experience.

# Project Overview

## Legacy project

Stakeglmr.com and stakemovr.com are currently Svelte SPAs with AWS Lambdas + DynamoDB on the backend. Chain data is currently indexed to a master DynamoDB table. The event stream of all INSERT operations is processed and triggers several Lambda microservices that update other tables in an idempotent manner. Although this setup is durable and has served us well, it poses limitations in upgradeability and expandability. Moreover, the code base has exploded with over 50 microservices and a largely patched frontend.

## The new dashboard

StakeBaby plans to fully revamp the backend and frontend code for stakeglmr.com and stakemovr.com, upgrading both platforms to V2. The new architecture aims to be scalable, durable, leaner, and more flexible, enabling new features and an improved interface.

### Faster load times - enhanced speed

The updated StakeGlmr and StakeMovr will load as quickly as standard apps, compared to the current 10-second load time. To achieve this, data will initially come from our API, with chain calls updating stale data as needed.

### Expandable and flexible - improved design

The new architecture will use Subsquid to index the chain to a Postgres database, allowing for efficient creation and execution of various ETLs. This approach will enable quick re-implementation of existing features, easy extraction of more useful information, and a future-proof design.

Temporal.io will be used to manage ETL workflows, replacing the previous complex choreography and making it easier to adapt and expand. This design will ensure durability while allowing us to focus on business logic and value.

### Less data, more information - streamlined interface

The collator dashboard will be simplified, offering users the option to access more details if desired. New features will include collator age, previous identities, and editable post-mortem reports for missed rounds.

Personal dashboards will be completely redesigned for a more streamlined and user-friendly experience. Improvements will address current issues like long waiting times, lack of event navigation, fixed chart periods, no date filtering, and no real-time updates.

### Advanced staking interface - enhanced functionality

While the current StakeGlmr does not offer staking extrinsics due to Moonbeam's existing solution, the new version will promote diversification across multiple collators. Users will be able to choose their staking amount, allocation strategy, and collators to stake with in a single transaction. This will increase the stability of the active set and improve delegators' undelegation flexibility.

### Multiple wallet integration

The new platform will seamlessly support multiple wallets for both stakemovr and stakeglmr from the outset.

### Cost-effective, robust, and speedy

While our current setup is durable, it's expensive, costing $1,000 per month in cloud provisions. Additionally, due to DynamoDB stream limitations, errors must be resolved within 24 hours, or events are lost. The new configuration will be just as robust but more cost-effective, allowing indefinite retention of ETL errors.

To guarantee a durable and near-real-time API, we'll deploy our services in two layers. The first, faster but less reliable layer, will have a dedicated server hosting all services (node, indexer, and ETL services) in a single unit. This server will mostly update DynamoDB tables and be responsible for catching up with the chain from its genesis.

The second layer will be cloud-based, utilizing microservices, cloud instances, cloud-based Postgres, and multiple RPC node providers. This layer will be activated daily for a short period (to catch up with the chain) or when layer 1 fails. By running this stack for only a fraction of the time, we'll achieve durability and reliability at a much lower cost.

Both layers will utilize temporal.io to coordinate and ensure processes are completed and errors are addressed. Table updates will be detected by microservices and sent to connected clients via Lambdas and websockets, maintaining an auto-scalable push infrastructure.

# Team Experience

Our team has a deep understanding of parachain staking pallet mechanics, which we've leveraged to consult other networks and create similar dashboards for them. We appreciate the needs of both collators and delegators and are committed to providing reliable, trustworthy data—especially important as more resources offer inconsistent information.

The project will involve two senior developers with extensive experience in various programming languages and cloud technology stacks. Ioannis will focus on backend development, while Abdullah will concentrate on frontend tasks and deployment pipelines, both bringing their expertise to all aspects of the project. We chose exclusively senior talent because the required stack is advanced and multidisciplinary, making junior talent more costly in the long run.

# Value to the Moonbeam Ecosystem

Staking efficiency is crucial for network decentralization and security of a PoS network. Our new staking platform aims to simplify the user experience while promoting a healthier network.

The new Moonbeam staking website aims to provide a better user experience for stakers. Many stakers have found the current staking system complicated and have had issues with not receiving rewards. To address this, the new website will use pizza (yes, pizza!) as an example to explain how rewards are calculated, making it easier for users to understand.

In addition, the new website will allow users to stake with multiple collators in one move, reducing their risk of not receiving rewards due to a dropped-out collator. The website will also enable account login from the home page, allowing for custom advice on the minimum stake and currently staked, to avoid going below the minimum bond.

By improving the user experience, the hope is to gradually increase the total percentage staked. By spreading delegations among multiple collators, the stability of the active set will increase, thereby reducing the volatility of funds staked and improving overall security. Finally, decreased use frustration should enhance the perceived value of Moonbeam and promote growth.

# Total Cost and Deliverables

## Milestones

We anticipate deploying a production ready version to Moonriver and Moonbeam in 4 months. We have divided the project to two, 2-month milestones:

M1, 2 months

* SvelteKit frontend app, with mock db calls
* Inegration of app with wallets, chain queries, and extrinsic calls
* Indexing backend and ETL services

M2, 4 months

* Additional microservices
* Full frontend + backend integration
* Testing
* Deployment to production

## Team

Ioannis T. - Senior backend developer and cloud architect

Abdullah C. - Senior frontend developer and deployment specialist

## Cost

Our two senior developers each working 20 hours per week. At a rate of $70 per hour, the total cost comes to $44,800. Requested amount is going to be divided between Moonbeam and Moonriver treasury in 80-20 ratio (respectfully):

Moonbeam part (total for M1 and M2): $35,840:

100,397.91 GLMR, based on MA(30): GLMR: 0.35697954 (Coinmarketcap)
This proposal concerns only M1, which is 50% of the total, that is 50,198.95 GLMR

Moonriver part (total for M1 and M2): $8,960:

1,135.65 MOVR, based on MA(30): MOVR: 7.889724578 (Coinmarketcap)
This proposal concerns only M1, which is 50% of the total, that is 567.82 MOVR

## Use of Treasury Funds

The treasury funds would be used for paying out to Skinny Bottle Ltd company for development expenses. The proposal execution will be started if the proposal is approved.

This proposal covers both M1 and M2 expenses that are required to deliver a fully functional, production-ready product.

We propose two payments: 50% of the GLMR and MOVR total amounts upfront for M1, and, after the delivery of M1, 50% upfront for M2.

# Technical Specifications
StakeBaby will use the following stack to implement and deploy the projects.

### SubSquid for indexing and processing ETL jobs
After testing SubSquid, we found it to be a highly reliable and efficient solution for indexing both Substrate and EVM data.

### Temporal.io for orchestrating indexing and ETL jobs
Our tests with Temporal and SubSquid revealed that they effectively address most challenges associated with orchestrating indexing and ETL workflows, allowing us to concentrate on value-driven logic now and in the future.

### AWS DynamoDB for user-requested transformed data
We currently use DynamoDB, which performs well. The new design will have both Lambdas and SvelteKit directly query DynamoDB, as opposed to just Lambdas.

### Postgres for storing raw indexed data
SubSquid's default choice, Postgres works well for storing raw data that doesn't require frequent access or concurrent user requests.

### AWS Lambda
AWS Lambda for scalable, independent microservices or those needing to run for longer than 3 seconds.

### SvelteKit frontend application framework + Vercel for deployment
SvelteKit enables server-rendered pages and SPA functionality, reducing the number of managed microservices, simplifying deployment, and enhancing SEO.

### NodeJS and Go for the backend
NodeJS will be our default language, with Go used in cases where high concurrency is needed (e.g., pushing to websockets).

Thank you for your attention and please let us know if you have any questsions/suggestions.

---


# Project Report - M2 Delivery

## Code Stats Summary

|Component|Language|Lines of Code|
| --- | --- | --- |
|SvelteKit App|Typescript|14,740|
|SvelteKit App|Svelte|9,912|
|Chat Server|Typescript|4,346|
|Staking Indexer|Typescript|11,730|
|Deep State Indexer|Typescript|8,888|

**Total Typescript Lines: 39,704**

Initial Schedule: 2-6 months Actual Time: 1 year and 2 months

## Milestone Status

### Milestone 1

* ✅ SvelteKit frontend app, with mock db calls
* ✅ Integration of app with wallets, chain queries (TODO: extrinsic calls)
* ✅ Indexing backend and ETL services

### Milestone 2

* ✅ Additional microservices (pending only the collator management services)
* ✅ Full frontend + backend integration (pending only the integration of the above)
* ✅ Backend Testing
* TODO: Frontend Testing
* TODO: Deployment to production

## Features planned and delivered

* New dashboards with more staking info for collators
* New personal account dashboards for delegators
* Faster load time - V2 loads all data straight from the database on a single http call. Collator details data load on separate call, when requested.
* We ended up not using Subsquid and built our own custom indexing pipeline using Temporal for cloud-level process durability on our own hardware.
* Wallet Connect was used to support multiple wallets.
* The new setup allows infinite resolution times, should an error occur during the ETL process. Of course, this does cause the indexer to fall behind, but there is no deadline by which data will start getting lost.
* Cost-efficiency: the new setup requires one 48-core Hetzner server to house the database and workflow/activity programs ($200 per month), one vercel app ($30), and one S3-compatible data bucket. It also requires Temporal cloud services (we don't run our own temporal system) which is a flat $50 (pro-rata, as i also run other services on Temporal) + $10 variable.

## Features not planned and delivered

* Deep State Substrate Indexer. We have built an indexing pipeline that goes well beyond indexing what is readily available, i.e. extrinsic, event, and block data, to indexing the values returned by pallet methods, for any valid arguments. The indexer is built around substrate and the Polkadot.js library. In a nutshell, it works by reading the chain metadata, deconstructing every method input and output values to basic types, creating new basic and complicated inputs, and feeding them back into the methods, and repeating the process (outputs create new inputs).
* Chat interface for the staking data and deep state indexer. This is a ChatGPT assistant based interface that uses ~35 methods to query the database. I plan to add more methods in the future that will provide some interesting graph-based abilities to the bot.

## Features planned and not delivered yet

* Multiple collator staking functionality. This includes the backend logic for recommending staking allocations, and the evm calls on the frontend.
* Full integration with insurance contracts. The contract code is there but i have to connect it to the frontend.
* Push updates of dashboard information via websockets. This is supported out of the box by surrealdb but the functionality is still a bit buggy. Waiting for it to mature. Then, it should be as simple as rewriting the current db queries to include a LIVE keyword and opening surrealdb's websocket port.

## Features planned but will not be delivered

* We will not use a two-layer indexing architecture due to the high computing cost required by the deep state indexer. Instead, we will backup the data extracted files (large jsons, initially cached in s3) and take snapshots of rocksdb.

## Next Steps

### Production Indexing

Catching up to the chain from block 0 will be a challenge. Using a single 48-core machine would take around 7 months to get to block 6M, and by that time the chain would be well ahead especially given the 6-second block periods. Fortunately, the process can be parallelized across multiple servers. I would like to wait for surrealdb 2 to hit the production version before starting syncing from block 1. We are currently using surrealdb 1.5

### Finishing Up Pending Functionality

I will finish up all remaining tasks, but I can't work full-time on this anymore. Indexing will take some time anyways, so I can probably finish everything over part-time weekends.

## M2 Payment

We are way past the second milestone so I would like to submit a vote to the committee. If it's ok with you, I would like to add $2K which is the minimum that I will have to pay for deep-state indexing Moonbeam form block 1. This was not part of the original proposal (neither was the deep state indexer) so I am ok with covering the cost if I have to.

## Questions for the committee

* Future running costs I can run the staking indexer and the apps (for both stakeglmr and stakemovr) for less than 100 EUR per month on infra costs. I think the treasury can cover this once every year or two, no problem. However, running the deep state indexer requires renting a powerful machine from Hetzner that is ~220 EUR per month for each chain. What are your thoughts on this? Should we just do one chain and see how it goes? If so, which one?

## Other Questions

### How was the money spent

* Abdullah received approx. $4K for working on SvelteKit code.
* I have spent around $3K in infrastructure for development and testing.
* The other $11K went to coffee and diapers over 15 months.

### Why did it take so long?

I spent 70-80% of the time on getting the deep state indexer to work. As far as i know, no other chain has something similar, so I think it was worth it. Although the approach worked, it turned out to be much more challenging that I originally thought for 4 reasons. 1) The recursive architecture of the chain metadata required complicated recursive functions that took forever to get right, 2) running hundreds of thousands of queries to index each block required a asynchronous architecture at all 3 levels (in each process, across processes, and across machines), 3) i spent a couple months trying to implement the deep state indexer in golang to leverage its speed but ran into other issues, and 4) surrealdb is still not quite production ready so I had to spend a lot of time submitting GitHub issues and finding ways around them. Knowing what I know now, I would have to taken up this challenge, but what's done is done and (luckily) it works :)


----


@TreasuryCouncil 
Alright, here is the M2 quote breakdown.

|Total||M2 Payment|||30D MA|||
|---|---|---|---|---|---|---|---|
|$44,800||$22,400|Moonbeam|17,920|0.1958|91,522|GLMR|
||||Moonriver|4,480|9.3326|480|MOVR|


I did not add the $2K for the deep state indexing process. I'll cover it myself but I can only do deep indexing for Moonbeam and not Moonriver cause it's too expensive. This means that the Moonriver app will be missing the Explorer and Chat sections.

If anyone wants to review the code send me your Github account email so i can invite you to the repositories.

If you have questions, please don't be shy. A meeting would also work and would probably be more efficient.
