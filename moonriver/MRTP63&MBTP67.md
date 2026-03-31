# [[Proposal: MB11 & 30 / MR8 & 26] StakeGlmr.com and StakeMovr.com V2 - Treasury Proposal](https://forum.moonbeam.network/t/proposal-mb11-30-mr8-26-stakeglmr-com-and-stakemovr-com-v2-treasury-proposal/801/128)

# [](#p-2304-abstract-1)Abstract

StakeBaby (Skinny Bottle Ltd.) proposes a complete revamp of [stakeglmr.com](http://stakeglmr.com) and [stakemovr.com](http://stakemovr.com), to address limitations in the current code base. The new architecture will improve flexibility, expandability, and future-proof the design. The new platform will have faster load times, improved user experience, and an advanced staking interface that promotes diversification across multiple collators. The proposed setup will be cost-efficient, durable, and fast, using a two-layer approach for API durability and near-real-time performance at a lower operational cost.

![](https://forum.moonbeam.network/uploads/db2361/optimized/1X/8bb7652f4e1cf431c47b38773b572fdb826d2785_2_624x305.jpeg)
1600×784 224 KB

*Screenshot of custom UI components we have made for the new dashboard. This is just a template - not related to staking*

# [](#p-2304-motivation-2)Motivation

StakeBaby has supported over 100,000 unique Moonbeam and Moonriver users in making well-informed staking decisions by offering dependable and relevant data. This was achieved through self-funding and collation income. While this approach allowed us to serve the community, it led to a code base that is difficult to maintain and expand. As a result, we plan to replace the old code and develop a new system designed to 1) facilitate the addition of new features, and 2) enhance the overall staking experience.

# [](#p-2304-project-overview-3)Project Overview

## [](#p-2304-legacy-project-4)Legacy project

[Stakeglmr.com](http://Stakeglmr.com) and [stakemovr.com](http://stakemovr.com) are currently Svelte SPAs with AWS Lambdas + DynamoDB on the backend. Chain data is currently indexed to a master DynamoDB table. The event stream of all INSERT operations is processed and triggers several Lambda microservices that update other tables in an idempotent manner. Although this setup is durable and has served us well, it poses limitations in upgradeability and expandability. Moreover, the code base has exploded with over 50 microservices and a largely patched frontend.

## [](#p-2304-the-new-dashboard-5)The new dashboard

StakeBaby plans to fully revamp the backend and frontend code for [stakeglmr.com](http://stakeglmr.com) and [stakemovr.com](http://stakemovr.com), upgrading both platforms to V2. The new architecture aims to be scalable, durable, leaner, and more flexible, enabling new features and an improved interface.

### [](#p-2304-faster-load-times-enhanced-speed-6)Faster load times - enhanced speed

The updated StakeGlmr and StakeMovr will load as quickly as standard apps, compared to the current 10-second load time. To achieve this, data will initially come from our API, with chain calls updating stale data as needed.

### [](#p-2304-expandable-and-flexible-improved-design-7)Expandable and flexible - improved design

The new architecture will use Subsquid to index the chain to a Postgres database, allowing for efficient creation and execution of various ETLs. This approach will enable quick re-implementation of existing features, easy extraction of more useful information, and a future-proof design.

[Temporal.io](http://Temporal.io) will be used to manage ETL workflows, replacing the previous complex choreography and making it easier to adapt and expand. This design will ensure durability while allowing us to focus on business logic and value.

### [](#p-2304-less-data-more-information-streamlined-interface-8)Less data, more information - streamlined interface

The collator dashboard will be simplified, offering users the option to access more details if desired. New features will include collator age, previous identities, and editable post-mortem reports for missed rounds.

Personal dashboards will be completely redesigned for a more streamlined and user-friendly experience. Improvements will address current issues like long waiting times, lack of event navigation, fixed chart periods, no date filtering, and no real-time updates.

### [](#p-2304-advanced-staking-interface-enhanced-functionality-9)Advanced staking interface - enhanced functionality

While the current StakeGlmr does not offer staking extrinsics due to Moonbeam’s existing solution, the new version will promote diversification across multiple collators. Users will be able to choose their staking amount, allocation strategy, and collators to stake with in a single transaction. This will increase the stability of the active set and improve delegators’ undelegation flexibility.

### [](#p-2304-multiple-wallet-integration-10)Multiple wallet integration

The new platform will seamlessly support multiple wallets for both stakemovr and stakeglmr from the outset.

### [](#p-2304-cost-effective-robust-and-speedy-11)Cost-effective, robust, and speedy

While our current setup is durable, it’s expensive, costing $1,000 per month in cloud provisions. Additionally, due to DynamoDB stream limitations, errors must be resolved within 24 hours, or events are lost. The new configuration will be just as robust but more cost-effective, allowing indefinite retention of ETL errors.

To guarantee a durable and near-real-time API, we’ll deploy our services in two layers. The first, faster but less reliable layer, will have a dedicated server hosting all services (node, indexer, and ETL services) in a single unit. This server will mostly update DynamoDB tables and be responsible for catching up with the chain from its genesis.

The second layer will be cloud-based, utilizing microservices, cloud instances, cloud-based Postgres, and multiple RPC node providers. This layer will be activated daily for a short period (to catch up with the chain) or when layer 1 fails. By running this stack for only a fraction of the time, we’ll achieve durability and reliability at a much lower cost.

Both layers will utilize [temporal.io](http://temporal.io) to coordinate and ensure processes are completed and errors are addressed. Table updates will be detected by microservices and sent to connected clients via Lambdas and websockets, maintaining an auto-scalable push infrastructure.

# [](#p-2304-team-experience-12)Team Experience

Our team has a deep understanding of parachain staking pallet mechanics, which we’ve leveraged to consult other networks and create similar dashboards for them. We appreciate the needs of both collators and delegators and are committed to providing reliable, trustworthy data—especially important as more resources offer inconsistent information.

The project will involve two senior developers with extensive experience in various programming languages and cloud technology stacks. Ioannis will focus on backend development, while Abdullah will concentrate on frontend tasks and deployment pipelines, both bringing their expertise to all aspects of the project. We chose exclusively senior talent because the required stack is advanced and multidisciplinary, making junior talent more costly in the long run.

# [](#p-2304-value-to-the-moonbeam-ecosystem-13)Value to the Moonbeam Ecosystem

Staking efficiency is crucial for network decentralization and security of a PoS network. Our new staking platform aims to simplify the user experience while promoting a healthier network.

The new Moonbeam staking website aims to provide a better user experience for stakers. Many stakers have found the current staking system complicated and have had issues with not receiving rewards. To address this, the new website will use pizza (yes, pizza!) as an example to explain how rewards are calculated, making it easier for users to understand.

In addition, the new website will allow users to stake with multiple collators in one move, reducing their risk of not receiving rewards due to a dropped-out collator. The website will also enable account login from the home page, allowing for custom advice on the minimum stake and currently staked, to avoid going below the minimum bond.

By improving the user experience, the hope is to gradually increase the total percentage staked. By spreading delegations among multiple collators, the stability of the active set will increase, thereby reducing the volatility of funds staked and improving overall security. Finally, decreased use frustration should enhance the perceived value of Moonbeam and promote growth.

# [](#p-2304-total-cost-and-deliverables-14)Total Cost and Deliverables

## [](#p-2304-milestones-15)Milestones

We anticipate deploying a production ready version to Moonriver and Moonbeam in 4 months. We have divided the project to two, 2-month milestones:

M1, 2 months

- SvelteKit frontend app, with mock db calls

- Inegration of app with wallets, chain queries, and extrinsic calls

- Indexing backend and ETL services

M2, 4 months

- Additional microservices

- Full frontend + backend integration

- Testing

- Deployment to production

## [](#p-2304-team-16)Team

Ioannis T. - Senior backend developer and cloud architect

Abdullah C. - Senior frontend developer and deployment specialist

## [](#p-2304-cost-17)Cost

Our two senior developers each working 20 hours per week. At a rate of $70 per hour, the total cost comes to $44,800. Requested amount is going to be divided between Moonbeam and Moonriver treasury in 80-20 ratio (respectfully):

Moonbeam part (total for M1 and M2): $35,840:

100,397.91 GLMR, based on MA(30): GLMR: 0.35697954 (Coinmarketcap)

This proposal concerns only M1, which is 50% of the total, that is 50,198.95 GLMR

Moonriver part (total for M1 and M2): $8,960:

1,135.65 MOVR, based on MA(30): MOVR: 7.889724578 (Coinmarketcap)

This proposal concerns only M1, which is 50% of the total, that is 567.82 MOVR

## [](#p-2304-use-of-treasury-funds-18)Use of Treasury Funds

The treasury funds would be used for paying out to Skinny Bottle Ltd company for development expenses. The proposal execution will be started if the proposal is approved.

This proposal covers both M1 and M2 expenses that are required to deliver a fully functional, production-ready product.

We propose two payments: 50% of the GLMR and MOVR total amounts upfront for M1, and, after the delivery of M1, 50% upfront for M2.

# [](#p-2304-technical-specifications-19)Technical Specifications

StakeBaby will use the following stack to implement and deploy the projects.

### [](#p-2304-subsquid-for-indexing-and-processing-etl-jobs-20)SubSquid for indexing and processing ETL jobs

After testing SubSquid, we found it to be a highly reliable and efficient solution for indexing both Substrate and EVM data.

### [](#p-2304-temporalio-for-orchestrating-indexing-and-etl-jobs-21)[Temporal.io](http://Temporal.io) for orchestrating indexing and ETL jobs

Our tests with Temporal and SubSquid revealed that they effectively address most challenges associated with orchestrating indexing and ETL workflows, allowing us to concentrate on value-driven logic now and in the future.

### [](#p-2304-aws-dynamodb-for-user-requested-transformed-data-22)AWS DynamoDB for user-requested transformed data

We currently use DynamoDB, which performs well. The new design will have both Lambdas and SvelteKit directly query DynamoDB, as opposed to just Lambdas.

### [](#p-2304-postgres-for-storing-raw-indexed-data-23)Postgres for storing raw indexed data

SubSquid’s default choice, Postgres works well for storing raw data that doesn’t require frequent access or concurrent user requests.

### [](#p-2304-aws-lambda-24)AWS Lambda

AWS Lambda for scalable, independent microservices or those needing to run for longer than 3 seconds.

### [](#p-2304-sveltekit-frontend-application-framework-vercel-for-deployment-25)SvelteKit frontend application framework + Vercel for deployment

SvelteKit enables server-rendered pages and SPA functionality, reducing the number of managed microservices, simplifying deployment, and enhancing SEO.

### [](#p-2304-nodejs-and-go-for-the-backend-26)NodeJS and Go for the backend

NodeJS will be our default language, with Go used in cases where high concurrency is needed (e.g., pushing to websockets).

Thank you for your attention and please let us know if you have any questsions/suggestions.

---

### Reply by Aleksandr

Hey, Ioannis, first of all, Thank you for your hard work and excellent services!

Many community members rely on your platform as a dashboard to monitor collator selection and other data. i believe that updating the design and adding new features is necessary and exciting.

Are there any potential security risks associated with adding these new features? 
![:point_down:](https://forum.moonbeam.network/images/emoji/twitter/point_down.png?v=12)

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/48/147_2.png)
 Ioannis | StakeBaby:

> 
While the current StakeGlmr does not offer staking extrinsics due to Moonbeam’s existing solution, the new version will promote diversification across multiple collators. Users will be able to choose their staking amount, allocation strategy, and collators to stake with in a single transaction. This will increase the stability of the active set and improve delegators’ undelegation flexibility.

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/48/147_2.png)
 Ioannis | StakeBaby:

> 
In addition, the new website will allow users to stake with multiple collators in one move, reducing their risk of not receiving rewards due to a dropped-out collator.

---

### Reply by stakebaby

Short answer - Yes!

Both stakeglmr and stakemovr already allow interaction with the insurance and the pool, so some users are already executing contract txs already. Obviously, the new platform will increase the number of transactions many-fold.

I don’t want to get into too much detail about how we manage security, but deployment basically requires access to a custom IAM role that is password protected, AND subsequent access to the AWS console using a separate account that requires a hardware key.

The new deployment pipeline will require something similar on Vercel. The good thing about Vercel is that it can do an instant switch from one repo to another one, so there is no gradual invalidation of cloudfront files, and we might be able to switch from a two-step approach to a one-step with hardware key.

Having a small, two-person team, makes it much easier to keep things secure so. I will be doing all the chain integration stuff in any case, cause Abdullah does not have any blockchain experience.

---

### Reply by stakebaby

Forgot to mention that I don’t use Google or anything else to store my AWS password… lol, it’s in my head 
![:grin:](https://emoji.discourse-cdn.com/twitter/grin.png?v=12)

---

### Reply by blackk_magiik

Hey @ioannis_DVN

Great proposal, rely on your websites all the time. Curious, how much do you think your current costs will be reduced by?

 ioannis_DVN:

> 
While our current setup is durable, it’s expensive, costing $1,000 per month in cloud provisions. Additionally, due to DynamoDB stream limitations, errors must be resolved within 24 hours, or events are lost. The new configuration will be just as robust but more cost-effective, allowing indefinite retention of ETL errors.

---

### Reply by stakebaby

Off the top of my head, DynamoDB is 75%, and Lambda like 15%. Most of this is just indexing (90% or $800), so, that will be replaced with a dedicated server at $200/month. There will be some extra costs for the cloud sync setup, but this will only run for a few minutes per day, so it will be negligible. At the end of the day, it will be a much more performant and cheaper setup. Easier to manage too, thanks to [temporal.io](http://temporal.io)’s reporting.

[EDIT: There are still indexing ops / writes to DynamoDB ETL tables, but these tables are ~15% of the size of the archive table]

---

### Reply by jose.crypto

Hey [@stakebaby](/u/stakebaby) thanks for the proposal

I have personally confirmed the recurring use by users in order to obtain information about APR and collators

so I think this proposal is worth it, cause

improving the user experience is always good in the long run and will attract new users also facilitating the staking election process , I support it in a general sense

I like that the proposal is divided into 2 payments based on milestones

The only concern would be to add more txs features, this would be through tx batch calls or through smart Contracts that would act en behalf to the user, like the insurance smart Contract, should this be audited?

---

### Reply by stakebaby

Thanks for the support! The proposal does not involve writing any smart contracts, and, as you correctly point out, that’s what there is batching for. If, for some weird reason, we cannot batch staking requests, the user would have to sign separate txs.

---

### Reply by Jim_CertHum

Hey [@stakebaby](/u/stakebaby) , thanks for sharing your plans to update [stakeglmr.com](http://stakeglmr.com) and [stakemovr.com](http://stakemovr.com) with a relevant refresh. Your sites and moonscan are two of my main go-to sites to get a quick snapshot of how our collators are perceived by delegators. Sometimes when not at a desk that’s all that is needed to know things are running smoothly (although we have many other notifications if something breaks). In fact, in times of new entrants to the active set, I refresh so often I might be a main driver of some of your costs.

Your focus on fairness while still helping community collators differentiate themselves is also commendable. Thanks for all you’ve done to strike the right balance.

Lastly, I’ll just relay feedback that I have received many times from delegators (which I am sure you’ve seen or heard yourself) – it’s still too difficult for new delegators to make heads or tails of staking, so anything you can do to improve that experience for noobs I’m sure will be welcomed. Good luck with the grant request.

---

### Reply by stakebaby

If anybody has any feature requests or ideas for the new platform, please share them with me here or over DM.

The new design will increase the upgradeability of the platform in any case, so it will be much much easier to add new features going forward. However, we might as well do a feature request list now, while we are it!

---

### Reply by Aleksandr

hey, ioannis, i was thinking about some features that I would like to be able to use on your platform. one example is the ability to see which collator the reward comes from. this would be especially useful for delegators who choose multiple collators and want to know which collator pays what reward. additionally, it would be helpful to have a list of actions that the delegator has performed, such as increasing or reducing their bond, or revoking it. It would also be great if users could access a full list of the rewards they earned for the entire staking period. lastly, many users would benefit from a simulator that shows them what rewards they could earn with a certain number of tokens – these features are available on web3go and are incredibly convenient

---

### Reply by stakebaby

Thanks for the input!

On the ability of delegators to see which collator a reward comes from, there is already a related chart in the personal staking dashboard. Do you mean the same in table form?

![image](/uploads/db2361/optimized/1X/5c8d4fb6e21468484723906f153a25a9f964edb4_2_690x387.png)

image922×518 48.9 KB

You also currently get APR per collator so you can compare.

On the actions performed - yeap, there will be a list of all actions! I am actually thinking about creating a master activity list, with summarized events (so that the list is not overtaken by reward payouts) and user actions. The user should be able to filter it too.

On the list of rewards, I think you mean something like a table on a weekly/monthly basis. Right?

We can integrate an expected APR on the multi-collator delegation form that will depend on the entered amounts. Some disclaimer would have to go in though… I personally dislike the word “expected” hahaha

PS: The expected reward function in web3go is wrong because 1) it does not take into account requested un-delegations for the current collator APR, and 2) it does not take into account the diluting effect of the amount to be delegated. Not a fan I am afraid 
![:stuck_out_tongue:](https://emoji.discourse-cdn.com/twitter/stuck_out_tongue.png?v=12)

---

### Reply by jose.crypto

if you are going to integrate a list of actions and a table of last rewards, not chart

It would be good if the timeframe is customizable or at least several options

for example, to be able to choose from such a date to such a date,

or give the options of, last 7, 14, 30, days, and  also show the total of that timeframe , idk if i explained myself well jajaj

---

### Reply by Aleksandr

oh, I didn’t know about such a chart, thanks for sharing. I think if it could be additionally seen in the form of a table, it would also be incredibly convenient.

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/48/147_2.png)
 Ioannis | StakeBaby:

> 
On the list of rewards, I think you mean something like a table on a weekly/monthly basis. Right?

yes, that’s right, users sometimes ask about it and want to see it. on web3go, this looks like the total reward for the entire staking period

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/48/147_2.png)
 Ioannis | StakeBaby:

> 
We can integrate an expected APR on the multi-collator delegation form that will depend on the entered amounts. Some disclaimer would have to go in though… I personally dislike the word “expected” hahaha

PS: The expected reward function in web3go is wrong because 1) it does not take into account requested un-delegations for the current collator APR, and 2) it does not take into account the diluting effect of the amount to be delegated. Not a fan I am afraid 
![:stuck_out_tongue:](https://forum.moonbeam.network/images/emoji/twitter/stuck_out_tongue.png?v=12)

haha, this is also a fairly frequent request from users tbh, as many are incredibly happy to play with such a simulator, idk if it can somehow be made more accurate, but it seems that in web3go it shows fairly approximate figures that seem true

btw, what I like about web3go is that I can view all this data for the delegator just by knowing his address, is it possible to make viewing this data available to everyone?

sorry that I often mention web3go here, it’s just that these are pretty cool features that I often have to use as a moderator, and it helps incredibly to sort out various problems and issues

---

### Reply by stakebaby

> 
oh, I didn’t know about such a chart, thanks for sharing. I think if it could be additionally seen in the form of a table, it would also be incredibly convenient.

You can also see personal APR per collator, historically. Will add tables!

> 
btw, what I like about web3go is that I can view all this data for the delegator just by knowing his address, is it possible to make viewing this data available to everyone?

It used to be like that actually! You could copy/paste in any address to

[https://stakeglmr.com/dashboard/dash-staking](https://stakeglmr.com/dashboard/dash-staking)

but then we replaced that with a multi-wallet login. I will bring it back then, it makes sense.

> 
it seems that in web3go it shows fairly approximate figures that seem true

Throw in a million glmr and it will overestimate APR by 25%. Haha. “The more at stake, the bigger the mistake” it even rhymes 
![:stuck_out_tongue:](https://forum.moonbeam.network/images/emoji/twitter/stuck_out_tongue.png?v=12)

> 
It would be good if the timeframe is customizable or at least several options

Introducing time (as in hours and days, not blocks) will be tricky, but I think it’s a must.

---

### Reply by jose.crypto

However, you can do the calculation in blocks with target time, of course, when there is an obvious delay this will have its errors, but you can place a warning

![Screenshot_2023-04-25-10-23-13-944_com.discord](/uploads/db2361/optimized/1X/90912230d747199d6c0dfb401aba557439b9d876_2_225x500.jpeg)

Screenshot_2023-04-25-10-23-13-944_com.discord1080×2400 223 KB

---

### Reply by Daniel_TrueStaking

![](https://forum.moonbeam.network/user_avatar/forum.moonbeam.network/stakebaby/48/147_2.png)
 Ioannis | StakeBaby:

> 
To achieve this, data will initially come from our API, with chain calls updating stale data as needed.

Your sites are very valuable to the community and very much appreciated!

Can you elaborate on how the new design will be lower the overall RPC call rate for users of your sites?

Thanks!

---

### Reply by stakebaby

It’s easy to cut corners like that, and then a user looks up an XCM transaction one year ago where DOT left Polkadot and arrived to xcDOT one hour before it left (because of the different time lag between chains)… oops!

---

### Reply by stakebaby

Thanks for the question Dan.

Both stakemovr and stakeglmr users are served by United Bloc for chain queries and EVM queries. UB has helped a LOT with increasing speed and getting rid of timeouts.

Now, stakeglmr and stakemovr are quite heavy on the requests for 2 reasons: 1) the inherent amount of required data, and 2) duplicated requests on some cases.

For V2, we want to make sure that the user feels like they are using a regular web2 app as far as load times are concerned. Therefore, we plan on caching all the content on the server side (and actually rendering it there on the initial request). The client will then take over and update values on the client side using chain queries. This was not possible on the current design due to the way sorting works and how things are piped together.

This will allow us to improve on two things in regard to rpc calls. First, we can eliminate duplicate queries (currently fired on Svelet’s discretion because that’s just how it works). Second, it will allow us to spread them over a longer time frame cause the user will already be seeing data. Third, it will allow us to query more efficiently in some cases. For example, instead of firing off 72 queries to read the insurance contract balance of all collators, we can just query only cached cover members over a few seconds.

All in all, the new dashboard will be much more polite to the endpoints 
![:slight_smile:](https://emoji.discourse-cdn.com/twitter/slight_smile.png?v=12)

Many thanks to UB for putting up with us until then!

---

### Reply by Daniel_TrueStaking

That sounds like a significant improvement Ioannis and I am pleased to support this proposal.

---
*Generated by Payoutor*
*Moonbeam Proposal ID: 67*
*Moonriver Proposal ID: 63*
*Beneficiary: 0x1980E75f1b1cdAAe3b2f79664C7cb83b86A3D404*
*Reward: 616.1586 MOVR*
*Submitted by: Yaron*
