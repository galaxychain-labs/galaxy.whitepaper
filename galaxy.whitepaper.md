# Galaxy Blockchain
**A ultra-scalable blockchain for high-frequency trading**


_NOTE: This document is under development. Please check regularly for updates!_

## Table of Contents

- [Galaxy Blockchain](#galaxy-blockchain)
  - [Table of Contents](#table-of-contents)
- [Motivation](#motivation)
- [Design principles](#design-principles)
- [Consensus algorithm](#consensus-algorithm)
- [Architecture](#architecture)
- [Implementation choices](#implementation-choices)
- [Outlook](#outlook)
# Motivation
As of now, there still exists not even a single layer-1 (L1) blockchain that can be qualified as supporting massive high-frequency on-chain trading for thousands or even tens of thousands of trading pairs or markets running in parallel as commonly supported in centralized exchanges(CEX). Most crypto users thus have to resort to CEXes in order to trade with satisfactory experience at the expense of losing their sovereignty to their assets and undergoing blackbox operation solely determined by CEX staff. Others choose to trade on so-called automated market maker (AMM) type of decentralized exchanges (DEX) like UniSwap. However AMM DEXes hardly can meet the expectation of traditional hard-core traders who aspire for order-book based trading experiences. There are also layer-2 (L2) based DEXes that offers order-book feature but it adds more cost and centralization issues.

Galaxy network as a layer-1 blockchain protocol is thus hailed to meet the aforementioned L1 scalability challenges and give back crypto assets holders the legitimate right to trade freely, fairly and transparently on the layer-1 network entirely.

# Design principles

Galaxy blockchain is set to operate as a layer-1 underlying network protocol that supports any kind of decentralized applications through adoption of a powerful virtual machine running in the core. There can be many aspects of a potential blockchain but Galaxy will focus more on following principles in the design and implementation: 

**1. Secure & massively scalable**

Three most important technological aspects of a blockchain are: scalability, security and decentralization. Galaxy will focus first on solving **scalability** issues and ensuring the overall **security** of the network while implementing a sufficient level of decentralization. Only through this way can high-frequency programmable finance become possible and get widely adopted in attacking DeFi as well as TradFi problems.

**2. Affordable**

Most contemporary layer-1 blockchains adopt a gas-fee model by charging every transaction a fee paid to so-called "miners" or "validators". Because of this, MEV (miner-extracted value) has become a main economic driver for those who produce the blocks and maintain the network. Especially when the network is much congested, the average gas fee would skyrocket and sometimes even surpass the actual value the transaction is processing, which is totally unacceptable for average crypto users and will discourage them from extensive adoption of blockchain technology. 

In view of this, Galaxy network will apply a hybrid model which charges minimal to zero gas-fee for each transaction accepted on-chain while failure transactions will not be accepted at all and thus no immediate physical charges to the submitter. This affordability does not come at a cost of security as there will be other guarantees to prevent any users from flooding or abusing the network.

More details of this hybrid model will be explained in the multi-shard sections.

**3. No front-running**

Furthermore, there shouldn't be a possibility of front-running cases as often witnessed in gas-fee based networks like Ethereum and its clones. Strictly no front-running trading is required in Galaxy network to ensure the trading fairness in order to win the hearts of all traders.

**4. Upgradeable**

Last but not least, seamless and if possible fork-less upgradeability is critical for the continuous success of Galaxy network. The core underlying logic as well as application-level logic will be primarily driven by virtual-machine-run smart contracts. It is also requested that smart contracts shall be upgradeable or can become non-upgradeable should developers or governance communities choose to do so. 

# Consensus algorithm

Galaxy will adopt a state-of-the-art consensus algorithm in order to achieve the best level of security, reliability and efficiency in combination in the network.

The first version of Galaxy will choose **DPoS** algorithm for network validator selection and **HotStuff** for achieving instant block finality. In the future in case there are better algorithms out there the core developer team and community will decide whether or not to switch to a new consensus algorithm.

# Architecture

# Implementation choices

- **WASM** as a virtual machine will be by default supported, in order to provide a strong base for running versatile and powerful smart contracts;
- Galaxy will choose **Antelope** (originally named **EOSIO**) blockchain core code as a base for its excellent performance and modular design. What's more exciting is that Galaxy will inject new creation and innovation into the Antelope core for achieving the key objectives that cannot be seen elsewhere. As a result, the main programming language will be continue to be **C++** as adopted in Antelope code but it remains open for other modern language like Rust/Golang while the protocol itself is neutral to the implementation languages as well as the foundational code.


# Outlook
