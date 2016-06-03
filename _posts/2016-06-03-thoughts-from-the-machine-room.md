---
layout: post
title: "Thoughts From The Machine Room: Ethereum Gas Price, Dapps & Adoption"
timezone: Europe/Zurich
date:   2016-06-03 00:00:01
image: Ethereum-Gas-AKASHA.jpg
comments: true
tags: AKASHA, Ethereum, Gas, Homestead, Dapps, Adoption
draft: true
---

We are now over three months into [Homestead](https://blog.ethereum.org/2016/02/29/homestead-release/), and it has been an intense ride as we've seen increased mainstream media attention, massive [ETH price increases](http://ethereumprice.org/), and witnessed the birth of "[The DAO](https://daohub.org/)" as the [largest crowdfunded project](https://en.wikipedia.org/wiki/List_of_highest_funded_crowdfunding_projects) **ever**.
 
All these are reasons to celebrate and be grateful that we are lucky enough to participate in something so epic. Many people, myself included, were not expecting things to move quite so quickly.
 
The mind blowing part is that things don't appear to be slowing down at all - on the contrary, the rhythm seems to be accelerating.
 
With all these exciting things happening in such a short while, it's easy to get lost in this rush and forget **why we started doing this thing** in the first place. So, let's take a few moments to look back and think about why we started this, where we are, and where we want to go as the only way to shape our future is by taking control of the present.

### The Rise of Ethereum & Ether: The Side Effects of Success
> *“Eighty percent of success is showing up.” ― Woody Allen*

Ethereum made the concepts of decentralized applications and organizations possible by introducing ETH as a "cryptofuel", which can be used to pay the “gas” used for computation on its turing-complete blockchain.
 
This is how Ethereum was described as a "platform for decentralized applications", a “blockchain apps platform” or, more recently, a “shared world computer”. These descriptions differentiated it from the sea of “altcoins” that was floating around the blockchain space and made it easier for people to understand that Ethereum is “more than an altcoin”, in the sense you can build cool things both with and on it.
 
This paradigm shift sparked the imagination of developers worldwide and even attracted the attention of established institutions and corporations from multi-national banks to international corporations.
 
However, in a paradoxical way, the recent wave of positive news and events that brought along the ETH price increase also boosted the costs of running these groundbreaking decentralized applications and organizations.
 
Before continuing, for those that haven’t yet wrapped their heads around the concept of “Ethereum gas”, I highly recommend watching this presentation, given by Joseph Chow:

<iframe width="560" height="315" src="https://www.youtube.com/embed/dd-ajiMl4HY" frameborder="0" allowfullscreen></iframe>

The side effect of ETH price increase is negligible when talking about basic things such as sending ETH from one account to another since the equivalent in USD would be around ~$0.007 at the current prices for ~21K gas to cover the transaction.
 
The problem becomes more visible when we look at how this affects decentralized applications and organizations. If we take “the DAO” as an example, something as simple as transferring DAO tokens from one address to another or casting a vote can reach fees between $0.05 - $0.1 to cover the computation gas.
 
We learned of this problem as we were experimenting with an identity system for AKASHA where each profile had its own smart contract. We touched upon this ID system [a while ago](https://www.reddit.com/r/ethereum/comments/4hm678/unveiling_akasha_a_nextgeneration_social_media/d2qyuhx), but briefly, this approach comes with increased extensibility at the cost of complexity. Our tests with this method revealed fees as high as ~$0.16 for ~500K gas used for deploying your own smart contract profile.
 
We were expecting higher costs with this approach and there are probably places where we can optimize the gas usage, but this is beside the point of this article. Instead, **let’s focus on the bigger picture as a community**. We will cover the nitty, gritty, smart contract details in another post.
 
Here is an overview of the Ethereum market cap/Ether price evolution, courtesy of [coincap](http://coincap.io/):

![Ether Price Evolution]({{ site.baseurl }}/content/images/ETH-Price.jpg)

And here, is an overview the Ethereum gas price evolution during the past few months:

![Ethereum Gas Price Evolution]({{ site.baseurl }}/content/images/Gas-Price.jpg)

You can clearly observe in the next chart how the gas price adjustment introduced with the homestead release impacted the gas price across the network:

![Ethereum Gas Price Since Homestead]({{ site.baseurl }}/content/images/Gas-Price-Homstead.jpg)

The graph above also shows how the gas price has not changed, even if the price per ETH more than doubled.

### The Bigger Picture
> *“Whatever the mind can conceive and believe, it can achieve.” ― Napoleon Hill*

Homestead brought with it the first gas price adjustment and to a certain extent, the issue we’re facing now related to the ETH/Gas price increase was to be expected, as [pointed out by Vitalik in the last discussion on this topic](https://www.reddit.com/r/ethereum/comments/499a7w/gas_prices_are_already_kinda_down_to_20_shannon/).
 
Today, the ETH price is more than double compared to when the first gas price adjustment was made, and we think another gas price adjustment is needed. These high gas prices are harmful to the Ethereum ecosystem in the long run, as they slow adoption down by making it too expensive to build and run things on it.
 
Oversimplified, I think things look like this:
 
High Gas Price -> Less Dapps -> Less Adoption -> Smaller Ecosystem -> Smaller Market Cap -> Everyone Loses
 
VS
 
Low Gas Price -> More Dapps -> More Adoption -> Bigger Ecosystem -> Bigger Market Cap -> Everyone Wins
 
Maybe we are more aware of this problem as we are on the frontline of dapp development with [AKASHA](http://akasha.world/). However, I'm sure everyone would benefit from another gas price adjustment because this would lower the entry barriers while increasing the chance of adoption at large scale – and, in the end, **adoption is critical for technologies like Ethereum**.
 
This is an open call for a new discussion on how we can deal with the problem of gas prices now and how we can tackle this issue to keep the Ethereum World Computer accessible to as many developers and users as possible.
 
**Ethereum was created to serve humanity, and it cannot fulfill its world-changing destiny if it becomes too expensive to use.**
 
All this being said, one of the most amazing things Ethereum has, besides the fantastic technology, is this great community united by a pure passion for ideating, co-creating and iterating.
 
This is why, I’m sure we can fix this one as well, together. [Join the community discussion here](reddit.com/r/ethereum/).

![Ethereum World]({{ site.baseurl }}/content/images/Ethereum-AKASHA-Project.jpg)

----

**About the Author**

Mihai Alisie is the Founder and CEO of [AKASHA](http://akasha.world/){:target="_blank"}.

He has been actively involved in the blockchain technology space, since 2011 when he created with [Vitalik Buterin](http://vitalik.ca){:target="_blank"} the world’s first Bitcoin centric publication - [Bitcoin Magazine](https://bitcoinmagazine.com/){:target="_blank"}. He served as Editor-in-Chief for the magazine, until late 2013, when he joined Vitalik in founding the [Ethereum project](https://ethereum.org/){:target="_blank"}.

In the early days of Ethereum, Mihai led the Swiss efforts to establish the business infrastructure and legal framework critical for the Ethereum “pre-sale” campaign. Following the successful Swiss setup, he oversaw the Ethereum operations as Strategic Manager and Vice-President of the Ethereum Foundation, until late 2015, when he focused his attention on making the AKASHA dream a reality.

![Mihai Alisie]({{ site.baseurl }}/content/images/Mihai275x.jpg)

Twitter: [@MihaiAlisie](https://twitter.com/MihaiAlisie){:target="_blank"} | 
LinkedIn: [Mihai Alisie](https://www.linkedin.com/in/mihaialisie){:target="_blank"} | 
Contact: [mihai@akasha.world](mailto:mihai@akasha.world)
