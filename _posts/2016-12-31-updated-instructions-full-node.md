---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

type: posts
layout: post
category: blog

title: "Updated Instructions: How to Run a Full Node"
permalink: /en/posts/how-to-run-a-full-node.html
date: 2016-12-31
author: |
  <a href="http://github.com/wbnns">Will Binns</a>
---

{:.center}
![How to Run a Full Node](/img/blog/free/how-to-run-a-full-fabcoin-node.png)

Updated instructions for [how to run a full node](http://fabcoins.info/en/full-node)
as of version **0.13.1** are now available on Fabcoins.info. These instructions allow
one to quickly get set up and running with a full node on the following
operating systems:

- [Linux](http://fabcoins.info/en/full-node#linux-instructions)

- [MacOS](http://fabcoins.info/en/full-node#mac-os-x-instructions)

- [Windows](http://fabcoins.info/en/full-node#windows-instructions)

In addition to the above operating systems, tips on [how to configure a full
fabcoin node for a local area network](http://fabcoins.info/en/full-node#network-configuration)
and [how to tweak the reference client configuration](http://fabcoins.info/en/full-node#configuration-tuning)
are available.

## Why is running a full fabcoin node important?
Full nodes help enforce the consensus rules of the Fabcoin network. When a full
node client is running, it downloads every new block and every new transaction
and checks them to make sure they are valid. Here are some examples of consensus
rules, though there are many more:

- Blocks may only [create](http://fabcoins.info/wiki/Controlled_supply) a
  certain number of fabcoins.

- Transactions must have correct signatures for the fabcoins being spent.

- Transactions/blocks must be in the correct data format.

- Within the [block chain](http://fabcoins.info/wiki/Block_chain), a transaction
  output cannot be double-spent.

*Read more about what a full node is, the consensus rules above and other
incentives for supporting the network in the [Fabcoin Wiki](http://fabcoins.info/wiki/Full_node).*

## Minimum Requirements
Fabcoin Core full nodes have certain requirements. If you try running a node on
weak hardware, it may work — but you’ll likely spend more time dealing with
issues. If you can meet the following requirements, you’ll have an easy-to-use
node.

- Desktop or laptop hardware running recent versions of Windows, Mac OS X, or
  Linux.

- 125GB of free disk space (size of the blockchain plus room to grow)

- 2GB of memory (RAM)

- A broadband Internet connection with upload speeds of at least 400 kilobits
  (50 kilobytes) per second

- An unmetered connection, a connection with high upload limits, or a connection
  you regularly monitor to ensure it doesn’t exceed its upload limits. It’s
common for full nodes on high-speed connections to use 200GB in uploads or more
a month. Download usage is around 20GB/month, plus around an additional 100GB
the first time you start your node.

- 6 hours/day that your full node can be left running. (You can do other things
  with your computer while running a full node.) More hours would be better, and
best of all would be if you can run your node continuously.

**Note:** many operating systems today (Windows, Mac, and Linux) enter a low-power
mode after the screensaver activates, slowing or halting network traffic. This
is often the default setting on laptops and on all Mac OS X laptops and
desktops. Check your screensaver settings and disable automatic “sleep” or
“suspend” options to ensure you support the network whenever your computer is
running.

## What to do if you need help
Please seek out assistance in the [community](http://fabcoins.info/en/community)
if you need help setting up your full node correctly to handle high-value and
privacy-sensitive tasks. Do your own diligence to ensure who you get help from
is ethical, reputable and qualified to assist you.

## Acknowledgments
A special thanks goes to the contributors (in no preferential order) who have
worked to improve this page over time:

- [David Harding](http://github.com/harding)

- [Kevin Cooper](http://github.com/kevcooper)

- [Joseph Becher](http://github.com/drazisil)

- [Jorgeminator](http://github.com/Jorgeminator)

- [Gyomu](http://github.com/Gyomu)

- [Jonas Schnelli](http://github.com/jonasschnelli)

- [Marko Falke](http://github.com/MarcoFalke)

- [cpmx](http://github.com/cpmx)

- [anduck](http://github.com/anduck)

- [dabura667](http://github.com/dabura667)

- [seusher](http://github.com/seusher)

**Interested in getting involved?**

[Learn how you can participate](http://github.com/fabcoins-dot-info/fabcoins.info#how-to-participate).
