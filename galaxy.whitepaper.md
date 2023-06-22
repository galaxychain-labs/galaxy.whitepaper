# Galaxy Blockchain
**A ultra-scalable blockchain for high-frequency programmable finance


_NOTE: This document is under development. Please check regularly for updates!_

## Table of Contents

- [Motivation](#motivation)
- [Design Principles](#design-principles)
- [Consensus Algorithm](#consensus-and-validator-quorum)
  * [Proof of Stake](#proof-of-staked-authority)
  * [Validator Quorum](#validator-quorum)
  * [Security and Finality](#security-and-finality)
  * [Reward](#reward)
- [Tokenomics](#token-economy)
  * [Native Token](#native-token)
  * [Other Tokens](#other-tokens)
- [Architecture](#architecture)
  * [Account model](#cross-chain-transfer)
  * [Resource model](#bc-to-bsc-architecture)
  * [Scalability design](#bsc-to-bc-architecture)
    * [Multichain and xChain](#timeout-and-error-handling)
    * [Multishard and xShard](#cross-chain-user-experience)
- [Outlook](#outlook)
# Motivation
As of now, there still exists not even a single layer-1 (L1) blockchain that can be qualified as supporting massive high-frequency on-chain trading for thousands of even tens of thousands of trading pairs as commonly supported in centralized exchanges(CEX). Most crypto users thus have to resort to CEXes in order to trade with satisfactory experience. Others choose to trade on so-called automated market maker (AMM) type of dencentralized exchanges (DEX) like UniSwap. However AMM DEXes hardly can meet the expectation of traditional hard-core traders who aspire for order-book based trading experiences. There are also layer-2 (L2) based DEXes that offers order-book feature but it adds more cost and centralization issues.

Galaxy network as a layer-1 blockchain protocol is thus haild to meet the abovementioned L1 scalability challenges and give back crypto assets holders the legitimate right to trade freely, fairly and transparently on the layer-1 network entirely.