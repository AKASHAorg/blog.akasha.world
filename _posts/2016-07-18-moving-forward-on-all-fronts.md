---
layout: post
title: "Moving Forward On All Fronts"
timezone: Europe/Zurich
date: 2016-07-18 00:00:01
future: true
image: telescope.jpg
comments: true
tags: AKASHA, Ethereum, IPFS, Alpha, Raiden, Metamask, Light-Client
published: true
---

Hello everyone, it's been a while since the last update!

The Ethereum ecosystem has seen many things since our last post. From the rise and fall of "the" DAO accompanied by a [/r/ethereum](https://www.reddit.com/r/ethereum/){:target="_blank"} "troll invasion" to [abandoned soft forks](https://www.reddit.com/r/ethereum/comments/4q9ewf/ethereums_dao_wars_soft_fork_is_a_potential_dos/){:target="_blank"} and intensely [debated hard forks](http://carbonvote.com/){:target="_blank"}, we've been through a lot as a community during these last few weeks. 

However, even in the midst of all the panic and heated debates, we had quite a few big positive things going on at the same time. In this update I will try to focus on some of the most important news surrounding the Ethereum and IPFS ecosystems and what that news means to us.

Here at AKASHA we’ve focused our efforts lately on revamping the smart contracts architecture in preparation for the alpha release while actively participating in historic discussions surrounding the Swiss regulatory environment for blockchain companies.

We are very happy with the results and we want to share them with you as well :)

### Alpha Release Progress Overview

![ogogog]({{ site.baseurl }}/content/images/keyboard.jpg)

In the light of the recent events we revamped our smart contract architecture, and by applying the lessons learned from "the" DAO attack we’ve ensured AKASHA is now more secure, modular and extensible. The new smart contracts have been deployed on the testnet and we are now in the process of testing the various flows found inside the application.

For identity management we chose to experiment in the first release with "one profile, one (simple) smart contract" as this approach enables us to explore interesting scenarios and most likely will serve as a stepping stone for a future AKASHA identity and reputation system. 

We are well aware that identity and reputation are really hard problems to solve in one go, so we chose to build something simple and usable for the MVP, and will be continuing to experiment with this area in incremental steps. 

Another interesting test will come in the form of entries that will have their own smart contract. After the voting period ends, the entry contract will self-destroy, distributing to the author all the ETH gathered from votes in the process. 

We're excited to test and better understand how well this approach scales; we're looking towards future experiments with things such as smart content licensing, syndication, translations and more.

The Ethereum address/key pair generated while creating your profile will be used as the signing key with the added "collector" or "wallet" functionality for receiving the ETH from your entries. If we're using the voting example, in case you haven't changed the defaults, at the end of the voting period you will receive your ETH at the key associated with the profile's smart contract. 

This being said, if you want your ETH to go somewhere else, the default "collector" address can easily be changed to one from your favorite Ethereum wallet. 

The search and discovery of content in a decentralized context turned out to be a fascinating challenge to solve. The pursuit for solutions to this challenge led to a number of (potentially) great ideas and we are looking forward to testing them. 

Just as in the case of identity and reputation, we accept that this is a very, very hard thing to get "perfect" from the start, especially in a decentralized setup, and we plan to improve it as we go since we want to incorporate the community feedback along the way.

Solid progress is also being made on fusing the Ethereum and IPFS technologies inside our dapp. **We have open sourced our work**; those interested can find our Ethereum and IPFS connectors below:

**Ethereum Go connector**

- [GitHub repository](https://github.com/AkashaProject/geth-connector){:target="_blank"}
- [npm package](https://www.npmjs.com/package/@akashaproject/geth-connector){:target="_blank"}
- [Documentation](http://docs.akasha.world/geth-connector/globals.html){:target="_blank"}

**IPFS Go connector**

- [GitHub repository](https://github.com/AkashaProject/ipfs-connector){:target="_blank"}
- [npm package](https://www.npmjs.com/package/@akashaproject/ipfs-connector){:target="_blank"}
- [Documentation](http://docs.akasha.world/ipfs-connector/globals.html){:target="_blank"}

We’ve also started to experiment with a custom [IPLD](https://github.com/ipfs/specs/tree/master/ipld){:target="_blank"}-like pathing scheme using [JS IPFS API](https://github.com/ipfs/js-ipfs-api){:target="_blank"} with the more stable [Go IPFS implementation](https://github.com/ipfs/go-ipfs){:target="_blank"} running in the background. Those who are curious and interested in playing with our home-baked IPLD experiment can find the code powering it in our [IPFS connector repository](https://github.com/AkashaProject/ipfs-connector){:target="_blank"}. 

As always, feedback and contributions are more than welcome!

### Noteworthy Ethereum & IPFS Ecosystems Progress

**[IPFS](https://ipfs.io/){:target="_blank"}**, or the Inter-Planetary File System, is a new hypermedia distribution protocol, addressed by content and identities. We are using it to store and distribute the content published on AKASHA in a decentralized fashion. 

![IPFS JS]({{ site.baseurl }}/content/images/ipfs-js.jpg)

The IPFS team made notable progress lately on their [JavaScript Implementation](https://github.com/ipfs/js-ipfs){:target="_blank"} and we played with it in order to better understand how we can use it when we’re ready for prime time. I'd like to thank everyone, again, for taking the time to help and answer our questions.

[IPFS JS](https://github.com/ipfs/js-ipfs){:target="_blank"} is very interesting for us since it can exponentially increase the access to information posted on AKASHA by making it accessible also from classic Web 2.0 browsers such as Chrome and Firefox. 

However, currently IPFS JS is in the (very) [early stages of development](https://github.com/ipfs/js-ipfs/blob/master/ROADMAP.md){:target="_blank"} and that comes, as expected, with big changes from one version to another and stability challenges.

At this point in time, the [IPFS Go](https://github.com/ipfs/go-ipfs){:target="_blank"} implementation is considerably more stable and mature compared to the JavaScript implementation and we will probably end up using it for the alpha release. 

**[Ethereum](https://ethereum.org/){:target="_blank"}** is a decentralized applications platform with a consensus engine in the form of a turing-complete blockchain. We are using it for verifiability, pub/sub relationships, identity/profile management, voting and micropayments. 

![Ethereum light client tests]({{ site.baseurl }}/content/images/vitalik-light-client.jpg)

At the end of June, the [Ethereum light client](https://github.com/zsfelfoldi/go-ethereum/wiki/Light-Ethereum-Subprotocol-(LES)){:target="_blank"} entered in public tests. We are particularly excited about this, as one of the biggest adoption issues we anticipate when it comes to mainstream adoption is the Ethereum blockchain size and synchronization time. On this note, **instant sync from a trusted checkpoint was introduced** a few days after the initial public test release (awesome!!!).

We are keeping a close eye on the progress in this area as we hope to have something to work with for the beta release. For those eager to learn more, you can find more information on the light client public test in [this document](https://github.com/zsfelfoldi/go-ethereum/wiki/Light-Client-Public-Test){:target="_blank"}.

Moving on, in early July, the [Ethereum Mist browser](https://github.com/ethereum/mist){:target="_blank"} reached a historic milestone with the 0.8.0 version as it marks the first public release of the browser. The browser is still in the early stages of development and we expect to see major improvements and new applications populating it in the following months. 

![Ethereum Mist Wallet]({{ site.baseurl }}/content/images/mist-wallet.jpg)

This release comes by default with a proof-of-concept dapp called Stake Voice, which allows ETH holders to submit statements and/or vote on existing ones via the Ethereum blockchain. 

![Ethereum Mist Stake Voice]({{ site.baseurl }}/content/images/mist-stake.jpg)

We are considering implementing AKASHA as a Mist application in the near future; however, this decision heavily depends on the progress made by the [fantastic Mist dev team](https://github.com/ethereum/mist/graphs/contributors){:target="_blank"} in the meantime. 

Another **very** interesting development comes from the [Raiden Network](http://raiden.network/){:target="_blank"} team. Similar to the Bitcoin [lightning network](https://lightning.network/){:target="_blank"}, the basic idea behind Raiden is to implement a model that allows users to privately exchange messages which sign the transfer of value instead of having all transactions recorded on the public blockchain.

![Raiden Network]({{ site.baseurl }}/content/images/raiden.jpg)

In other words, Raiden is a technology that can leverage off-chain state networks to extend Ethereum with some very interesting properties for asset transfers:

- **Scalable**: It scales linearly with the number of participants (1,000,000+ transfers per second possible)
- **Fast**: Transfers are confirmed and final within a fraction of a second
- **Confidential**: Single transfers don’t show up in the global shared ledger
- **Interoperable**: Works with any token that follows Ethereum’s standardized token API
- **Low Fees**: Transaction fees can be seven orders of magnitude lower than on the blockchain
- **Micro-payments**: Low transaction fees allow the efficient transfer of tiny values

For us, something like this would be a match made in heaven as it would drastically lower micro-transaction fees while enabling at the same time a frictionless token economy inside the Ethereum and AKASHA ecosystems thanks to its interoperability properties. Raiden is a very promising project for Ethereum and AKASHA, and we will surely follow its development closely.

At the other end of the Ethereum ecosystem, just before publishing this update, the awesome [Metamask](https://metamask.io/){:target="_blank"} team released the public beta version of a [Chrome plugin](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn){:target="_blank"} that transforms normal Chrome browsers into Ethereum browsers. 

![Metamask]({{ site.baseurl }}/content/images/metamask.jpg)

Metamask is extremely interesting for us as it can lower the entry barriers significantly for new users that do not necessarily want to install a new application on their machines. 

**Combined with IPFS JS, Metamask could potentially make AKASHA fully functional from normal Web 2.0 browsers**. During the next few weeks we will investigate and experiment with this plugin, exploring in the process how it fits with the rest of our puzzle.

In conclusion, the Ethereum light client, the Mist browser, the Raiden network, the Metamask plugin and IPFS JS are all wildcards in our development roadmap. For now we will continue building the AKASHA MVP as a standalone dapp with Go-Ethereum and Go-IPFS until we have something more stable to experiment with and/or build upon. 

But in any case, if anything, all the recent developments across both the IPFS and Ethereum ecosystems are very encouraging with regards to the future of AKASHA and they serve as an example of the **synergy** that comes with building an application on top of these technologies.

### The Swiss Cherry On Top

![Beautiful Zug]({{ site.baseurl }}/content/images/zug-cover.jpg)

On July 1 a historic event took place in Switzerland: the first official Bitcoin transaction with a local Canton administration. [Zug](https://en.wikipedia.org/wiki/Zug){:target="_blank"}, the home of Ethereum and AKASHA, has taken a first big step forward.

![Zug Tweet]({{ site.baseurl }}/content/images/zug-tweet2.jpg)

[Presented as a pilot program](http://www.dw.com/en/alpine-crypto-valley-pays-with-bitcoins/a-19371082?){:target="_blank"}, Zug looks towards a future in which blockchain technologies will increasingly become part of our society and, in my opinion, this first Bitcoin experiment is just the tip of the iceberg.

It's also worth mentioning that besides this pilot program, there are many other exciting things happening in the background such as the drafting of a new hybrid organizational structure that could fill the current gap between fully decentralized and fully centralized companies. 

This in itself could become a major breakthrough for Ethereum projects as the relationships between companies and smart contracts could be mapped clearly for everyone, avoiding situations such as Slock's DAO, DAO.link, Slock.it and Slock UG, where many people still don't quite understand who's who and what's what. 

Moreover, there is also a big chance of seeing a Swiss "regulatory sandbox" initiative soon for FinTech companies operating in the blockchain industry space. The specifics are not yet set in stone but this could become very important both for the already established Swiss blockchain companies and companies/projects looking to set their base in Switzerland. 

If things go smoothly, we will most likely witness the rise of an important player in the emerging blockchain-based industry.

Back to Zug's Bitcoin pilot program. During the roundtable discussions following the transaction and press meeting, I did a short presentation with the main goal of explaining that blockchains can be "more than money" and how this is impacting the current regulatory environment around the world.

![Zug Roundtable]({{ site.baseurl }}/content/images/zug-roundtable1.jpg)

While touching on Ethereum and new concepts such as decentralized applications and organizations, I was surprised at how well everyone seemed to intuitively grasp these new abstract notions and concepts.

One of the follow-up questions asked at the table was regarding the social implications for blockchains in general, offering me the perfect chance to talk about AKASHA as a catalyst for freedom of expression and how the technologies used fit together into the picture.

At first sight, everyone at the table seemed to appreciate the importance of things such as online privacy and freedom of expression, so I think we will see many refreshing initiatives flourishing in this sort of innovation-friendly environment. 

![Zug Roundtable]({{ site.baseurl }}/content/images/zug-roundtable2.jpg)

The next steps should be very interesting as the feeling we all had after the roundtable was one of optimism and enthusiasm. 

It felt like the Crypto Valley dream is within reach and that history is in the making.

### Closing Thoughts: Preparing for the Marathon

During these last few weeks we’ve tried as much as possible to stay away from the drama being stirred around "the DAO" fiasco and focus instead on delivering a working alpha version. That went well in our opinion, and we feel that **we are close to releasing a pre-alpha version very, very soon**. 

Nothing is set in stone yet, but things are looking promising.

The plan is to do a slow rollout and gradually test the features, starting with the core publishing function. After the initial tests are satisfactory, we will proceed with the rest of the features such as quadratic voting, mentions, search and discovery of content, and so on.

We believe that this approach will allow us to isolate potential problems in a more efficient manner while testing our smart contracts one by one with real users and real content.

We are eager to test and observe how well the ideas we’ve been brainstorming for the past months will behave in the wild. If what we are imagining is even remotely close to what will happen in the “real world” then we are set for a truly epic journey into the ether, and beyond.

Many, many thanks to the **over 3000 people** who signed up for the alpha release and to the Ethereum community as a whole for the incredible support and enthusiasm! Special thanks go also to all the people that have helped and encouraged us along the way - you are awesome!

Even if in some regards it feels like we're approaching a sort of "finish line," we realize that this represents just the starting point for the long journey that lay ahead of us all. This is both exciting and humbling as we occasionally glimpse the implications of what we are building while discussing various scenarios during our time away from computers. 

We feel that by pushing the limits of what is possible we can reshape online publishing and create better web. A web where freedom of expression and privacy are not optional, but fundamental standards embedded into code. 

And best of all, we are almost *there*!

[AKASHA](http://akasha.world/){:target="_blank"} is nearly fully materialized and ready to flow into the Internet.

----

**About the Author**

Mihai Alisie is the Founder and CEO of [AKASHA](http://akasha.world/){:target="_blank"}.

He has been actively involved in the blockchain technology space, since 2011 when he created with [Vitalik Buterin](http://vitalik.ca){:target="_blank"} the world’s first Bitcoin centric publication - [Bitcoin Magazine](https://bitcoinmagazine.com/){:target="_blank"}. He served as Editor-in-Chief for the magazine, until late 2013, when he joined Vitalik in founding the [Ethereum project](https://ethereum.org/){:target="_blank"}.

In the early days of Ethereum, Mihai led the Swiss efforts to establish the business infrastructure and legal framework critical for the Ethereum “pre-sale” campaign. Following the successful Swiss setup, he oversaw the Ethereum operations as Strategic Manager and Vice-President of the Ethereum Foundation, until late 2015, when he focused his attention on making the AKASHA dream a reality.

![Mihai Alisie]({{ site.baseurl }}/content/images/Mihai275x.jpg)

Twitter: [@MihaiAlisie](https://twitter.com/MihaiAlisie){:target="_blank"} | 
LinkedIn: [Mihai Alisie](https://www.linkedin.com/in/mihaialisie){:target="_blank"} | 
Contact: [mihai@akasha.world](mailto:mihai@akasha.world)
