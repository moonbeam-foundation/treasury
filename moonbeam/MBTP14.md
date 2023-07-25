# Moonbeam NFT Tracker

## The project

Moonbeam NFT Tracker is a project that aims to provide the Moonbeam NFT community with valuable insights on promising NFT investments. The project is currently in its early stages of development, with the goal of becoming a fully automated system that posts insights on Twitter and Telegram.

### Social

Twitter:  
[@GlmrNftTracker  1](https://twitter.com/GlmrNftTracker)

Telegram:  
[@GlmrNftTracker](https://t.me/glmrnfttracker)

The current activity on Twitter and Telegram is low as I am working on the project

### NFT Projects

The tracker provides updates on the following projects:

-   Cult Bears DAO
-   Damned Pirates Society
-   Exiled Racers Pilot
-   GLMR APES
-   GLMR JUNGLE
-   Gromlins
-   MoonFit Beast and Beauty
-   Moonpets

Owning a NFT project on Moonbeam and want to be added? DM me on Twitter.

### NFT Marketplaces

The tracker fetches data form the following marketplaces:

-   NFTrade
-   ToFuNFT
-   Moonbeans
-   Raresama

Missing a marketplace? DM me on Twitter.

## Abstract

This proposal aims to secure funding for the operational costs of running the Moonbeam NFT Tracker software, subscription fees for ChatGPT Plus and Twitter Blue, enabling greater visibility. The goal is to cover expenses for running fully automated for one year. The project is expected to become self-sustaining in the future.

## Motivation

This proposal aims to enhance the Moonbeam NFT space by offering the community well-informed insights on promising NFT investments and by improving visibility for NFT projects. The primary goal is to promote and facilitate the growth of the Moonbeam NFT ecosystem.

## Project Overview and Team Experience

I am a highly experienced senior full-stack developer from the Netherlands, having obtained my bachelor’s degree nearly a decade ago. Currently, I am employed by an agency specialized in affiliate websites and software development.

In the beginning of this year, my interest in buying NFTs on Moonbeam inspired me to undertake this project. While I was buying, I encountered difficulties in identifying the most affordable and valuable items based on rarity. To overcome this challenge, I developed scrapers for various NFT marketplaces, laying the foundation for the current project. Presently, I am able to fetch prices for NFT projects and effortlessly generate multiple Twitter post images with just a single click.

My goal is to expand this project by automating the process of scraping prices and sharing insights from the cloud. Currently, the project operates on my development machine. However, by transitioning to a fully automated system, I can ensure more consistent posting and effectively identify significant price drops.

The Moonbeam NFT Tracker currently produces three types of visuals:

-   The cheapest NFTs currently available,
-   The best-priced NFTs determined by rarity/price ratio,
-   The largest price drop observed between two price-fetching periods.

Top 3 cheapest

Top 3 best priced

Biggest price drop

[![cheapest](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/optimized/1X/37710b6d63bbd25ab95ddf51995fab5cc287cc10_2_500x500.png)](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/37710b6d63bbd25ab95ddf51995fab5cc287cc10.png)

[![best_priced](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/optimized/1X/2a89d4f11bbeba7c78d0cdd3f7cac9e5b31fe181_2_500x500.png)](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/2a89d4f11bbeba7c78d0cdd3f7cac9e5b31fe181.png)


[![price_drop](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/optimized/1X/7807ee4d0a00e52b6ec68c979bbe0921f36bec0c_2_500x500.png)](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/7807ee4d0a00e52b6ec68c979bbe0921f36bec0c.png)


Although I currently don’t have concrete plans for its immediate creation, I have a long-term vision of developing a user-friendly front-end platform. This platform will offer real-time insights on the NFT projects covered by the tracker.

## Rationale

A successful blockchain ecosystem should encompass several key components, including DeFi and a thriving NFT community. From my perspective, there is a significant potential for growth within the Moonbeam NFT space. By utilizing the Moonbeam NFT Tracker, I hope to catalyze greater interest and engagement within the NFT community. This will be achieved through increased frequency of posts and enhanced visibility via Twitter Blue.

## Overall Cost

This proposal seeks funding to cover operational costs for one year, totaling $2380.

Average 30D price of moonbeam is $0.2616 resulting in 9098 GLMR

## Use of Treasury Funds

The treasury funds will exclusively cover operational costs, which are as follows:

-   **Hosting, including support**: $165 per month, resulting in $1980 per year
-   **ChatGPT Plus**: $24.10 per month, resulting in $289 per year
-   **Twitter Blue subscription**: $111 per year
-   I personally view working on this project as a hobby, so $0 there.

Upon receiving the treasury funds, I will implement the feature allowing for automatic Twitter posts. This enhancement will ensure the project runs continuously, independent of my development machine.

Verified projects on Moonbeam will be continually added to the platform. Verification occurs when a project is validated on ToFuNFT, NFTrade, Moonbeans, or Raresama and has an active community. This is something that I currently moderate myself.

In the event of any changes implemented on these marketplaces, I commit to updating the scrapers within one week. This timely update is essential to justify the operational costs incurred.

## Specifications

The Moonbeam NFT Tracker is built using Laravel 10 using PHP 8.1 and Puppeteer (using Typescript) for scraping the various marketplaces and generating screenshots. I need to utilize scraping as APIs are absent.

Key technologies utilized:

-   **Laravel Filament**: This admin interface facilitates the setup of new NFT projects.
-   **Laravel Horizon**: These technologies handle:
    -   Jobs that fetch NFT metadata and images
    -   Jobs that calculate rarities based on trait occurrence, or a rarity value provided by the metadata
    -   Scraping jobs
    -   Jobs that process and aggregate data from the scrapers
    -   Jobs that create visuals for posts. Visuals will only be generated if the hash of the outcome is not equal to the previous hash of the same post type.
    -   Jobs that post visuals on Telegram
    -   Jobs that post visuals on Twitter  _(under construction)_
-   **MySQL**: This database system stores all project data.

## Steps to Implement

The initial setup of services will be performed on the hosting environment.

Technically, I will create a job that automates the posting of visuals on Twitter. ChatGPT will assist in partially writing the captions for these posts.

Given my active involvement in the Moonbeam community, I am always open to embracing improvements and welcoming new ideas. My passion lies in continuing to build and improve the Moonbeam NFT Tracker. I believe in the potential of this project and its ability to contribute to the growth and success of the Moonbeam NFT ecosystem.

**Updates since opening the proposal:**

-   Every NFT Project has its own thread on the Telegram channel.

    -   This allows for more frequent posting.
    -   This allows users to only put notifications on for the projects they are interested in.

        [![Scherm­afbeelding 2023-07-15 om 15.25.04](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/optimized/1X/8f23377f1e70453726991bdbf0894ace023dca73_2_198x375.jpeg)](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/8f23377f1e70453726991bdbf0894ace023dca73.jpeg)


-   Posts shared on Telegram now have links to the items featured in the graphic

    [![Scherm­afbeelding 2023-07-15 om 15.20.58](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/optimized/1X/750d0a3169ccde37621200a0821c67f92f3fc3f6_2_334x375.jpeg)](https://europe1.discourse-cdn.com/standard21/uploads/moonbeam/original/1X/750d0a3169ccde37621200a0821c67f92f3fc3f6.jpeg)



Much love to the Moonbeam community!  