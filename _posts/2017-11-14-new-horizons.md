---
layout: post
title: "New Horizons"
date:   2017-11-14 00:00:01
image: akasha-in-cancun.jpg
comments: true
tags: AKASHA, Ethereum, IPFS, Beta, Release, DEVCON, Decentralized Social Network
published: true
---

Many, many things happened since our last update. Following our last alpha release, we started working on an entirely new dapp, in parallel with a complete redesign of the whole user experience. In other words, the sparse updates were not caused by a lack of activity, quite the opposite. Now, after much hard work, we are extremely happy to change gears and announce that **[the signups for the AKASHA beta version are now open!](https://akasha.world/){:target="_blank"}** \o/

### DEVCON 3: Strength in Numbers

![AKASHA in Cancun]({{ site.baseurl }}/content/images/akasha-team.jpg)

The [DEVCON 3 event](https://ethereumfoundation.org/devcon3/){:target="_blank"} was our second Ethereum conference participating as the AKASHA project, and it was *impressive*. The sheer number of people present at the event was simply astonishing. We couldn’t really imagine what a group of ~2000 looked like before, but now we can. 

It is both comforting and awe-inspiring to experience the relatedness found in shared interests, ideas, and projects with so many other like-minded people. 

That feeling of “belonging” we are subconsciously longing for was overflowing in the International Convention Center in Cancun during those four magical days. What I was only daydreaming about in 2013-2014, as co-founder of Ethereum, was **happening right in front of my eyes - a worldwide community of people co-creating today a better Web of tomorrow.** Epic.

![AKASHA DEVCON 3 Agenda]({{ site.baseurl }}/content/images/devcon-agenda.jpg)

AKASHA was scheduled to close the epic DEVCON3 as **the last presentation on the last day.** We were not exactly sure if this was a good thing, or if it brought extra challenges associated with an audience that was tired after 4 days of great presentations. Little did we know!

Fast forwarding to November 4th, at 4:20 PM we were making the final preparations for our presentation. The headset microphones were being installed backstage and I was restarting the Keynote app “just in case”. 

This was the first time we were showcasing our progress in months, and it was the biggest event we participated in as presenters. After an initial tech hiccup (inevitably) we managed to get the presentation going, and the audience was simply fantastic. For those of you that read these lines and were present - THANK YOU, YOU ARE AWESOME!

![DEVCON ON]({{ site.baseurl }}/content/images/devcon-on.jpg)

Words cannot explain the emotions overwhelming us. Those interested in watching the presentation and the beta demo can find the video at the bottom of this post, next to the Beta signup links!

### A Peek Behind The Curtain: From Alpha To Beta And Beyond

![DEVCON Stage]({{ site.baseurl }}/content/images/devcon-stage.jpg)

During the past ten months we have been focusing on the following:

- Building a fully functional AKASHA web version with IPFS.js and Metamask
- Improving the overall performance and stability of the new dapp
- Designing and implementing a new UX/UI
- Optimizing the Ethereum dapp architecture, gas footprint, and modularity for the next round of experiments
- Brainstorming and experimenting with various token ideas in the search for a good starting point

The biggest challenge we faced, and still do face, is the nascent state of the infrastructure on top of which we are building. Both Ethereum and IPFS are very ambitious technologies seeking to push the boundaries of previous experiments. These projects develop and evolve fast, but the documentation is hard to be kept up to date and information on what “can be” and “cannot be” or “how it should be” done is still scarce. 

This is the side-effect of the fast-evolving nature of things; we have to constantly remind ourselves that this is pioneering at its best, and we all still have a lot to learn. 

Although it can be seen as intimidating by some, for us it was liberating because it pushed us into a trial-and-error-error-error mindset. There are no “right” or “wrong” answers yet, and we’ll probably learn along the way how we can build something better. 

Yet, at the same time, you also have to start “somewhere” and in our case it meant designing a simple “publish flow” that combines Ethereum and IPFS in a way that is actually “usable” through a user-friendly interface. For us, this was the alpha release. 

To give you an idea, the alpha version of the user interface took about 6 months of work to design (mostly in Keynote) and almost a year to implement in code. Even if far from perfect, it offered us something “good enough” to spark the interest of the Community. The beta redesign has been a work in progress for 10 months now, with development moving in parallel. We believe that the wait will be worth it! 

On this note, you can find an example of a good lesson we learned and applied in the beta with a big impact on the user experience - fetching IPFS resources.

The classic “Freedom of Speech Status: Loading” you encountered so often in the alpha:

![Alpha Loading]({{ site.baseurl }}/content/images/alpha-load.jpg)

Lesson learned: fetching all IPFS resources at the same time is not ideal

![Loading Map]({{ site.baseurl }}/content/images/map-load.jpg)

Lesson applied: fetch the IPFS resources individually. 

![Beta Loading]({{ site.baseurl }}/content/images/beta-load1.jpg)

TA-DA!

![Beta Loading]({{ site.baseurl }}/content/images/beta-load2.jpg)

Aside from all the nice and shiny stuff, the elephant in the room is “how will the infrastructure hold up with the added transaction and data volume resulting from using AKASHA?”. In the alpha, we almost reached 10,000 identities created. However, the UX and features were (intentionally) quite limited. Plus, we were using a private Ethereum chain to keep things simple.

On the other hand, the beta was designed to make continued use a more intuitive and enjoyable experience. This, combined with a Web version accessible from “normal browsers” such as Chrome, will hopefully generate enough activity to offer us a glimpse at further possible optimizations and their implications. 

The assumption, in this case, is that the more people who will try the beta, the more clear the answers will become (through more data). On top of this, we can then build better models and solutions. This is why for the beta, our success will be measured in terms of transaction output and further optimizations in anticipation of the AKASHA ONE (1.0) release on the main Ethereum network.

Also, since the beta will be living on a public test network, we can begin exploring the synergies with other projects from the ecosystem, with ENS being just one simple yet meaningful example.

### Main Beta Mission: Pushing The Limits

![Stress Testing]({{ site.baseurl }}/content/images/devcon-stage2.jpg)

The beta smart contracts have been deployed on the Rinkeby test network and are undergoing intense tests at the moment. A big THANK YOU goes to [Péter Szilágyi](https://twitter.com/peter_szilagyi){:target="_blank"} and the Ethereum Go team for all the help to get things working!

**We invite everyone in the Community to join us in the beta release because we need help with:**

- Stress testing the new smart contracts architecture and security
- Stress testing the carrying capacity of the Ethereum network and blockchain
- Stress testing the carrying capacity of the IPFS network
- Testing our first crypto economic assumptions & incentive structures
- Testing the new information architecture and UX/UI
- Testing the fully-functional AKASHA web version (IPFS.js and MetaMask)
- Collecting feedback and formulating the main Ethereum chain deployment plan

Since one of the main goals of the beta is to stress test the infrastructure and see how far can we take it, we could choose the number of users as a metric with 1K, 5K, 10K, 20K, 30K … 100K+ as milestones. It will all come down to how much transactional output a decentralized social network with many users will generate, and how well the Ethereum network can take it. 

Even if the 100K milestone might seem a bit crazy, the current biggest Ethereum communities are sizeable - https://www.reddit.com/r/ethereum/ has almost 150K readers and https://www.reddit.com/r/ethtrader/ has over 100K readers. There is definitely some overlap between the two subreddits, but the main idea is that if we can engage the online Ethereum community to stress test Ethereum itself, we might actually be able to do it - together.

If we can uncover insights and answers to questions such as “Should we actively engage the Ethereum mining community for raising the gas limits in anticipation of the main chain deployment?” and “What would be the gas limit that allows AKASHA and the entire Ethereum ecosystem to comfortably coexist on the same chain?” we think that we’ll be well on our way to a successful launch.

With this in mind, we invite everyone to [join us on our new Discord channel](https://discordapp.com/invite/JqqKasJ){:target="_blank"} while we build the necessary tools to have the entire community organizing and chatting in AKASHA directly.

### Highlight: The AETH Crypto Economic Experiment

After long discussions and thought experiments, we chose the starting point for our token exploration. A big ‘thank you’ is in order for everyone who participated in the conversations that culminated in this first token iteration! 

![States Overview]({{ site.baseurl }}/content/images/token-states2.jpg)

The AETH token is currently modeled to have multiple states, with the token being transferable in some states and non-transferable in others. The introduction of states in the token brings with it, in theory, a system of checks and delays that should alleviate some of the problems associated with manipulation and Sybil attacks. 

Here is a brief AETH states overview, followed by a short explanation for each:

- **AETH** is a transferable, ERC 20 compatible token, living on the Rinkeby test network
- **Mana** is non-transferable and is obtained by locking AETH for X time at Y ratio (Manafied AETH). The Mana amount regenerates every day for as long as AETH remains locked, in a “Manafied” state.
- **Essence** is non-transferable and is obtained through positive contributions. It can be burned to mint new AETH into existence. When people use their Mana to vote on artifacts, the authors can collect the burned Mana as Essence.
- **Karma** is not a state, but rather a score tracking user contributions. For every unit of Essence collected, the user receives also Karma. Karma is used for defining milestones, thresholds and unlocking functionality within the dapp.

##### Aether
AETH (Aether) implements an ERC 20 token interface and has the standard features found in most ERC 20 tokens, but with a twist - AETH can be “locked”/“staked” to generate Mana. The AETH can also be “unlocked”, after a predefined delay associated with this action, at the cost of Mana.

Important note: When using AKASHA, the users will not consume their AETH. The interactions consume Mana, which regenerates daily.

##### Mana
Mana acts as a crypto fuel inside the AKASHA ecosystem, and is required for various interactions in the dapp (publishing, commenting, voting, etc). The user’s AETH balance is not affected by interactions, only Mana and ETH (for gas) is spent. 

The Mana is regenerated every 24 hours, with the unused mana from the previous round being lost. The artifacts created by burning Mana can, in turn, generate Essence from the upvotes of other users.

##### Essence
The Essence can be consumed to mint new AETH tokens into existence if certain thresholds defined as a conditions at token protocol level are met. 

When people burn their Mana to vote on content, the authors can collect the burned Mana as Essence. The users voting with the majority in the initial round of voting (deciding the quality of an artifact) are also rewarded with Essence equal to the Mana they burned to vote.

##### Karma
Karma is a form of proto-reputation and reflects the user’s positive contributions associated with collecting Essence. The Karma does not decrease when Essence is converted to AETH.

Karma also unlocks features inside the AKASHA dapp depending on the score of the user. One example is the ability to create and curate public lists: everyone can create and curate their local lists as bookmarks or collections, but only those that have actively contributed can create a public list. This tries to ensure higher-quality curation lists.

Finally, Karma is also used in Formula K to determine the Mana costs for interactions within AKASHA - the users with higher Karma scores will burn less Mana for interactions such as publishing, commenting and so on. This will gradually decrease the Mana costs for the most active users, thus increasing the number of interactions possible with the same amount of AETH locked.

Below you can find an overview of the flow between the states above and how they interact:

![Token States Flow]({{ site.baseurl }}/content/images/aeth-flow.jpg)

More information can be found in our presentation and the full model will be released on the AKASHA beta, which takes us to the next topic.

### Crowdsourced Crypto Economics: Towards Token 2.0

![TokensTokensTokens]({{ site.baseurl }}/content/images/stargate-blueprint.jpg)

This first (and presumably imperfect) theoretical design of AETH will be live tested with real participants in the beta release. The token architecture and future direction will be discussed openly on the AKASHA dapp under various tags such as #akasha #bugbounty #CryptoOlympics #AETHresearch etc.

To give you an example of how this works in the actual application, the user would simply add a tag column and then they would be up-to-date with everything posted in that particular stream of information. 

![Adding a Tag]({{ site.baseurl }}/content/images/tag-add1.jpg)

The entries in this tag can be used as improvement proposals or counter-proposals, whereas the comments can serve as the debate arena. The voting mechanism will allow the best ideas to organically bubble up from the Community, and will thus help to identify them.

When promising ideas are identified, the next stage would be closer analysis and an implementation in code to see how the concept holds up in practice.

![Tag added]({{ site.baseurl }}/content/images/tag-add2.jpg)

In the process, we will gather real data and feedback in a test-driven environment in order to gain insights into what makes a great social network token work and, most importantly, why? 

Together we think we can find some really satisfying answers to these questions! 

Also, **to add a little extra incentive to the mix, IF a token 2.0 will result from this experiment we are contemplating allowing ONLY the Ethereum keys created in the AKASHA alpha and beta to participate in the crowdsale. This means that only the people that have helped with testing the AKASHA alpha and beta version will be included in the AKASHA ONE token genesis event.** 

**This way we would reward the people testing the application with the right to participate in the main Ethereum network genesis, and even those that are seeking just to trade or flip the token(s) will end up contributing toward improving our code through their simple participation in the beta.**

We’re looking forward to hearing the community’s thoughts on this!

### The End? Nope, Just Another Beginning!

![Seatbelts On!]({{ site.baseurl }}/content/images/Dragonv2.jpg)

> “The paths are not to be found, but made. And the activity of making them changes both the maker and the destination.” — John Schaar

The unknown is part of every adventure. 

Even if we don’t have all the answers yet, we believe that together we can reach new, emergent, shared understandings. Just one short glimpse into the future can offer us enough information to at least point us in the direction in which we should take our next steps.

If one thing is clear, it is that no one has all the answers in this Crypto Adventure.

Not even Vitalik.

We are all winging it as we go, to the best of our abilities. It’s just that some people are winging it better than others. 

Through this lens, people that are successfully building things in this space are applying a hacker mindset for solving problems as they appear. This process is far from what people usually understand when we say “expert”. 

That being said, I strongly believe that this particular mindset/skill/talent is admirable on its own, without dressing it as something else – some sort of higher state that is out of reach for mere mortals. We all have it in us.

It would be refreshing to see more people approaching things from this perspective rather than trying to pose as “experts” and other fancy self-appointed labels. It would be less intimidating for someone looking to get involved in this space. 

“If they are winging it, maybe I can wing it too!” vs. “Oh, they are blockchain experts and I am just a _______. Why even bother?”

At least this is what we want to achieve with our Crypto Economic Olympics - invite as much cross-disciplinary collaboration as possible in the search of truly groundbreaking ideas, no matter if they arise from “blockchain experts” (whatever that means), academicians, musicians, journalists or a gamer’s mind. 

The more diverse the group searching for answers, the better our chances of uncovering [entire flocks of black swans](https://en.wikipedia.org/wiki/Black_swan_theory){:target="_blank"}. The collective intelligence of the group increases with diversity, and one thousand half-baked ideas can come together into something completely new. 

We don’t expect it to happen overnight, and it will probably take many iterations in the search for the best possible solutions.  Nonetheless, when that moment of insight is reached, the collective mind will identify it and nothing will ever be the same again. 

We will reach new levels of understanding and possibilities.

Two years After Ethereum, “How far can we take it?!” is still a question without an answer. 

**Join us in the beta and [let’s find out together!](https://akasha.world/){:target="_blank"}**

<iframe width="720" height="440" src="https://www.youtube-nocookie.com/embed/ugbRyZSPfYE?rel=0&amp;showinfo=0&amp;start=12680" frameborder="0" allowfullscreen></iframe>


----

**About the Author**

Mihai Alisie is the Founder of [AKASHA](http://akasha.world/){:target="_blank"}.

He has been actively involved in the blockchain technology space, since 2011 when he created with [Vitalik Buterin](http://vitalik.ca){:target="_blank"} the world’s first Bitcoin centric publication - [Bitcoin Magazine](https://bitcoinmagazine.com/){:target="_blank"}. He served as Editor-in-Chief for the magazine, until late 2013, when he joined Vitalik in founding the [Ethereum project](https://ethereum.org/){:target="_blank"}.

In the early days of Ethereum, Mihai led the Swiss efforts to establish the business infrastructure and legal framework critical for the Ethereum “pre-sale” campaign. Following the successful Swiss setup, he oversaw the Ethereum operations as Strategic Manager and Vice-President of the Ethereum Foundation, until late 2015, when he focused his attention on making the AKASHA dream a reality.

![Mihai Alisie]({{ site.baseurl }}/content/images/Mihai275x.jpg)

Twitter: [@MihaiAlisie](https://twitter.com/MihaiAlisie){:target="_blank"} | 
LinkedIn: [Mihai Alisie](https://www.linkedin.com/in/mihaialisie){:target="_blank"} | 
Contact: [mihai@akasha.world](mailto:mihai@akasha.world)
