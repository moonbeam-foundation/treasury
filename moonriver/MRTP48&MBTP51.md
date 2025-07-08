# [[Proposal: MB11 & 30 / MR8 & 26] StakeGlmr.com and StakeMovr.com V2 - Treasury Proposal](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801)[](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801 "edit the title and category of this topic")

[Governance](https://forum.moonbeam.network/c/governance/2)[Treasury Proposals](https://forum.moonbeam.network/c/governance/treasury-proposals/8)

[moonbeam](https://forum.moonbeam.network/tag/moonbeam)[moonriver](https://forum.moonbeam.network/tag/moonriver)[submitted](https://forum.moonbeam.network/tag/submitted)

4.6kviews228likes21links13users

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/96/147_2.png "stakebaby")](https://forum.moonbeam.network/u/stakebaby "stakebaby")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/jose.crypto/96/20_2.png "jose.crypto")](https://forum.moonbeam.network/u/jose.crypto "jose.crypto")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/blackk_magiik/96/1067_2.png "blackk_magiik")](https://forum.moonbeam.network/u/blackk_magiik "blackk_magiik")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/michele_amurri/96/1267_2.png "Michele Amurri")](https://forum.moonbeam.network/u/Michele_Amurri "Michele_Amurri")

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/aleksandr/96/17_2.png "Aleksandr")](https://forum.moonbeam.network/u/Aleksandr "Aleksandr")

read28  min

Top replies

[Apr 2023](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801/1 "Jump to the first post")

[7h](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801/125)

​

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/96/147_2.png)](https://forum.moonbeam.network/u/stakebaby)

[stakebaby](https://forum.moonbeam.network/u/stakebaby)

10

[Apr 2023](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801?u=_yrn "Post date")

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#abstract-1)Abstract

StakeBaby (Skinny Bottle Ltd.) proposes a complete revamp of  [stakeglmr.com](http://stakeglmr.com/)  and  [stakemovr.com](http://stakemovr.com/), to address limitations in the current code base. The new architecture will improve flexibility, expandability, and future-proof the design. The new platform will have faster load times, improved user experience, and an advanced staking interface that promotes diversification across multiple collators. The proposed setup will be cost-efficient, durable, and fast, using a two-layer approach for API durability and near-real-time performance at a lower operational cost.  

[![](https://forum.moonbeam.network/uploads/db2361/optimized/1X/8bb7652f4e1cf431c47b38773b572fdb826d2785_2_624x305.jpeg)](https://forum.moonbeam.network/uploads/db2361/original/1X/8bb7652f4e1cf431c47b38773b572fdb826d2785.jpeg)

1600×784 224 KB

  
_Screenshot of custom UI components we have made for the new dashboard. This is just a template - not related to staking_

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#motivation-2)Motivation

StakeBaby has supported over 100,000 unique Moonbeam and Moonriver users in making well-informed staking decisions by offering dependable and relevant data. This was achieved through self-funding and collation income. While this approach allowed us to serve the community, it led to a code base that is difficult to maintain and expand. As a result, we plan to replace the old code and develop a new system designed to 1) facilitate the addition of new features, and 2) enhance the overall staking experience.

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#project-overview-3)Project Overview

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#legacy-project-4)Legacy project

[Stakeglmr.com](http://stakeglmr.com/)  and  [stakemovr.com](http://stakemovr.com/)  are currently Svelte SPAs with AWS Lambdas + DynamoDB on the backend. Chain data is currently indexed to a master DynamoDB table. The event stream of all INSERT operations is processed and triggers several Lambda microservices that update other tables in an idempotent manner. Although this setup is durable and has served us well, it poses limitations in upgradeability and expandability. Moreover, the code base has exploded with over 50 microservices and a largely patched frontend.

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#the-new-dashboard-5)The new dashboard

StakeBaby plans to fully revamp the backend and frontend code for  [stakeglmr.com](http://stakeglmr.com/)  and  [stakemovr.com](http://stakemovr.com/), upgrading both platforms to V2. The new architecture aims to be scalable, durable, leaner, and more flexible, enabling new features and an improved interface.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#faster-load-times-enhanced-speed-6)Faster load times - enhanced speed

The updated StakeGlmr and StakeMovr will load as quickly as standard apps, compared to the current 10-second load time. To achieve this, data will initially come from our API, with chain calls updating stale data as needed.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#expandable-and-flexible-improved-design-7)Expandable and flexible - improved design

The new architecture will use Subsquid to index the chain to a Postgres database, allowing for efficient creation and execution of various ETLs. This approach will enable quick re-implementation of existing features, easy extraction of more useful information, and a future-proof design.

[Temporal.io](http://temporal.io/)  will be used to manage ETL workflows, replacing the previous complex choreography and making it easier to adapt and expand. This design will ensure durability while allowing us to focus on business logic and value.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#less-data-more-information-streamlined-interface-8)Less data, more information - streamlined interface

The collator dashboard will be simplified, offering users the option to access more details if desired. New features will include collator age, previous identities, and editable post-mortem reports for missed rounds.

Personal dashboards will be completely redesigned for a more streamlined and user-friendly experience. Improvements will address current issues like long waiting times, lack of event navigation, fixed chart periods, no date filtering, and no real-time updates.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#advanced-staking-interface-enhanced-functionality-9)Advanced staking interface - enhanced functionality

While the current StakeGlmr does not offer staking extrinsics due to Moonbeam’s existing solution, the new version will promote diversification across multiple collators. Users will be able to choose their staking amount, allocation strategy, and collators to stake with in a single transaction. This will increase the stability of the active set and improve delegators’ undelegation flexibility.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#multiple-wallet-integration-10)Multiple wallet integration

The new platform will seamlessly support multiple wallets for both stakemovr and stakeglmr from the outset.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#cost-effective-robust-and-speedy-11)Cost-effective, robust, and speedy

While our current setup is durable, it’s expensive, costing $1,000 per month in cloud provisions. Additionally, due to DynamoDB stream limitations, errors must be resolved within 24 hours, or events are lost. The new configuration will be just as robust but more cost-effective, allowing indefinite retention of ETL errors.

To guarantee a durable and near-real-time API, we’ll deploy our services in two layers. The first, faster but less reliable layer, will have a dedicated server hosting all services (node, indexer, and ETL services) in a single unit. This server will mostly update DynamoDB tables and be responsible for catching up with the chain from its genesis.

The second layer will be cloud-based, utilizing microservices, cloud instances, cloud-based Postgres, and multiple RPC node providers. This layer will be activated daily for a short period (to catch up with the chain) or when layer 1 fails. By running this stack for only a fraction of the time, we’ll achieve durability and reliability at a much lower cost.

Both layers will utilize  [temporal.io](http://temporal.io/)  to coordinate and ensure processes are completed and errors are addressed. Table updates will be detected by microservices and sent to connected clients via Lambdas and websockets, maintaining an auto-scalable push infrastructure.

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#team-experience-12)Team Experience

Our team has a deep understanding of parachain staking pallet mechanics, which we’ve leveraged to consult other networks and create similar dashboards for them. We appreciate the needs of both collators and delegators and are committed to providing reliable, trustworthy data—especially important as more resources offer inconsistent information.

The project will involve two senior developers with extensive experience in various programming languages and cloud technology stacks. Ioannis will focus on backend development, while Abdullah will concentrate on frontend tasks and deployment pipelines, both bringing their expertise to all aspects of the project. We chose exclusively senior talent because the required stack is advanced and multidisciplinary, making junior talent more costly in the long run.

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#value-to-the-moonbeam-ecosystem-13)Value to the Moonbeam Ecosystem

Staking efficiency is crucial for network decentralization and security of a PoS network. Our new staking platform aims to simplify the user experience while promoting a healthier network.

The new Moonbeam staking website aims to provide a better user experience for stakers. Many stakers have found the current staking system complicated and have had issues with not receiving rewards. To address this, the new website will use pizza (yes, pizza!) as an example to explain how rewards are calculated, making it easier for users to understand.

In addition, the new website will allow users to stake with multiple collators in one move, reducing their risk of not receiving rewards due to a dropped-out collator. The website will also enable account login from the home page, allowing for custom advice on the minimum stake and currently staked, to avoid going below the minimum bond.

By improving the user experience, the hope is to gradually increase the total percentage staked. By spreading delegations among multiple collators, the stability of the active set will increase, thereby reducing the volatility of funds staked and improving overall security. Finally, decreased use frustration should enhance the perceived value of Moonbeam and promote growth.

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#total-cost-and-deliverables-14)Total Cost and Deliverables

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#milestones-15)Milestones

We anticipate deploying a production ready version to Moonriver and Moonbeam in 4 months. We have divided the project to two, 2-month milestones:

M1, 2 months

-   SvelteKit frontend app, with mock db calls
-   Inegration of app with wallets, chain queries, and extrinsic calls
-   Indexing backend and ETL services

M2, 4 months

-   Additional microservices
-   Full frontend + backend integration
-   Testing
-   Deployment to production

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#team-16)Team

Ioannis T. - Senior backend developer and cloud architect

Abdullah C. - Senior frontend developer and deployment specialist

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#cost-17)Cost

Our two senior developers each working 20 hours per week. At a rate of $70 per hour, the total cost comes to $44,800. Requested amount is going to be divided between Moonbeam and Moonriver treasury in 80-20 ratio (respectfully):

Moonbeam part (total for M1 and M2): $35,840:

100,397.91 GLMR, based on MA(30): GLMR: 0.35697954 (Coinmarketcap)  
This proposal concerns only M1, which is 50% of the total, that is 50,198.95 GLMR

Moonriver part (total for M1 and M2): $8,960:

1,135.65 MOVR, based on MA(30): MOVR: 7.889724578 (Coinmarketcap)  
This proposal concerns only M1, which is 50% of the total, that is 567.82 MOVR

## [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#use-of-treasury-funds-18)Use of Treasury Funds

The treasury funds would be used for paying out to Skinny Bottle Ltd company for development expenses. The proposal execution will be started if the proposal is approved.

This proposal covers both M1 and M2 expenses that are required to deliver a fully functional, production-ready product.

We propose two payments: 50% of the GLMR and MOVR total amounts upfront for M1, and, after the delivery of M1, 50% upfront for M2.

# [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#technical-specifications-19)Technical Specifications

StakeBaby will use the following stack to implement and deploy the projects.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#subsquid-for-indexing-and-processing-etl-jobs-20)SubSquid for indexing and processing ETL jobs

After testing SubSquid, we found it to be a highly reliable and efficient solution for indexing both Substrate and EVM data.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#temporalio-for-orchestrating-indexing-and-etl-jobs-21)[Temporal.io](http://temporal.io/)  for orchestrating indexing and ETL jobs

Our tests with Temporal and SubSquid revealed that they effectively address most challenges associated with orchestrating indexing and ETL workflows, allowing us to concentrate on value-driven logic now and in the future.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#aws-dynamodb-for-user-requested-transformed-data-22)AWS DynamoDB for user-requested transformed data

We currently use DynamoDB, which performs well. The new design will have both Lambdas and SvelteKit directly query DynamoDB, as opposed to just Lambdas.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#postgres-for-storing-raw-indexed-data-23)Postgres for storing raw indexed data

SubSquid’s default choice, Postgres works well for storing raw data that doesn’t require frequent access or concurrent user requests.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#aws-lambda-24)AWS Lambda

AWS Lambda for scalable, independent microservices or those needing to run for longer than 3 seconds.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#sveltekit-frontend-application-framework-vercel-for-deployment-25)SvelteKit frontend application framework + Vercel for deployment

SvelteKit enables server-rendered pages and SPA functionality, reducing the number of managed microservices, simplifying deployment, and enhancing SEO.

### [](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801#nodejs-and-go-for-the-backend-26)NodeJS and Go for the backend

NodeJS will be our default language, with Go used in cases where high concurrency is needed (e.g., pushing to websockets).

Thank you for your attention and please let us know if you have any questsions/suggestions.

---
[...]

---

[  
stakebaby](https://forum.moonbeam.network/u/stakebaby)

[6d](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801/123?u=_yrn "Post date")

Hi team,  [@Michele_Amurri](https://forum.moonbeam.network/u/michele_amurri)

-   Moonriver sync was completed (from block 1M to today). Replaced the previous database (that was from block 9M or so). There is an issue with the Age field - investigating.
-   Activated Moonriver chat page, as there is now enough data to draw from
-   Fyi. I created  [https://chainy.bot](https://chainy.bot/)  as a contribution to the Polkadot DN program. These chatbots have direct access to all chain query methods (metadata updated daily), and Moonbeam and Moonriver are obviously included. Think of it as an assistant that knows how to query the chain, has access to RPC, and learns gradually from user interactions.

And it’s time for the quarterly infra bill…

Months: April, May, June 2025  
at EUR 400 per month, + EUR 50 safety margin  
Total EUR 1,350.00

Same details as before.

thanks!  
Ioannis

  

[![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/_yrn/96/1746_2.png)](https://forum.moonbeam.network/u/_yrn)

[_yrn](https://forum.moonbeam.network/u/_yrn)Treasury Council Member

[23h](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801/124?u=_yrn "Post date")

Hey  [@stakebaby](https://forum.moonbeam.network/u/stakebaby)

Your total of EUR 1,350.00 was converted to USD 1,580.57 at an exchange rate of 1.17079567 EUR/USD as of July 7, 2025 (source: Google Finance).

That USD total was divided between GLMR and MOVR tokens in a 60:40 ratio.  
We’ve captured 30d EMA prices at  [$ 0.069352](https://moonbeam.subscan.io/tools/price_converter?value=1&type=block&from=GLMR&to=USD&time=11629355)  for GLMR at block  [11629355](https://moonbeam.subscan.io/block/11629355)  and  [$ 5.613303](https://moonriver.subscan.io/tools/price_converter?value=1&type=block&from=MOVR&to=USD&time=12275120)  for MOVR at block  [12275120](https://moonriver.subscan.io/block/12275120). This will result in a payout of 13,674.36 GLMR and 112.63 MOVR.

Both proposals were put on-chain moments ago and are currently awaiting additional votes of members of the Treasury Council. Expect their confirmations and payouts to hit your wallets  _very_  soon.

Thank you for your contributions to the MB ecosystem — Much appreciated!  
yaron