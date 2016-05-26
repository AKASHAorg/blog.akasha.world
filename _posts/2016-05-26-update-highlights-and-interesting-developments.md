---
layout: post
title: "The First Three Weeks: Highlights & Interesting Developments"
timezone: Europe/Zurich
date:   2016-05-26 00:00:01
image: Spacelapse.jpg
comments: true
tags: AKASHA, update, highlights, developments, ethereum, ethcore, IPFS, orbit-db
published: true
---

Many things have happened since we unveiled [AKASHA](http://akasha.world/){:target="_blank"}. On May 3rd, the [announcement blogpost](http://blog.akasha.world/2016/05/03/unveiling-akasha/){:target="_blank"} received a warm welcome and was the most upvoted thread on [/r/ethereum](https://www.reddit.com/r/ethereum/comments/4hm678/unveiling_akasha_a_nextgeneration_social_media/){:target="_blank"} and [/r/ethtrader](https://www.reddit.com/r/ethtrader/comments/4hm6kk/unveiling_akasha_a_nextgeneration_social_media/){:target="_blank"}, which are the biggest Ethereum Reddit communities. The feedback was overwhelmingly positive across the community, leading to over **200 signups** for the alpha release in the first 24 hours. 

![200 Signups Tweet]({{ site.baseurl }}/content/images/24h-tweet.jpg)

Following the initial splash, we received a good deal of news coverage from various publications in the blockchain space, but the best was yet to come, as a few days later, we hit the front page of hackernews. Before the [hackernews post](https://news.ycombinator.com/item?id=11678810){:target="_blank"}, we were at almost 1000 signups already, but thanks to the increased exposure, we are nearing, at the time of writing, almost **2000 signups**.

![Hackernews Frontpage]({{ site.baseurl }}/content/images/hackernews-frontpage2.jpg)
 
![Hackernews Tweet]({{ site.baseurl }}/content/images/hackernews-tweet.jpg)

We are both ecstatic and humbled by the warm response, as it is ***way beyond*** our wildest expectations. Many thanks, again, to everyone with the courage to join us in this adventure into the ether. 

At the other side of the Ethereum ecosystem, around the same time as our unveiling, our friends from Ethereum Foundation and ConsenSys made a big announcement as well - the launch of [BTC Relay](http://btcrelay.org/){:target="_blank"} on the main Ethereum network.

This is a **big deal** and ties in with what [Rune Christensen](https://twitter.com/RuneKek){:target="_blank"}, founder of the [Maker](https://makerdao.com/){:target="_blank"} project, explained a while ago. One of the best things Ethereum offers, by default, is the incredible synergy that all dapps living on the network can benefit from. 

![BTCrelay.org]({{ site.baseurl }}/content/images/BTCrelay-website.jpg)
 
![BTCrelay Tweet]({{ site.baseurl }}/content/images/thanks-BTCrelay-tweet.jpg)

In our case, BTC Relay makes possible, at least in theory, the support of both Ether and Bitcoin as native tokens in our beta, hopefully, in the process, bridging the gap formed between these two amazing crypto communities. 

In the middle of all this craziness, we had a call with [Juan Benet](https://twitter.com/juanbenet){:target="_blank"} and the friendly [IPFS team](http://ipn.io/){:target="_blank"}, regarding our roadmaps for the future, trying to find the best way to collaborate with the [IPFS project](https://ipfs.io/){:target="_blank"}. 

![Thank You IPFS]({{ site.baseurl }}/content/images/thanks-ipfs-tweet.jpg)

We agreed to help with the Electron IPFS tests, since we're already using [Electron](http://electron.atom.io/){:target="_blank"} as part of our tech stack. We then covered some of the pain points encountered in IPFS development; one of them was getting the IPFS API to work on Windows. 

In our case, this is important, as our alpha signup list revealed (not to anyone's surprise really) there are **many** Windows users out there. This is why, after a few days of intense research and development, Marius came up with a way to make the IPFS executable download seamlessly on multiple platforms and architectures, Windows included. Hooray for Windows users!

The solution was received with enthusiasm by our friends from IPFS, and they will use a similar approach to deliver the right IPFS binaries across multiple platforms soon :)

![IPFS API Windows]({{ site.baseurl }}/content/images/ipfs-wrapper-issue.jpg)

During this call, we also talked with [Samuli Pöyhtäri](https://twitter.com/haadcode){:target="_blank"}, the creator of the awesome IPFS based database [Orbit-DB](https://github.com/haadcode/orbit-db){:target="_blank"}. We've been eyeing Orbit-DB for a while, as we researched a number of options for solving the client-side storage problem - from SQL to Level DB, from RethinkDB to BigChainDB, and beyond.

Samuli was helpful and offered answers that sounded like music to our ears. We are now working together on some cool and exciting things, but we'll cover that in more detail in the next section.

Later in the week, we received a special visit in our Bucharest hacklab from [Dr. Gavin Wood](https://twitter.com/gavofyork){:target="_blank"} and [Marek Kotewicz](https://twitter.com/iDebris5){:target="_blank"} from [Ethcore](https://ethcore.io/){:target="_blank"}. We haven't seen each other since before the [Ethereum Genesis](http://etherscan.io/block/0){:target="_blank"}, and we had a great time catching up.

![Ethcore In The House]({{ site.baseurl }}/content/images/ethcore-visit.jpg)

During the visit, we talked about the challenges we face on the Ethereum side of things, followed by a demonstration of what [Parity](https://github.com/ethcore/parity){:target="_blank"} can do. At the moment, we are using the [Go-Ethereum](https://github.com/ethereum/go-ethereum){:target="_blank"} implementation (Geth); however, Parity looks very interesting, especially for blockchain size and sync time. 

Gav and Marek, later, shared with us some of their plans, in the process, exploring ways we can collaborate. After the discussions, one thing is sure - we'll continue to experiment with Parity as it matures and see if/when it makes sense to switch from Geth.

![Gav In The Mix]({{ site.baseurl }}/content/images/ethcore-brainstorming.jpg)

The discussions later converged into a brainstorming on the smart contracts architecture, the session resulting in some interesting insights into how things could be improved. For example, we discussed how being a good blockchain citizen comes with rewards in the form of recovered gas when cleaning up the old deployed contracts via the `suicide` function.

All this being said, I would like to recap by giving **kudos** to Joseph Chow and the ConsenSys team for making BTC Relay happen, a **big thank you** goes to the IPFS/Orbit-DB team for being so awesome and willing to collaborate, and **special thanks** go to the ethcore team for their visit and all the invaluable knowledge shared. 

I'm convinced we can - and we will - build epic things together. 

### (Very) Interesting Developments
> “Creating a better future requires creativity in the present.” ― Matthew Goldfinger

![IPFS FTW]({{ site.baseurl }}/content/images/IPFS-background.jpeg)

At the beginning of this entry, we started to collaborate more closely with the guys from IPFS and Orbit-DB. This led to an experiment, which we think might benefit both the Ethereum and IPFS ecosystems.

[Orbit-DB](https://github.com/haadcode/orbit-db){:target="_blank"} is one of the most interesting databases explored, while looking into ways to solve the problem of client-side storage for our dapp. However, Orbit-DB uses a [redis](http://redis.io/){:target="_blank"} server to notify nodes when a new hash appears on the network and needs to be synced locally, as an intermediary solution, until IPFS implements a [pub-sub schema](https://github.com/ipfs/go-ipfs/pull/2599){:target="_blank"} at protocol level. 

We weren't happy with this solution, as it would introduce a [single point of failure](https://en.wikipedia.org/wiki/Single_point_of_failure){:target="_blank"} in our dapp architecture, so we had to take a break and think it through. 

While thinking if we should still go forward with Orbit-DB, considering the above, an idea sparked inside the AKASHA hacklab, during a conversation between Marius and Sever - *"what if instead of redis we use smart contracts for emitting events?"*

This is how, by combining IPFS, Orbit-DB, and Ethereum smart contract events, we may have created what seems to be the "missing link" between IPFS and Ethereum. 

And this opens the path to many interesting things that weren’t possible before. 

In our case, Orbit-DB morphed into a decentralized client-side storage/database for fast access to followed sources, with custom indexes, without the smart contract limitations, while allowing queriable contract events/logs. 

It might help to imagine these Orbit-DB instances as localized spheres of cached data from the main Ethereum network for fast and customizable access. 

Within the AKASHA dapp, Orbit-DB would work like a local cache of the smart contract events, which helps us speed the access to information stored on the Ethereum network, with the added bonus of read-only **offline** access, which comes in handy when no Internet connection is available.

On this note, people asked, in various channels, if we are planning to use [Swarm](http://swarm-gateways.net/bzz:/swarm/ethersphere/orange-papers/2/smash.pdf){:target="_blank"} and how we see things moving forward, once Swarm is launched. 

We know that some of the things we are trying to accomplish with this experiment might work better on Swarm (when launched), as it works on top of Ethereum, by default. But we wanted to have something working **now**, and IPFS is an awesome technology, which is live **right now**. 

Moreover, IPFS/Orbit-DB has a great team that will collaborate and experiment with these new things. This was enough for us to put in the time to experiment and make it happen. 

When Swarm will be live, we will definitely experiment with it to see how it fits with our needs, and depending on our findings, we will make a decision to see which one is best for our dapp. In the meantime, we will continue to work on this, as it allows us to push forward with AKASHA, as a fully functional decentralized application. 

More details, regarding this experiment, will follow in another blogpost soon, as it is an interesting topic that deserves an entry of its own. 

### Final Thoughts
> “Never doubt that a small group of thoughtful, committed, citizens can change the world. Indeed, it is the only thing that ever has.”  ― Margaret Mead

![Keep your coins, I want change]({{ site.baseurl }}/content/images/Banksy-change.jpg)

Looking back to the past three weeks, it feels both exciting and reassuring to see we are not alone in this. The general feeling we got is that users and developers from around the world have been waiting for something, like AKASHA, to appear. 

We are blown away by the positive response, and we are doing our best to get an alpha version in your hands soon. Now, as with every software project, it is difficult to give an exact ETA, so please bear with us as we are approaching the finish line. 

With all that in mind, it’s good to remember, occasionally, that **everything**, starting from the decentralized [architecture](https://en.wikipedia.org/wiki/BitTorrent){:target="_blank"} to the [Ethereum chain](https://github.com/ethereum/wiki/wiki/White-Paper){:target="_blank"} to [IPFS](https://github.com/ipfs/papers){:target="_blank"} and going all the way through ***every piece*** of our tech stack, ***is a great experiment***, as we’re [standing on the shoulders of ever-growing giants](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants){:target="_blank"}, accelerating in their growth. 

In a way, it could be said that we are crafting a new ethereal canvas and the tools to freely express yourself on this new medium. However, be prepared - unexpected errors and hidden bugs are expected to be revealed through your activity. So when you'll stumble upon things like this, smile and remember that you’re experiencing the bleeding edge of what can be achieved with *highly experimental technologies*. 

If you have signed up for the alpha, when the time comes, you will receive an invitation and instructions on how to get started. If everything goes according to plan, you will soon have, at your fingertips, something that can really make a positive difference on a global scale. 

The alpha release will most likely not be *perfect*, but every great journey must begin with a first step. As long as we all recognize **why** we need to take this step together, we can get over whatever will come in our way. 

So, in a few weeks from now, when you write your first entry on AKASHA, remember you are writing history, while helping us, at the same time, to build a better channel of expression for you and everyone else. 

Thank you for being part of this! 

----

**About the Author**

Mihai Alisie is the Founder and CEO of AKASHA.

He has been actively involved in the blockchain technology space, since 2011 when he created with [Vitalik Buterin](http://vitalik.ca){:target="_blank"} the world’s first Bitcoin centric publication - [Bitcoin Magazine](https://bitcoinmagazine.com/){:target="_blank"}. He served as Editor-in-Chief for the magazine, until late 2013, when he joined Vitalik in founding the [Ethereum project](https://ethereum.org/){:target="_blank"}.

In the early days of Ethereum, Mihai led the Swiss efforts to establish the business infrastructure and legal framework critical for the Ethereum “pre-sale” campaign. Following the successful Swiss setup, he oversaw the Ethereum operations as Strategic Manager and Vice-President of the Ethereum Foundation, until late 2015, when he focused his attention on making the AKASHA dream a reality.

![Mihai Alisie]({{ site.baseurl }}/content/images/Mihai275x.jpg)

Twitter: [@MihaiAlisie](https://twitter.com/MihaiAlisie){:target="_blank"} | 
LinkedIn: [Mihai Alisie](https://www.linkedin.com/in/mihaialisie){:target="_blank"} | 
Contact: [mihai@akasha.world](mailto:mihai@akasha.world)
